# MEMORY — RiskMind AI

This file stores lightweight persistent memory for RiskMind AI.

Do not store full policies, SOPs, playbooks, confidential customer data, or raw document content.

Use this file only for:

* Important document index
* Frequently asked stakeholder questions
* Documentation gaps
* Ownership clarifications
* Stakeholder feedback
* Risk investigation heuristics

---

# Important Knowledge Sources

| Document Name                | Type        | Topic                                | Owner     | Location                                                                   | Notes                                                                         |
| ---------------------------- | ----------- | ------------------------------------ | --------- | -------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| ATO Cheat Sheet (NhuTN)      | Cheat Sheet | ATO, Payment Platform, Risk Mapping  | NhuTN     | `/root/.openclaw/workspace/KNOWLEDGE_BASE/ato_cheat_sheet.md`              | Reference for AppID, PMC ID, Authen, Trusted Device and Risk Decision Mapping |
| Fraud Risk Criteria          | Policy      | Fraud assessment framework           | NhuTN     | `/root/.openclaw/workspace/KNOWLEDGE_BASE/fraud_risk_criteria.md`          | Risk classification and handling framework                                    |
| Merchant Onboarding Standard | Standard    | Merchant onboarding and restrictions | BD / Risk | `/root/.openclaw/workspace/KNOWLEDGE_BASE/merchant_onboarding_standard.md` | Merchant due diligence and restrictions                                       |

---

# Frequently Asked Questions

## Domain Model

### How is a ZaloPay transaction described?

A transaction is typically described by:

* AppID (product/service)
* TransType (transaction type)
* PMC ID (source of fund)
* zpsystem (payment channel)
* sofaction (payment method)
* Authentication method
* Risk decision

These attributes are the primary dimensions used in fraud investigation and transaction analysis.

---

## Payment Platform

### What is AppID?

AppID identifies a ZaloPay product or service.

Important AppID groups:

| Group                 | AppID                 |
| --------------------- | --------------------- |
| Transfer              | 450 (P2P), 241 (IBFT) |
| Withdraw              | 452, 888              |
| Topup                 | 454                   |
| Disbursement          | 1228, 3253            |
| Credit Card Repayment | 45                    |
| Internal Operation    | 1                     |

### Which AppIDs are most important for ATO or Wallet Fraud investigations?

Priority:

* 450 (P2P Transfer)
* 241 (IBFT Transfer)
* 452 (Withdraw)
* 454 (Topup)

These AppIDs directly affect money movement.

---

## Transaction Flow

### What is TransType?

TransType identifies the transaction category.

Fund-in examples:

* Topup Wallet
* Bank Topup
* Receive Money

Fund-out examples:

* Payment
* Transfer
* Withdraw
* QR Payment
* Gateway Payment

### Which TransTypes are most relevant when evaluating financial loss?

Focus on:

* Payment
* Transfer
* Withdraw

These activities reduce user assets.

---

## Source Of Fund

### What is PMC ID?

PMC ID (Payment Channel ID) identifies the source of funds used in a transaction.

### What are the major source-of-fund categories?

Internal funds:

* Wallet Balance
* MMF
* Fixed Deposit
* Stock Balance

External funds:

* Bank Account
* ATM API
* Credit Card
* Debit Card

### When is a source of fund considered Low Risk?

When total confirmed balance ≤ 200,000 VND.

### When is a source of fund considered High Risk?

When:

* Confirmed balance > 200,000 VND.
* Balance source cannot be fully identified.

---

## Login & Ownership

### What login methods are supported?

* Phone Number + PIN + OTP
* Zalo OAuth

### Why is Zalo OAuth useful during investigations?

It links a wallet UserID to a ZaloID and helps establish account ownership.

---

## Trusted Device

### What is a Trusted Device?

A device with established transaction history and successful authentication history.

### Typical Trusted Device signals

* Historical transactions exist.
* Historical OTP verification exists.
* Not in blacklist.
* Long-lived device.
* Historical fund-out activity exists.

### Why is Trusted Device important?

It is one of the strongest signals for distinguishing legitimate users from account takeover attempts.

---

## Authentication

### Authentication strength hierarchy

Captcha → PIN → Biometrics → OTP → SmartOTP → KYC → Face Authentication → NFC → BCA Validation

### Face Authentication types

* Passive Face Authentication
* Active Face Authentication

### Why is NFC alone insufficient?

NFC data may be cloned or replayed.

Strong verification should combine:

* NFC
* Face Authentication
* BCA verification

### Can SmartOTP replace SMS OTP?

Yes.

SmartOTP is considered a stronger authentication mechanism and can replace SMS OTP in many scenarios.

---

## Payment Channel

### What is zpsystem?

Determines whether a transaction originates from:

* ZP_WALLET
* ZP_GATEWAY

### What is sofaction?

Identifies the specific payment method selected by the user.

Examples:

* Apple Pay
* Card On File

---

## Refund

### How is refund destination determined?

Refund routing depends on:

* PMC ID
* Bank connector
* zpsystem
* TransType
* Payment service configuration

### Common refund behavior

* Wallet Balance → Wallet
* Credit Card → Bank
* Debit Card → Bank or Wallet depending on configuration

---

## Risk Engine

### What is a Risk Decision?

The decision generated by Risk Engine for a transaction.

Each decision maps to a transaction status.

### Major Risk Categories

* Wallet Risk
* Fraud Risk
* KYC Risk
* Credit Risk
* Promotion Abuse
* Merchant Risk

### Common status mappings

| Risk Type | Reject | Challenge |
| --------- | ------ | --------- |
| Wallet    | -348   | -356      |
| Fraud     | -357   | -354      |
| Credit    | -358   | -363      |
| KYC       | -359   | N/A       |

---

## Post Mortem

### What is Post Mortem (POM)?

Analysis of confirmed ATO users and transactions for loss assessment, investigation and detection improvement.

### Typical ATO Loss Characteristics

* Labeled as ATO.
* Successful transaction.
* Payment or transfer activity.
* Not internal topup activity.

---

## Investigation Heuristics

### Recommended ATO investigation sequence

1. Trusted Device
2. Login Method
3. Source Of Fund
4. Topup History
5. Transfer / Withdraw Activity
6. Authentication History
7. OTP History
8. Face Authentication Result
9. Risk Decision

### Common Account Takeover indicators

* New device
* Abnormal login behavior
* Authentication method changes
* Unusual topup behavior
* Immediate transfer or withdrawal after topup
* Behavior inconsistent with historical patterns
* Successful challenge using previously unseen methods

### Signals supporting legitimate ownership

* Trusted Device
* Historical OTP success
* Long-term device history
* Successful Face Authentication
* Behavior consistent with historical usage

---

# Operational Knowledge

### SLA - CS - Risk Ticket Routing

| Domain | PIC | Routing Rule | SLA (WD = working days) |
|----------|----------|----------|----------|
| Account Risk | NhuTN | InfoCode 2xxxx, 3xxxx, disputed txn, account requests | 3-5 WD |
| Promotion Abuse | AnhTP6 | -332, -333, -361, InfoCode 1xxxx, 7xxxx | 3-5 WD |
| KYC Risk | AnhTP6 | KYC-related issues | 3-5 WD |
| Partner Risk | VyNT | InfoCode 4xxxx, merchant complaints | 3-5 WD |
| Credit Risk | TramCTB | -358, InfoCode 6xxxx | 5 WD |
| Trust Score | DatHT | Trust score issues | 3-5 WD |

---

## Risk Review Requirement - SLA for process review/assessment is 2 working weeks

Risk review is required if a change affects:

- User funds or money movement
- Transaction validation or authorization logic
- Account security (PIN, phone, KYC, face auth, OTP)
- Core system integrations or Risk-related APIs
- Promotion, reward, or incentive mechanisms

Risk review is NOT required only when ALL above conditions are unaffected.
---

# Unresolved Questions

| Date | Question | Missing Evidence | Suggested Owner | Status |
| ---- | -------- | ---------------- | --------------- | ------ |
| TBD  | TBD      | TBD              | TBD             | Open   |

---

# Documentation Gaps

| Date | Gap | Impact | Suggested Action | Owner | Status |
| ---- | --- | ------ | ---------------- | ----- | ------ |
| TBD  | TBD | TBD    | TBD              | TBD   | Open   |

---

# Stakeholder Feedback

| Date | Team | Feedback | Suggested Improvement | Status |
| ---- | ---- | -------- | --------------------- | ------ |
| TBD  | TBD  | TBD      | TBD                   | Open   |

---

# Operating Reminder

RiskMind AI must not answer policy, SOP, playbook, ownership, approval, or compliance questions from memory alone.

Always retrieve and cite approved documentation when available.

If evidence is unavailable, respond:

"I cannot find sufficient evidence from the available documents to provide a definitive conclusion. Please consult the document owner or Risk Team before proceeding."