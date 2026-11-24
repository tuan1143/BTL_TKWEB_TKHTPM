# 🤖 Nhật ký Sử dụng Công cụ AI (AI Usage Log)

* **Học phần:** FIT4014 – Thiết kế web và triển khai hệ thống phần mềm  
* **Bài tập:** Bài tập lớn A3 – Website Đặt Lịch Cắm Trại Cao Cấp (CampVibe Glamping)  
* **Sinh viên thực hiện:** [Điền Họ và Tên] – Mã SV: `1771020716`  
* **Công cụ AI đã sử dụng:** Google Gemini  

---

## 1. Nguyên tắc Tuân thủ & Trách nhiệm Học thuật

* Công cụ AI chỉ được sử dụng với vai trò **trợ lý kỹ thuật** để gợi ý ý tưởng cấu trúc, tham khảo cú pháp CSS3 nâng cao và rà soát tối ưu mã nguồn.
* Sinh viên **không sao chép thụ động**: Toàn bộ cấu trúc tệp, mã HTML/CSS đều được tự tay lắp ghép, biên tập nội dung tiếng Việt, thay thế hình ảnh, kiểm thử thực tế trên nhiều kích thước màn hình và tự thực hiện quy trình quản lý phiên bản trên Git/GitHub.

---

## 2. Chi tiết Các Phiên Làm việc Hỗ trợ

| Phiên | Mục đích hỗ trợ | Nội dung AI gợi ý | Phần việc Sinh viên tự thực hiện & Hiệu chỉnh |
| :--- | :--- | :--- | :--- |
| **Phiên 1** | Lên ý tưởng đề tài & cấu trúc thư mục | Đề xuất chủ đề Website Glamping 5 trang và cách tổ chức thư mục chuẩn (`index.html`, `campsites.html`, `detail.html`, `blog.html`, `contact.html`, `assets/css/style.css`). | Chốt tên thương hiệu **CampVibe**, xây dựng yêu cầu R1–R5 và khởi tạo kho lưu trữ Git trên máy cá nhân. |
| **Phiên 2** | Thiết kế Hệ thống màu & Trang chủ | Gợi ý khai báo biến `:root` và bố cục Bento Grid bằng CSS Grid cho phần điểm đến nổi bật. | Tự điều chỉnh mã màu xanh rêu/cam đất, chọn lọc ảnh từ Unsplash, chỉnh sửa kích thước chữ và kiểm thử Responsive. |
| **Phiên 3** | Kỹ thuật tương tác thuần CSS | Hướng dẫn dùng `input[type="radio"]` + `:checked` làm bộ lọc địa điểm và thư viện chuyển đổi ảnh không cần JS. | Tích hợp vào `campsites.html` và `detail.html`, căn chỉnh lại hiệu ứng chuyển cảnh (`transition`) và khoảng cách lưới. |
| **Phiên 4** | Kiểm tra hợp lệ Form & Modal | Gợi ý kết hợp `:not(:placeholder-shown):invalid` để báo lỗi nhập liệu Form và `:target` làm hộp thoại xác nhận. | Viết biểu thức `pattern` kiểm tra số điện thoại Việt Nam (10 số bắt đầu bằng 0), bổ sung thông báo lỗi tiếng Việt. |