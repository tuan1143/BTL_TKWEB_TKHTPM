# 📋 Ghi chú Phát hành (Release Notes) – CampVibe Glamping

## Phiên bản `v1.0.0` — Bản Bàn Giao Chính Thức (Bài tập lớn A3)

* **Ngày phát hành:** 24/11/2026  
* **Trạng thái:** Đã kiểm thử & Triển khai ổn định trên GitHub Pages  
* **URL Triển khai:** [https://tuan1143.github.io/BTL_TKWEB_TKHTPM/](https://tuan1143.github.io/BTL_TKWEB_TKHTPM/)  

---

### ✨ Tính năng Mới (Features)
* **Hệ thống 5 trang hoàn chỉnh:** Xây dựng đầy đủ luồng trải nghiệm người dùng từ Trang chủ (`index.html`), Danh sách (`campsites.html`), Chi tiết (`detail.html`), Cẩm nang (`blog.html`) đến Đặt lịch & Liên hệ (`contact.html`).
* **Điều hướng Responsive:** Thanh Header cố định tích hợp Menu Hamburger thuần CSS cho màn hình dưới `768px`.
* **Bộ lọc & Thư viện ảnh không dùng JS:** Lọc khu cắm trại theo 3 khu vực (Đà Lạt, Ba Vì, Hồ Cốc) và chuyển đổi 4 góc ảnh chi tiết lều mượt mà.
* **Kiểm tra dữ liệu Form trực quan:** Cảnh báo viền đỏ/xanh tức thì khi nhập họ tên, số điện thoại và email tại trang đặt lịch.

### 🐛 Sửa lỗi & Tối ưu (Bug Fixes & Improvements)
* **Sửa lỗi đường dẫn tài nguyên khi deploy:** Chuyển đổi toàn bộ đường dẫn tệp CSS từ đường dẫn tuyệt đối (`/assets/...`) sang đường dẫn tương đối (`assets/...`) để tương thích với cấu trúc thư mục con của GitHub Pages.
* **Tối ưu hiển thị trên màn hình hẹp (`375px`):** Điều chỉnh chiều cao khung ảnh chính tại `detail.html` từ `480px` xuống `280px` trên thiết bị di động và chuyển danh sách tiện nghi từ 2 cột sang 1 cột để tránh tràn chữ.

### ⚠️ Các giới hạn đã biết (Known Limitations)
* Các bộ lọc tiện ích dạng checkbox ở cột bên trái trang `campsites.html` hiện đóng vai trò minh họa giao diện tĩnh (chỉ bộ lọc theo khu vực địa điểm hoạt động tương tác).
* Nút gửi biểu mẫu đặt lịch hiển thị hộp thoại xác nhận giả lập qua `:target`, chưa lưu dữ liệu xuống máy chủ.