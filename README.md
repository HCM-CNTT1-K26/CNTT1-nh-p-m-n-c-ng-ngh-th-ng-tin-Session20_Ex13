# CNTT1-nh-p-m-n-c-ng-ngh-th-ng-tin-Session20_Ex13
## Phần 1 – Googling đúng cách

**1. Vì sao câu hỏi "văn nói" cho kết quả kém:**

* Chứa nhiều từ thừa, cảm tính ("tại sao em", "thầy ơi").
* Google cần từ khóa kỹ thuật cốt lõi; câu dài dòng làm loãng thông tin, trả về bài viết chung chung thay vì đúng lỗi hệ thống.

**2. Bóc tách lỗi:**

| Thành phần | Nội dung bóc tách |
| --- | --- |
| **Tên phần mềm / Hệ điều hành** | Node.js / npm trên Windows 11 |
| **Mã lỗi nguyên văn** | 'npm' is not recognized as an internal or external command, operable program or batch file. |
| **Thao tác đang làm** | Mở Terminal (VS Code) gõ lệnh npm -v |

**3. Ba câu truy vấn Google tối ưu:**

* **Toán tử site::** site:stackoverflow.com "is not recognized as an internal or external command" npm
* **Toán tử "":** "npm is not recognized as an internal or external command" windows 11
* **Toán tử -:** npm is not recognized as an internal or external command windows -xp -vista

---

## Phần 2 – Thẩm định StackOverflow

**1. So sánh Câu trả lời A và B:**

| Tiêu chí | Câu trả lời A | Câu trả lời B |
| --- | --- | --- |
| **Vote & Tích xanh** | +186 upvotes, có Tích xanh (Accepted Answer) | +2 upvotes, Không có tích xanh |
| **Thời gian đăng bài** | 2 năm trước | 9 năm trước |
| **Tags khớp hệ điều hành/phần mềm** | [node.js] [windows] [npm] | [node.js] [windows-xp] |

**2. Lựa chọn và bẫy nguy hiểm:**

* **Chọn:** Câu trả lời A.
* **Bẫy Câu trả lời B:** Đề xuất cài lại driver mạng cho Windows XP trong khi máy đang dùng Windows 11. Làm theo sẽ không sửa được lỗi mà còn phá hỏng cấu hình mạng hiện tại.

**3. Quy tắc 30 Giây Đọc lướt:**

1. Nhìn ngay vào Tích xanh và số lượng Upvotes.
2. Đọc lướt nhanh khung code giải pháp xem có khớp lỗi không.
3. Kiểm tra tags và thời gian có phù hợp với hệ điều hành hiện tại không.

---

## Phần 3 – Hỏi AI đúng cách và nhận diện rủi ro

**1. Prompt 3 Thành phần:**

text

[Context]

Tôi vừa cài Node.js trên laptop Windows 11. Mở Terminal trong VS Code gõ lệnh kiểm tra thì báo lỗi không nhận lệnh. Đã thử thêm đường dẫn vào biến môi trường PATH nhưng vẫn bị lỗi.



[Raw Error]

'npm' is not recognized as an internal or external command, operable program or batch file.


[Instruction]

Giải thích vì sao thêm PATH vẫn lỗi và hướng dẫn các bước kiểm tra thay thế chi tiết trên Windows 11.



**2. Đánh giá câu trả lời của AI ở mục 3e:**

* **An toàn hay không:** **Tuyệt đối KHÔNG AN TOÀN**.
* **Vì sao:** Lệnh del /f /s /q C:\Windows\System32\* sẽ xóa sạch file hệ thống quan trọng, làm sập hoàn toàn máy tính ngay lập tức. Đây là một lỗi ảo giác AI nguy hiểm.

**3. Cách phản hồi lại AI:**

* Cảnh báo ngay: *"Lệnh này sẽ xóa sạch file hệ thống và làm hỏng máy. Lỗi này liên quan đến PATH của Node.js, hãy đưa ra giải pháp an toàn khác."*

---

## Phần 4 – Viết Bug Report chuẩn

**1. Tin nhắn Kém:**

> *"Thầy ơi máy em bị lỗi npm rồi, không chạy được lệnh, sửa sao ạ?"*

**2. Tin nhắn Chuẩn (Bug Reporting Framework):**

| Mảnh ghép | Nội dung trong tin nhắn của bạn |
| --- | --- |
| **Context** | Cài mới Node.js trên Windows 11, dùng VS Code Terminal, đã thêm PATH theo StackOverflow nhưng vẫn lỗi. |
| **Expected** | Gõ npm -v phải hiển thị số phiên bản npm. |
| **Actual** | Báo lỗi: 'npm' is not recognized as an internal or external command, operable program or batch file. |
| **Log & Screenshot** | [Đính kèm ảnh chụp màn hình Terminal kèm lỗi và cấu hình PATH] |

**3. Phím tắt và Lưu ý bảo mật:**

* **Phím tắt chụp màn hình:** Nhấn Windows + Shift + S.
* **Lưu ý bảo mật:** Che mờ các thông tin nhạy cảm (tên đăng nhập, email, đường dẫn chứa thông tin cá nhân) trước khi gửi ảnh lên nhóm chung.
