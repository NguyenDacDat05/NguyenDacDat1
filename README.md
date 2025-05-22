![image](https://github.com/user-attachments/assets/a3fa93c4-bba6-43cb-b240-7743f0a84639)
1. Chức năng của ứng dụng
Ứng dụng web cung cấp công cụ mã hóa và giải mã file sử dụng thuật toán AES (Advanced Encryption Standard) với các chức năng chính:

Tải lên file từ thiết bị người dùng.

Nhập khóa AES có độ dài tùy ý (tối thiểu 8 ký tự).

Chọn thao tác: Mã hóa hoặc Giải mã.

Tải về file kết quả sau khi xử lý.

Ứng dụng hướng đến bảo mật đơn giản, dễ sử dụng cho người dùng không chuyên.

2. Cách thức hoạt động
Quy trình hoạt động gồm các bước sau:

Bước 1: Người dùng thao tác
Truy cập trang web và giao diện chính.

Chọn file từ máy tính (dạng bất kỳ: PDF, TXT, PNG, DOCX,...).

Nhập khóa AES tùy chọn (ít nhất 8 ký tự).

Chọn chế độ Mã hóa hoặc Giải mã.

Nhấn nút "Xử lý tệp" để thực hiện hành động.

Bước 2: Backend xử lý
Hệ thống đọc file được tải lên.

Tùy vào chế độ:

Mã hóa: Nội dung file được mã hóa bằng thuật toán AES với khóa người dùng nhập.

Giải mã: File đầu vào được giải mã bằng khóa AES (nếu đúng khóa).

Hệ thống tạo một file kết quả mới và trả lại cho người dùng tải về.

Bước 3: Trả kết quả
File đã mã hóa/giải mã được gửi lại dưới dạng file tải về.

Nếu sai khóa hoặc định dạng không hợp lệ, hệ thống thông báo lỗi.
Bước 4: Công nghệ sử dụng
Frontend (Giao diện người dùng):
HTML5: Tạo cấu trúc trang web.

CSS3 (thuần): Tạo hiệu ứng màu sắc, bố cục, responsive, giao diện hiện đại tông tím.

Google Fonts: Sử dụng font chữ đẹp (Montserrat, Inter) tăng tính thẩm mỹ.

Font Awesome 6: Thêm icon đẹp mắt (khiên bảo mật, ổ khóa...).

JavaScript (tùy chọn): Có thể thêm để xử lý preview, validate nâng cao hoặc cải thiện UX.

Backend (Xử lý mã hóa/giải mã file):
Python:

Flask hoặc FastAPI để xây dựng RESTful Web Server.

pycryptodome hoặc cryptography để mã hóa/giải mã AES (128-bit, CBC mode, hoặc ECB).

Werkzeug (nếu dùng Flask): Xử lý upload file an toàn.

File I/O: Đọc và ghi nội dung file từ phía server.

Mã hóa AES: Chuyển nội dung file thành dữ liệu nhị phân, mã hóa với khóa, sau đó lưu lại thành file mã hóa.

4. Giao diện của Web
Giao diện được thiết kế hiện đại, nổi bật với tông màu tím ánh sáng neon:

Giao diện chính nằm gọn trong một khung giữa màn hình, bo tròn, bóng mờ hiện đại.

Tiêu đề lớn và nổi bật: "Mã hóa AES" với biểu tượng bảo mật.

Form người dùng dễ sử dụng:

Upload file.

Nhập khóa AES.

Radio button chọn mã hóa/giải mã.

Nút xử lý có hiệu ứng động gradient tím rực rỡ.

Hiệu ứng giao diện:

Hover nổi sáng, button chuyển màu tím gradient.

Input focus tạo ánh sáng tím.

Responsive tốt trên điện thoại và máy tính.
