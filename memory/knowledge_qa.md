# Knowledge Q&A - BD & Risk Questions

## Hướng dẫn sử dụng
Khi có ai hỏi câu hỏi bên dưới, trả lời CHÍNH XÁC theo nội dung đã học. Không được thay đổi, không được tìm kiếm thêm.

---

## Q1: BD có cần chờ team Risk duyệt hồ sơ trước khi tích hợp Merchant không?
**Trả lời:** Không cần ạ. Từ tháng 4/2025, BD được chủ động thực hiện thẩm định Merchant theo bộ tiêu chí của Risk mà không cần thông qua sự xác nhận của Risk. Tuy nhiên, BD phải điền đầy đủ thông tin vào "Biểu mẫu thẩm định" và lưu trữ tại Merchant Admin Tool để phục vụ hậu kiểm.

---

## Q2: Ngành hàng bán thuốc (Pharmacy) có được mở thẻ quốc tế không?
**Trả lời:** Có, ngành hàng bán thuốc đã được loại ra khỏi danh sách hạn chế. Merchant ngành này có thể được mở Full nguồn tiền (bao gồm thẻ quốc tế), nhưng vì đây là ngành nghề High-risk MCC nên BD bắt buộc phải thông báo cho Risk khi thực hiện tích hợp.

---

## Q3: Trong version 2026, nội dung cập nhật chính là gì?
**Trả lời:** Cập nhật bảng ngành hàng kinh doanh và các nguồn tiền được mở tương ứng, đặc biệt ngành bán thuốc/pharmacy được loại khỏi bảng ngành hàng hạn chế nguồn tiền và có thể mở full nguồn tiền, nhưng cần thông báo Risk vì là high-risk MCC.

---

## Q4: Merchant Cross-border trong version 2026 cần đáp ứng điều kiện gì?
**Trả lời:** Merchant không thuộc blacklist của Risk và không thuộc danh sách ngành nghề hạn chế mở nguồn tiền Paylater.

---

## Q5: Merchant Cross-border nếu đạt điều kiện thì có thể tích hợp những nguồn tiền nào?
**Trả lời:** Có thể tích hợp: Số dư ví, ATM, Tài khoản ngân hàng, VietQR, Số dư sinh lời, Tài khoản trả sau, Tài khoản trả góp.

---

## Q6: Nếu lỡ onboarding sai tiêu chuẩn của TCTQT, hậu quả là gì?
**Trả lời:** Hậu quả rất nghiêm trọng cho ZaloPay:
- Bị phạt từ 50.000 - 200.000 USD nếu vi phạm quy trình KYC/KYB
- Bị phạt từ 100.000 USD trở lên nếu xử lý thanh toán cho ngành nghề bị cấm hoặc rủi ro cao
- Nguy cơ bị Ngân hàng thanh toán hoặc TCTQT ngừng hợp tác, mất khả năng cung cấp dịch vụ thanh toán thẻ

---

## Q7: Nếu không tuân thủ tiêu chí thẩm định của TCTQT, ZaloPay có thể gặp rủi ro gì?
**Trả lời:** Có thể bị ngân hàng thanh toán hoặc TCTQT ngừng hợp tác, mất khả năng cung cấp dịch vụ thanh toán thẻ, bị phạt vì không tuân thủ KYC/KYB, hoặc bị phạt khi xử lý thanh toán cho ngành nghề cấm/rủi ro cao.

---

## Q8: Mức phạt không tuân thủ quy trình KYC/KYB có thể là bao nhiêu?
**Trả lời:** Từ 50.000 đến 200.000 USD nếu bị phát hiện.

---

## Q9: Mức phạt khi xử lý thanh toán cho ngành nghề bị cấm hoặc rủi ro cao có thể từ bao nhiêu?
**Trả lời:** Từ 100.000 USD trở lên, tùy mức độ nghiêm trọng.

---

## Q10: Các nhóm nguồn tiền áp dụng trong quy trình gồm những gì?
**Trả lời:** Gồm Số dư ví, Số dư sinh lời, nguồn tiền thẻ nội địa, nguồn tiền trả sau, nguồn tiền thẻ quốc tế và các phương thức khác.

---

## Q11: Nguồn tiền thẻ nội địa bao gồm những gì?
**Trả lời:** ATM và Tài khoản ngân hàng.

---

## Q12: Nguồn tiền trả sau bao gồm những gì?
**Trả lời:** Tài khoản trả sau và Tài khoản trả góp.

---

## Q13: Nguồn tiền thẻ quốc tế bao gồm những gì?
**Trả lời:** Thẻ Credit và Thẻ Debit quốc tế.

---

## Q14: Các phương thức khác gồm những gì?
**Trả lời:** VietQR, Apple Pay và Google Pay.

---

## Q15: Merchant có luôn được mở tất cả nguồn tiền không?
**Trả lời:** Không. Việc mở toàn bộ hoặc một phần nguồn tiền phụ thuộc vào mô hình kinh doanh, ngành hàng và phương thức tích hợp.

---

## Q20: Đối tác như thế nào đủ điều kiện mở nguồn tiền thẻ quốc tế?
**Trả lời:** Là Doanh nghiệp, Hộ kinh doanh hoặc Cá nhân đăng ký kinh doanh tại Việt Nam.

---

## Q21: Merchant cần có phạm vi hoạt động ở đâu để đủ điều kiện mở thẻ quốc tế?
**Trả lời:** Merchant cần có hoạt động bán hàng hoặc cung cấp dịch vụ tại phạm vi địa lý Việt Nam.

---

## Q22: Merchant nước ngoài có được tích hợp thẻ quốc tế không?
**Trả lời:** Không. Merchant nước ngoài không được tích hợp thẻ quốc tế.

---

## Q23: Merchant nước ngoài được tích hợp những nguồn tiền cơ bản nào?
**Trả lời:** Số dư ví, ATM, Tài khoản ngân hàng, và có thể mở thêm Tài khoản trả sau/Trả góp nếu đáp ứng điều kiện ngành nghề.

---

## Q24: Vì sao Merchant nước ngoài không được mở thẻ quốc tế?
**Trả lời:** Theo Visa/Mastercard rules, Sponsored Merchant phải được thành lập và hoạt động tại cùng quốc gia với Acquirer. Acquirer của ZaloPay hiện tại là Sacombank và VietinBank tại Việt Nam, nên Merchant phải là Merchant Việt Nam.

---

## Q25: Có mấy nhóm yếu tố chính cần kiểm tra khi thẩm định hình thức kinh doanh?
**Trả lời:** Có 4 nhóm: Bên mua, Bên bán, Sản phẩm/dịch vụ kinh doanh, và Kênh bán hàng.

---

## Q26: Ở bước kiểm tra Merchant Profile, cần kiểm tra nội dung gì?
**Trả lời:** Kiểm tra Merchant có thuộc blacklist rủi ro cao trong danh sách nội bộ ZaloPay/Partner Risk hay không.

---

## Q27: Khi kiểm tra blacklist, BD cần kiểm tra những thông tin nào?
**Trả lời:** Kênh bán hàng website/app, thông tin công ty như tên công ty/mã số thuế, và thông tin người đại diện pháp luật như họ tên/CCCD.

---

## Q28: Nếu Merchant không nằm trong blacklist thì xử lý thế nào?
**Trả lời:** Chuyển sang kiểm tra các tiêu chí tiếp theo.

---

## Q29: Nếu Merchant có thông tin nằm trong blacklist thì xử lý thế nào?
**Trả lời:** Cân nhắc từ chối hợp tác.

---

## Q30: Ở bước kiểm tra sản phẩm/dịch vụ, cần xác định điều gì?
**Trả lời:** Cần xác định Merchant có kinh doanh sản phẩm/dịch vụ thuộc bảng ngành nghề hạn chế ở mục 3.1 hay không.

---

## Q31: Nếu sản phẩm/dịch vụ không thuộc bảng ngành nghề hạn chế thì nguồn tiền được áp dụng thế nào?
**Trả lời:** Áp dụng tất cả các nguồn tiền.

---

## Q32: Nếu sản phẩm/dịch vụ thuộc bảng ngành nghề hạn chế thì nguồn tiền được áp dụng thế nào?
**Trả lời:** Chỉ áp dụng các nguồn tiền còn lại sau khi loại trừ nguồn tiền không được phép theo bảng ngành hàng.

---

## Q33: Ngành Cyberlockers không được áp dụng nguồn tiền nào?
**Trả lời:** Không được áp dụng Thẻ Credit & Debit quốc tế.

---

## Q34: Ngành bán thuốc trong version 2026 được xử lý như thế nào?
**Trả lời:** Ngành bán thuốc có thể được áp dụng full nguồn tiền, nhưng cần thông báo Risk vì đây là high-risk MCC.

---

## Q35: Game phải trả tiền để vào chơi như STEAM không được áp dụng nguồn tiền nào?
**Trả lời:** Không được áp dụng Thẻ Credit & Debit quốc tế.

---

## Q36: Văn hóa phẩm đồi trụy có được tích hợp ZaloPay không?
**Trả lời:** Không. Đây là ngành thuộc nhóm ngành cấm, không được tích hợp ZaloPay.

---

## Q37: Giao dịch tài chính liên quan đến tiền ảo, tiền điện tử không được áp dụng nguồn tiền nào?
**Trả lời:** Không được áp dụng Thẻ Credit & Debit quốc tế.

---

## Q38: Giao dịch mua bán hoặc môi giới công cụ tài chính phái sinh không được áp dụng nguồn tiền nào?
**Trả lời:** Không được áp dụng Thẻ Credit & Debit quốc tế, Tài khoản trả sau và Tài khoản trả góp.

---

## Q39: Ngành thẻ quà tặng không được áp dụng nguồn tiền nào?
**Trả lời:** Không được áp dụng Tài khoản trả sau và Tài khoản trả góp.

---

## Q40: Ngành thẻ điện thoại, thẻ game ngoài VNG không được áp dụng nguồn tiền nào?
**Trả lời:** Không được áp dụng Thẻ Credit & Debit quốc tế, Tài khoản trả sau và Tài khoản trả góp.

---

## Q41: Ngành thanh toán thẻ tín dụng, khoản vay tiêu dùng không được áp dụng nguồn tiền nào?
**Trả lời:** Không được áp dụng Thẻ Credit quốc tế, Tài khoản trả sau và Tài khoản trả góp.

---

## Q42: Các Merchant thuộc ngành Game sẽ được xử lý thẩm định thế nào?
**Trả lời:** Merchant ngành Game, kể cả in-house hoặc out-house, vẫn phải chuyển trực tiếp cho Risk thẩm định.

---

## Q43: Với kênh Offline, tiêu chí cần kiểm tra là gì?
**Trả lời:** Kiểm tra Merchant có địa điểm kinh doanh đúng như khai báo hay không.

---

## Q44: Với kênh Offline, hồ sơ kiểm tra bắt buộc gồm những hình ảnh nào?
**Trả lời:** Hình ảnh chụp hàng hóa/dịch vụ kinh doanh và hình ảnh tổng quan địa điểm kinh doanh có bảng hiệu, địa chỉ khớp với thông tin khai báo.

---

## Q45: Với kênh Online, có những nhóm tiêu chí cần kiểm tra nào?
**Trả lời:** Mô tả hàng hóa/dịch vụ, chính sách ảnh hưởng đến quyền lợi người dùng, luồng thanh toán cơ bản, và thông tin tiếp nhận/xử lý khiếu nại.

---

## Q46: Danh mục sản phẩm trên website/app cần có những thông tin gì?
**Trả lời:** Cần có đơn vị tiền tệ là VND và có thành phần sản phẩm đối với sản phẩm vật lý hoặc mô tả dịch vụ đối với sản phẩm phi vật lý/dịch vụ.

---

## Q47: Các trường hợp thường gặp khiến mô tả sản phẩm/dịch vụ không đạt yêu cầu là gì?
**Trả lời:** Sản phẩm/dịch vụ để giá liên hệ, sản phẩm vật lý không có hình ảnh, hoặc sản phẩm/dịch vụ không có thông tin mô tả.

---

## Q48: Kênh Online cần có những chính sách nào?
**Trả lời:** Điều kiện hủy giao dịch và đổi/trả hàng, chính sách hoàn tiền, chính sách giao hàng, và chính sách bảo mật thông tin.

---

## Q49: Nếu Merchant có nhiều loại hàng hóa/dịch vụ khác nhau thì chính sách cần thể hiện thế nào?
**Trả lời:** Mỗi loại hàng hóa/dịch vụ cần có chính sách và quy định riêng phù hợp.

---

## Q50: Các trường hợp không đạt yêu cầu về chính sách thường gặp là gì?
**Trả lời:** Kênh bán hàng không có chính sách, không thể hiện đầy đủ thông tin chính sách, hoặc Merchant nói không có chính sách hoàn trả nhưng nội dung này không được thể hiện trên kênh bán hàng.

---

## Q51: Chính sách đổi/trả hàng cần có những nội dung gì?
**Trả lời:** Điều kiện đổi trả hàng, thời gian cho phép đổi trả hàng, và hình thức đổi trả hàng.

---

## Q52: Chính sách hoàn tiền cần có những nội dung gì?
**Trả lời:** Điều kiện được hoàn tiền và thời gian hoàn tiền.

---

## Q53: Chính sách vận chuyển đối với hàng hóa vật lý cần có gì?
**Trả lời:** Phạm vi giao hàng và thời gian vận chuyển.

---

## Q54: Chính sách vận chuyển đối với hàng hóa phi vật lý/dịch vụ cần có gì?
**Trả lời:** Hình thức cung cấp hàng hóa/dịch vụ và thời gian cung cấp hàng hóa/dịch vụ.

---

## Q55: Chính sách bảo mật thông tin cần có gì?
**Trả lời:** Các thông tin cá nhân được bảo mật và nơi lưu trữ thông tin bảo mật.

---

## Q56: Luồng thanh toán cơ bản trên kênh Online cần có những bước nào?
**Trả lời:** Chọn hàng hóa/dịch vụ, điền thông tin khách hàng, và chọn phương thức thanh toán.

---

## Q57: Thông tin khách hàng trong luồng thanh toán cần gồm những gì?
**Trả lời:** Họ tên, thông tin liên hệ như SĐT/email, và địa chỉ giao hàng.

---

## Q58: Các trường hợp không đạt yêu cầu về luồng thanh toán thường gặp là gì?
**Trả lời:** Kênh bán hàng không có luồng thanh toán hoặc luồng thanh toán bị lỗi.

---

## Q59: Thông tin CSKH trên website/app cần có những gì?
**Trả lời:** Tên công ty, địa chỉ kinh doanh, số điện thoại và email.

---

## Q60: Các trường hợp không đạt yêu cầu về CSKH thường gặp là gì?
**Trả lời:** Kênh bán hàng không có thông tin CSKH hoặc thông tin CSKH không hoạt động.

---

## Q61: Nội dung chính sách và điều khoản T&C cần phù hợp với yếu tố nào?
**Trả lời:** Phải phù hợp với sản phẩm/dịch vụ tích hợp thanh toán ZaloPay.

---

## Q62: T&C có được dẫn link sang kênh khác không?
**Trả lời:** Không được dẫn sang kênh khác mà Merchant không có quyền sở hữu. Nội dung T&C phải nằm trên cùng website/ứng dụng.

---

## Q63: Mục đích của việc thu thập và điền phiếu đánh giá thẩm định là gì?
**Trả lời:** Hỗ trợ lưu trữ, audit khi cần và làm cơ sở chứng minh BD team đã kiểm tra theo quy định của TCTQT.

---

## Q64: Bộ hồ sơ lưu trữ thông tin thẩm định của từng Merchant bao gồm gì?
**Trả lời:** Biểu mẫu thẩm định upload lên Merchant profile tại Merchant Admin Tool và file Excel lưu trữ toàn bộ Merchant được onboarding tại ZaloPay để Risk hậu kiểm.

---

## Q65: Trong biểu mẫu thẩm định, phần "Phòng ban đánh giá" cần ghi như thế nào?
**Trả lời:** Ghi cụ thể phòng ban như DLS, DGS, MBS – Bộ phận phát triển kinh doanh.

---

## Q66: Trong biểu mẫu, phần nguồn tiền thanh toán được mở cần ghi như thế nào?
**Trả lời:** Liệt kê đầy đủ các nguồn tiền được mở như Số dư ví, thẻ ATM, Tài khoản ngân hàng, Tài khoản trả sau, Số dư sinh lời, VietQR, thẻ ghi nợ và tín dụng quốc tế.

---

## Q67: Trong biểu mẫu, phần mức độ rủi ro cần điền theo căn cứ nào?
**Trả lời:** Điền mức độ rủi ro theo bảng Risk đã gửi.

---

## Q68: Khi tick "Có" cho các chính sách trong biểu mẫu, cần lưu ý gì?
**Trả lời:** Chỉ tick "Có" với các chính sách đã được thể hiện trên kênh bán hàng.

---

## Q69: Người duyệt trong biểu mẫu cần ghi thông tin gì?
**Trả lời:** Ghi domain của line manager.

---

## Q71: Merchant nước ngoài muốn mở thẻ quốc tế, BD nên xử lý thế nào?
**Trả lời:** Không mở thẻ quốc tế. Chỉ xem xét mở các nguồn tiền cơ bản như Số dư ví, ATM, Tài khoản ngân hàng và Paylater/Trả góp nếu ngành nghề đáp ứng điều kiện.

---

## Q76: Merchant bán thuốc có được mở full nguồn tiền không?
**Trả lời:** Có thể được mở full nguồn tiền theo update 2026, nhưng cần thông báo Risk vì đây là high-risk MCC.

---

_Cập nhật: 2026-06-17_

---

# Transaction Risk Assessment Q&A

## Q-1: Mục đích của hệ thống đánh giá rủi ro giao dịch là gì?
**Trả lời:** Phát hiện sớm dấu hiệu gian lận, hỗ trợ quyết định chấp nhận, xác thực bổ sung hoặc từ chối giao dịch.

## Q-2: Hệ thống đánh giá rủi ro áp dụng cho những loại giao dịch nào?
**Trả lời:** Chuyển tiền, IBFT, thanh toán dịch vụ, thanh toán merchant, nạp tiền, rút tiền và giao dịch liên quan đến tài khoản ngân hàng hoặc thẻ.

## Q-3: Hệ thống đánh giá rủi ro có bao gồm AML không?
**Trả lời:** Không. Tài liệu này không bao gồm phòng chống rửa tiền và tài trợ khủng bố.

## Q-4: Rủi ro giao dịch được đánh giá dựa trên những yếu tố nào?
**Trả lời:** Người dùng, thiết bị, hành vi giao dịch và các mối liên kết liên quan.

## Q-5: Rủi ro giao dịch được đánh giá ở những giai đoạn nào?
**Trả lời:** Trước giao dịch, trong giao dịch và sau giao dịch.

## Q-6: Có bao nhiêu mức độ rủi ro giao dịch?
**Trả lời:** Low Risk, Medium Risk và High Risk.

## Q-7: Low Risk được xử lý như thế nào?
**Trả lời:** Chấp nhận giao dịch và không yêu cầu xác thực bổ sung.

## Q-8: Medium Risk được xử lý như thế nào?
**Trả lời:** Áp dụng xác thực tăng cường như OTP, Smart OTP hoặc xác thực sinh trắc học.

## Q-9: High Risk được xử lý như thế nào?
**Trả lời:** Có thể từ chối giao dịch, yêu cầu xác minh bổ sung hoặc chặn giao dịch.

## Q-10: Khi nào giao dịch bị chặn ngay lập tức?
**Trả lời:** Khi có dấu hiệu gian lận rõ ràng hoặc mức độ rủi ro rất cao.

## Q-11: Những nguồn dữ liệu nào được sử dụng để đánh giá rủi ro?
**Trả lời:** Dữ liệu nội bộ Zalopay, cảnh báo từ cơ quan quản lý, ngân hàng, Napas, tổ chức thẻ và phản ánh của khách hàng.

## Q-12: Blacklist trong đánh giá rủi ro là gì?
**Trả lời:** Danh sách các đối tượng hoặc yếu tố đã được xác định có rủi ro gian lận cao.

## Q-13: Người dùng đã xác nhận gian lận có thuộc blacklist không?
**Trả lời:** Có.

## Q-14: BIN thẻ thuộc danh sách rủi ro cao có phải tín hiệu gian lận không?
**Trả lời:** Có.

## Q-15: Merchant có tỷ lệ gian lận cao có được xem là yếu tố rủi ro không?
**Trả lời:** Có.

## Q-16: Đăng nhập từ thiết bị mới có phải tín hiệu rủi ro không?
**Trả lời:** Có, vì khác với lịch sử sử dụng trước đó của người dùng.

## Q-17: Nhiều giao dịch lặp lại trong thời gian ngắn có thể cho thấy điều gì?
**Trả lời:** Có thể là hành vi dò số dư, thử thông tin thanh toán hoặc gian lận tự động.

## Q-18: Velocity Risk là gì?
**Trả lời:** Rủi ro liên quan đến số lượng hoặc tổng giá trị giao dịch vượt ngưỡng trong một khoảng thời gian.

## Q-19: Hành vi chia nhỏ giao dịch có được xem là tín hiệu rủi ro không?
**Trả lời:** Có, vì có thể nhằm né tránh cơ chế kiểm soát.

## Q-20: Địa chỉ IP từ khu vực rủi ro cao có được xem là tín hiệu gian lận không?
**Trả lời:** Có.

## Q-21: Tài khoản mới tạo nhưng phát sinh giao dịch lớn có phải tín hiệu rủi ro không?
**Trả lời:** Có.

## Q-22: Tài khoản không hoạt động từ 180 ngày trở lên rồi giao dịch lớn có phải tín hiệu rủi ro không?
**Trả lời:** Có.

## Q-23: Những cơ chế kiểm soát nào được áp dụng trước giao dịch?
**Trả lời:** KYC và xác thực đa yếu tố MFA.

## Q-24: Risk Engine được sử dụng ở giai đoạn nào?
**Trả lời:** Trong giao dịch (In-Transaction).

## Q-25: Rule-based Detection dùng để làm gì?
**Trả lời:** Phát hiện các hành vi hoặc giao dịch có dấu hiệu bất thường theo các quy tắc được thiết lập.

## Q-26: Tần suất giao dịch tăng đột biến có phải tín hiệu rủi ro không?
**Trả lời:** Có.

## Q-27: Giao dịch vào khung giờ rủi ro cao có phải tín hiệu rủi ro không?
**Trả lời:** Có.

## Q-28: Giá trị giao dịch vượt xa lịch sử thông thường có phải tín hiệu rủi ro không?
**Trả lời:** Có.

## Q-29: Tài khoản nhận tiền nằm trong mạng lưới gian lận có được xem là rủi ro cao không?
**Trả lời:** Có.

## Q-30: Những loại hàng hóa nào cần được giám sát đặc biệt?
**Trả lời:** Thẻ cào, thẻ game và nạp điện thoại do có khả năng chuyển đổi thành tiền mặt cao.

## Q-31: Mã lỗi bất thường từ ngân hàng có được dùng để đánh giá rủi ro không?
**Trả lời:** Có.

## Q-32: AI và Machine Learning được sử dụng để làm gì?
**Trả lời:** Dự đoán nguy cơ gian lận và phát hiện các mẫu gian lận mới chưa có trong rule.

## Q-33: Sau giao dịch hệ thống còn tiếp tục đánh giá rủi ro không?
**Trả lời:** Có.

## Q-34: Khiếu nại gian lận từ khách hàng ảnh hưởng như thế nào đến đánh giá rủi ro?
**Trả lời:** Giao dịch có thể được phân loại là giao dịch rủi ro cao.

## Q-35: Dữ liệu tra soát và tranh chấp được sử dụng để làm gì?
**Trả lời:** Cập nhật và hiệu chỉnh các tiêu chí đánh giá rủi ro.

## Q-36: Giao dịch được khách hàng xác nhận hợp lệ được phân loại như thế nào?
**Trả lời:** Không rủi ro.

## Q-37: Feedback loop trong hệ thống quản lý rủi ro là gì?
**Trả lời:** Liên tục cập nhật rule và model dựa trên các fraud case thực tế.

## Q-38: Đơn vị nào chịu trách nhiệm xây dựng tiêu chí đánh giá rủi ro?
**Trả lời:** Phòng Quản lý Rủi ro.

## Q-39: Những KPI nào được dùng để đánh giá hiệu quả hệ thống rủi ro?
**Trả lời:** Tỷ lệ gian lận, tỷ lệ từ chối giao dịch, tỷ lệ xác thực bổ sung và các chỉ số vận hành khác.

---

## 6. Disputed / Unrecognized Transactions

### Q82. Với giao dịch không thừa nhận, CS có cần chuyển Risk ngay không?
**Trả lời:** Không cần chuyển Risk ngay; CS phải sử dụng Investigation Tool để chủ động kiểm tra giao dịch trước.

### Q83. Vì sao quy trình giao dịch không thừa nhận được thay đổi?
**Trả lời:** Quy trình được thay đổi để giảm việc CS tạo ticket chuyển Risk cho mọi case trong khi Risk thường chỉ cung cấp thông tin giao dịch và không can thiệp thêm với Medium Risk.

### Q84. Các bước CS xử lý giao dịch không thừa nhận là gì?
**Trả lời:** CS tiếp nhận thông tin từ khách hàng, dùng Investigation Tool kiểm tra giao dịch, phản hồi khách hàng theo kịch bản tra soát và lưu case.

### Q85. Khi Investigation Tool không trả kết quả thì CS làm gì?
**Trả lời:** CS tạo ticket và chuyển Risk xử lý tiếp.

### Q86. Khi kết quả điều tra cho thấy giao dịch có xác thực mật khẩu thanh toán thì nên phản hồi thế nào?
**Trả lời:** CS phản hồi rằng giao dịch được thực hiện có xác thực mật khẩu thanh toán và yêu cầu khách hàng kiểm tra lại giao dịch cũng như việc chia sẻ thông tin bảo mật cá nhân.

### Q87. Nếu log đăng nhập cho thấy tài khoản đăng nhập thành công trên thiết bị liên quan giao dịch nghi ngờ thì phản hồi thế nào?
**Trả lời:** CS cần thông tin cho khách hàng rằng hệ thống ghi nhận đăng nhập thành công trên thiết bị liên quan và yêu cầu khách hàng kiểm tra lại việc sử dụng hoặc chia sẻ thông tin bảo mật.

---

## 7. High Risk / Xác Minh Chính Chủ

### Q88. Những yêu cầu nào được xem là High Risk trong quy trình chủ tài khoản?
**Trả lời:** Các yêu cầu như thu hồi tiền, thanh lý số dư, đổi số điện thoại, mở khóa tài khoản, đóng tài khoản, reset PIN, tái sử dụng SIM và trust thẻ CYBS được xem là High Risk.

### Q89. Với High Risk request, khách hàng cần làm gì trước khi CS hỗ trợ?
**Trả lời:** Khách hàng cần xác minh chính chủ theo quy trình và cung cấp chứng từ đúng, đầy đủ theo từng loại yêu cầu.

### Q90. Nếu khách hàng cung cấp đầy đủ và đúng chứng từ thì CS làm gì?
**Trả lời:** CS hỗ trợ khách hàng theo quy trình tương ứng.

### Q91. Nếu chứng từ nghi ngờ gian lận thì CS làm gì?
**Trả lời:** CS từ chối hỗ trợ khách hàng.

### Q92. Nếu khách hàng không thể cung cấp đủ chứng từ vì lý do riêng nhưng cần hỗ trợ thêm thì CS làm gì?
**Trả lời:** CS chuyển Risk đánh giá.

### Q93. Low balance được hiểu như thế nào?
**Trả lời:** Low balance là tổng số dư có thể chắc chắn tính được nhỏ hơn hoặc bằng 200.000 VND.

### Q94. High balance được hiểu như thế nào?
**Trả lời:** High balance là tổng số dư có thể chắc chắn tính được lớn hơn 200.000 VND hoặc có ít nhất một source of fund không tính được.

### Q95. Nếu xuất hiện balance mới chưa tính được thì xử lý thế nào?
**Trả lời:** Nếu xuất hiện balance mới thì xem là unknown và cần Risk review.

### Q96. Source of fund nào có thể chắc chắn tính được?
**Trả lời:** Các nguồn có thể chắc chắn tính được gồm số dư ví, số dư sinh lời, ví trả sau theo điều kiện cập nhật, và tài khoản tiền gửi tiết kiệm có kỳ hạn.

### Q97. Khi xác minh nguồn gốc số dư qua call, CS cần hỏi gì?
**Trả lời:** CS cần hỏi 2 trong 5 thông tin gồm nhận từ ai hoặc chương trình nào, thời gian nhận, nội dung nhận, ngân hàng nạp hoặc nhận từ ngân hàng nào, và số tiền nhận.

### Q98. Khi xác minh lịch sử giao dịch qua call, CS cần hỏi gì?
**Trả lời:** CS cần hỏi 1 trong 5 thông tin gồm loại dịch vụ thường dùng, nguồn tiền thanh toán, số tiền thường thanh toán hoặc giao dịch gần nhất, thời gian giao dịch, mã giao dịch hoặc mã đơn hàng.

### Q99. Map bank hiện có những luồng nào?
**Trả lời:** Map bank hiện có map by card/bank account và map by FD.

---

## 8. Fund Recovery / Balance Liquidation

### Q100. Với chuyển tiền nhầm, khi nào có thể hỗ trợ đảo chiều?
**Trả lời:** Có thể hỗ trợ đảo chiều nếu chủ ví nhận nhầm đồng ý, không biết gì về giao dịch, hoặc ví nhận nhầm inactive trên 12 tháng và non-KYC, đồng thời chủ ví raise ticket đã KYC và cung cấp xác minh chính chủ cùng sao kê giao dịch nạp nhầm và một giao dịch từng thực hiện trên ví.

### Q101. Nếu chủ ví raise ticket chuyển tiền nhầm nhưng chưa KYC thì xử lý thế nào?
**Trả lời:** Không hỗ trợ ngay và yêu cầu khách hàng KYC rồi raise lại ticket.

### Q102. Nếu chủ ví nhận nhầm không đồng ý hoặc không liên lạc được thì có hỗ trợ thu hồi tiền không?
**Trả lời:** Không hỗ trợ.

### Q103. Với nạp tiền nhầm từ ngân hàng thì xử lý thế nào?
**Trả lời:** Case nạp tiền nhầm từ ngân hàng cần consult LG/CPL.

### Q104. Khi khách hàng không thể tự withdraw thì có thể thanh lý số dư không?
**Trả lời:** Có thể thanh lý số dư nếu khách hàng không thể tự withdraw do bị khóa ví, không thể sinh trắc học, không thể tap NFC hoặc là người nước ngoài không thể KYC, nhưng phải xác minh chính chủ và cung cấp nguồn nhận tiền cần thanh lý.

### Q105. Thanh lý số dư cho chủ ví đã qua đời với nguồn tiền là số dư ví cần chứng từ gì?
**Trả lời:** Cần giấy chứng tử của chủ tài khoản, GTTT của chủ tài khoản, GTTT của người hưởng di sản, giấy tờ chứng minh quan hệ và văn bản thừa kế di sản.

### Q106. Thanh lý số dư sinh lời cho chủ ví đã qua đời xử lý thế nào?
**Trả lời:** CS chuyển chứng từ cho INFINA xử lý hỗ trợ khách hàng theo quy trình của INFINA.

---

## 9. Change Phone

### Q107. Change phone cần điều kiện gì?
**Trả lời:** Change phone cần xác minh chính chủ trước khi hỗ trợ.

### Q108. Nếu khách hàng đổi số điện thoại hơn 2 lần trong 6 tháng thì xử lý thế nào?
**Trả lời:** Không hỗ trợ.

---

## 10. Account Unlock

### Q109. Nếu tài khoản bị khóa F1 do nhận tiền từ tài khoản gian lận và có tag ATO/Card Fraud victim confirmed thì có mở khóa không?
**Trả lời:** Không hỗ trợ mở khóa và hướng xử lý tiếp theo là thanh lý số dư.

### Q110. Nếu trans báo fraud nhưng tag là Friendly Fraud, Scamming hoặc Uncertain thì xử lý thế nào?
**Trả lời:** Có thể xử lý theo hướng xác minh chính chủ.

### Q111. Nếu tài khoản bị khóa do chủ thẻ khiếu nại ngân hàng và chủ thẻ chưa hủy khiếu nại thì có mở khóa không?
**Trả lời:** Không hỗ trợ mở khóa.

### Q112. Nếu chủ thẻ đã hủy khiếu nại ngân hàng thì cần gì để mở khóa?
**Trả lời:** Cần xác minh chính chủ, xác nhận mở khóa từ ngân hàng hoặc chủ thẻ qua ngân hàng/email, và sao kê giao dịch nếu chưa cung cấp ở bước xác minh.

### Q113. Nếu tài khoản bị khóa do spam số dư tài khoản ngân hàng thì cần gì để mở khóa?
**Trả lời:** Cần xác minh chính chủ, giấy xác nhận chủ thẻ hoặc tài khoản ngân hàng, và sao kê giao dịch có mộc ngân hàng từ thẻ/TKNH bị fail nhiều lần.

### Q114. Nếu tài khoản bị khóa theo yêu cầu của chủ tài khoản nhưng không có dấu hiệu fraud thì xử lý thế nào?
**Trả lời:** Có thể xử lý sau khi xác minh chính chủ.

### Q115. Nếu tài khoản bị khóa bởi bộ phận khác thì điều kiện mở khóa là gì?
**Trả lời:** Cần nguyên nhân khóa đã được xử lý hoặc bộ phận yêu cầu khóa chấp nhận hỗ trợ mở khóa, đồng thời khách hàng phải xác minh chính chủ.

---

## 11. Account Closure / SIM Reuse / PIN

### Q116. Đóng tài khoản cần điều kiện gì?
**Trả lời:** Đóng tài khoản cần xác minh chính chủ và thực hiện theo quy trình đóng tài khoản.

### Q117. Tái sử dụng SIM áp dụng cho trường hợp nào?
**Trả lời:** Tái sử dụng SIM áp dụng khi chủ SIM mua lại SIM đã có tài khoản Zalopay hoặc chủ SIM bị card fraud và cần dùng lại số điện thoại đã đăng ký Zalopay.

### Q118. Điều kiện để hỗ trợ tái sử dụng SIM là gì?
**Trả lời:** Tài khoản không được bị khóa bởi lý do liên quan đến gian lận và khách hàng cần cung cấp thông tin thuê bao, GTTT khớp thuê bao, nguồn gốc số dư nếu có giao dịch, và thẻ/TKNH liên kết nếu có map bank/card trong quá trình tranh chấp.

### Q119. Sau khi tái sử dụng SIM, UID cũ được xử lý thế nào?
**Trả lời:** SĐT được gỡ khỏi UID cũ, UID cũ quay về trạng thái K0 không có số điện thoại và vẫn có thể tiếp tục sử dụng nếu đăng nhập được qua ZPI hoặc liên hệ CS để xác minh chính chủ.

### Q120. Reset PIN cần điều kiện gì?
**Trả lời:** Reset PIN cần xác minh chính chủ.

### Q121. Reset Profile có được hỗ trợ không?
**Trả lời:** Không hỗ trợ vì Reset Profile đã deprecated.

---

## 12. Trust Card CYBS / BRR

### Q122. Trust thẻ CYBS cho giao dịch trên ví Zalopay cần chứng từ gì?
**Trả lời:** Cần xác minh chính chủ và hình ảnh thẻ ngân hàng 6 số đầu - 4 số cuối đang giao dịch fail, cần được trust.

### Q123. Trust thẻ CYBS cho giao dịch Gateway cần chứng từ gì?
**Trả lời:** Cần hình ảnh hai mặt GTTT, ảnh selfie cầm GTTT và hình ảnh thẻ ngân hàng 6 số đầu - 4 số cuối đang giao dịch fail.

### Q124. Sau khi trust thẻ CYBS, CS cần thông báo gì cho khách hàng?
**Trả lời:** CS cần thông báo khách hàng sẽ chịu trách nhiệm cho các rủi ro phát sinh trên tài khoản về sau.

### Q125. Hủy xác thực tích điểm ngân hàng BRR khi chủ ví là chủ thẻ cần gì?
**Trả lời:** Cần xác minh chính chủ và xác nhận khách hàng đồng ý hủy mọi quyền lợi tích điểm tại ví cũ.

### Q126. Hủy xác thực tích điểm ngân hàng BRR khi chủ ví khác chủ thẻ cần gì?
**Trả lời:** Cần xác minh chủ thẻ bằng hình ảnh thẻ ngân hàng 6 số đầu - 4 số cuối và GTTT khớp hình ảnh thẻ ngân hàng, đồng thời xác nhận khách hàng đồng ý hủy mọi quyền lợi tích điểm tại ví cũ.

---

## 13. Practical Decision Scenarios

### Q127. PM hỏi thay đổi text hiển thị trên màn hình lỗi, không ảnh hưởng tiền, giao dịch, bảo mật, tích hợp hoặc promotion thì có cần Risk Review không?
**Trả lời:** Không cần Risk Review nếu thay đổi thật sự chỉ là text/UI và không ảnh hưởng bất kỳ điều kiện kiểm soát nào.

### Q128. Dev muốn đổi payload gửi sang Risk Engine thì có cần Risk Review không?
**Trả lời:** Có, bắt buộc cần Risk Review.

### Q129. Product muốn thay đổi hạn mức nạp tiền bằng thẻ quốc tế thì có cần Risk Review không?
**Trả lời:** Có, bắt buộc cần Risk Review.

### Q130. CS nhận case khách hàng nói giao dịch không phải họ thực hiện thì bước đầu tiên nên làm gì?
**Trả lời:** CS cần dùng Investigation Tool để kiểm tra giao dịch trước khi chuyển Risk.

### Q131. CS nhận yêu cầu mở khóa ví nhưng ví bị khóa bởi team khác thì xử lý thế nào?
**Trả lời:** CS cần xin approval từ team đã khóa ví trước rồi mới hỗ trợ khách hàng.

### Q132. Khách hàng yêu cầu đổi số điện thoại lần thứ ba trong 6 tháng thì xử lý thế nào?
**Trả lời:** Không hỗ trợ.

### Q133. Khách hàng bị lỗi do BIN thẻ nằm trong blacklist thì CS nên tư vấn gì?
**Trả lời:** CS nên tư vấn khách hàng thanh toán bằng nguồn tiền khác.

### Q134. Khách hàng bị lỗi do vượt hạn mức 24 giờ thì CS nên tư vấn gì?
**Trả lời:** CS nên hướng dẫn khách hàng thử lại sau 24 giờ kể từ giao dịch thất bại hoặc thành công cuối cùng tùy rule cụ thể.

### Q135. Khách hàng bị chặn do thiết bị lạ nhưng chưa KYC thì CS làm gì?
**Trả lời:** CS hướng dẫn khách hàng KYC tài khoản.

### Q136. Khách hàng bị chặn do thiết bị lạ nhưng đã KYC thì CS làm gì?
**Trả lời:** CS add khách hàng vào danh sách để Risk check theo guideline tương ứng.

### Q137. Khách hàng muốn thanh lý số dư vì không thể sinh trắc học thì xử lý thế nào?
**Trả lời:** Có thể xử lý thanh lý số dư sau khi xác minh chính chủ và yêu cầu khách hàng cung cấp nguồn nhận tiền cần thanh lý.

### Q138. Khách hàng cung cấp chứng từ có dấu hiệu photoshop thì xử lý thế nào?
**Trả lời:** CS không nên hỗ trợ theo chứng từ đó và cần chuyển Risk đánh giá hoặc từ chối tùy trường hợp.

### Q139. Khách hàng dùng VNeID thay CCCD thì có chấp nhận không?
**Trả lời:** Có thể chấp nhận nếu ảnh chụp từ giao diện gốc VNeID chính chủ, hiển thị đầy đủ thông tin định danh, còn hiệu lực và khớp với hồ sơ Zalopay.

### Q140. Khách hàng dùng ảnh scan hộ chiếu để xác minh thì có hợp lệ không?
**Trả lời:** Không hợp lệ nếu là bản scan, bản in hoặc ảnh cũ không xác minh được nguồn gốc.

### Q141. Khi nguồn gốc số dư không liên quan đến giao dịch Zalopay thì có hợp lệ không?
**Trả lời:** Không hợp lệ.

### Q142. Nếu khách hàng có liên kết thẻ nhưng không cung cấp được nguồn gốc số dư thì CS nên yêu cầu gì?
**Trả lời:** CS yêu cầu khách hàng cung cấp hình ảnh thẻ ngân hàng hoặc tài khoản ngân hàng liên kết với ví theo quy định.

### Q143. Nếu khách hàng không liên kết thẻ và không cung cấp được nguồn gốc số dư thì xử lý thế nào?
**Trả lời:** CS gửi Risk đánh giá.

### Q144. Nếu case không nằm trong bất kỳ trường hợp guideline nào thì CS xử lý thế nào?
**Trả lời:** CS gửi Risk đánh giá.

### Q145. RiskMind nên ưu tiên trả lời theo guideline hay chuyển Risk?
**Trả lời:** RiskMind nên ưu tiên trả lời theo guideline nếu case khớp đầy đủ điều kiện, và chỉ hướng dẫn chuyển Risk khi case ngoài guideline, thiếu kết quả từ tool, chứng từ bất thường hoặc cần đánh giá ngoại lệ.

---

## SLA Questions

### SLA-1. SLA xử lý các yêu cầu vận hành cần Risk hỗ trợ là bao lâu?
**Trả lời:** SLA xử lý các yêu cầu vận hành cần Risk hỗ trợ là trong vòng 5 ngày làm việc. Với các trường hợp urgent như khách hàng đến trực tiếp công ty, khách hàng đã trình báo cơ quan công an hoặc case cần phối hợp xử lý gấp với bên liên quan, Risk sẽ ưu tiên xử lý trong khoảng 3-5 ngày làm việc tùy mức độ khẩn cấp và độ đầy đủ của thông tin đầu vào.

### SLA-2. SLA Risk Review cho các thay đổi liên quan đến product, feature hoặc process là bao lâu?
**Trả lời:** SLA Risk Review cho các thay đổi liên quan đến product, feature hoặc process là 2 tuần làm việc.

### SLA-3. Khi nào áp dụng SLA vận hành và khi nào áp dụng SLA Risk Review?
**Trả lời:** SLA vận hành được áp dụng khi yêu cầu là một case cụ thể đã phát sinh liên quan đến khách hàng, tài khoản hoặc giao dịch và cần Risk hỗ trợ xử lý. SLA Risk Review được áp dụng khi yêu cầu là một thay đổi mang tính thiết kế, thay đổi sản phẩm, tính năng, quy trình, rule, flow hoặc integration trước khi triển khai.
-e 
### Q146. High-risk MCC là gì?
**Trả lời:** High-risk MCC (Merchant Category Code) là một mã bốn chữ số được ngân hàng và các nhà cung cấp dịch vụ thanh toán sử dụng để phân loại các doanh nghiệp dựa trên loại hình hoạt động của họ. Các mã MCC này được sử dụng để đánh giá mức độ rủi ro thanh toán, với các mã MCC cao rủi ro thường liên quan đến các ngành có nguy cơ cao hơn về việc phát sinh thanh toán không thành công, gian lận và tranh chấp. Các mã MCC cao rủi ro thường dẫn đến các quy trình thanh toán phức tạp hơn, phí dịch vụ cao hơn và hạn chế hơn trong việc kết nối với các nhà cung cấp dịch vụ thanh toán. Các ngành có nguy cơ cao hơn về thanh toán không thành công, như giải trí, phụ kiện trang sức, và giáo dục tài chính, thường bị phân loại là cao rủi ro.
