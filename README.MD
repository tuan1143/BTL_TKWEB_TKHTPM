# 🏕️ CampVibe - Website Đặt Lịch & Trải Nghiệm Cắm Trại Cao Cấp (Glamping)

> **Bài tập lớn A3** — Học phần **FIT4014: Thiết kế web và triển khai hệ thống phần mềm**  
> **Trường Đại học Đại Nam** | Khoa Công nghệ Thông tin

---

## 🔗 Liên kết Bàn giao & Triển khai

* **🌐 Website trực tuyến (Live Demo):** [https://tuan1143.github.io/BTL_TKWEB_TKHTPM/](https://tuan1143.github.io/BTL_TKWEB_TKHTPM/)
* **📂 Kho mã nguồn (Repository):** [https://github.com/tuan1143/BTL_TKWEB_TKHTPM](https://github.com/tuan1143/BTL_TKWEB_TKHTPM)
* **🏷️ Phiên bản phát hành (Release Tag):** `v1.0.0`
* **📝 Nhật ký sử dụng AI:** [Xem chi tiết tại AI_LOG.md](./AI_LOG.md)
* **📋 Ghi chú phiên bản:** [Xem chi tiết tại RELEASE_NOTES.md](./RELEASE_NOTES.md)

---

## 👤 Thông tin Sinh viên Thực hiện

| Hạng mục | Nội dung |
| :--- | :--- |
| **Sinh viên thực hiện** | [Lỗ Văn Tuấn] |
| **Mã sinh viên** | `1771020716` |
| **Lớp / Ngành** | [20-02] – Công nghệ Thông tin |
| **Giảng viên hướng dẫn** | ThS. Lê Thái Bảo |
| **Học kỳ / Năm học** | Học kỳ 1 – Năm học 2026–2027 |

---

## 🎯 1. Tổng quan & Mục tiêu Dự án

**CampVibe** (kết hợp giữa *Camp* – cắm trại và *Vibe* – không khí, cảm xúc) là website giới thiệu và đặt lịch nghỉ dưỡng cắm trại cao cấp (Glamping) tại các điểm đến nổi tiếng của Việt Nam như Đà Lạt, Ba Vì và Hồ Cốc.

### Mục tiêu thiết kế & Kỹ thuật:
1. **Chuẩn Semantic HTML5:** Sử dụng hệ thống thẻ ngữ nghĩa rõ ràng (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`) giúp tối ưu cấu trúc tài liệu và khả năng truy cập (Accessibility).
2. **100% CSS3 Thuần (Zero JavaScript):** Toàn bộ hiệu ứng tương tác (Menu điện thoại, Bộ lọc sản phẩm theo khu vực, Thư viện chuyển đổi ảnh, Modal đọc bài viết, Kiểm tra hợp lệ Form) đều được xây dựng bằng kỹ thuật CSS hiện đại mà không phụ thuộc thư viện bên ngoài.
3. **Responsive Đa thiết bị:** Tương thích mượt mà trên mọi độ phân giải màn hình từ điện thoại di động (`375px`), máy tính bảng (`768px`) đến máy tính để bàn (`1440px`).

---

## ✨ 2. Các Chức năng & Kỹ thuật CSS Nổi bật

| Trang / Thành phần | Tệp nguồn | Kỹ thuật HTML5 / CSS3 áp dụng |
| :--- | :--- | :--- |
| **Thanh điều hướng (Header)** | `index.html` & `style.css` | `position: sticky`, `backdrop-filter: blur()`, kỹ thuật **Checkbox Hack** (`input[type="checkbox"]:checked`) tạo Menu Hamburger trên Mobile. |
| **Trang chủ (Home)** | `index.html` | **CSS Grid Bento Layout** (`grid-column: span 2`, `grid-row: span 2`), hiệu ứng phóng to ảnh mượt mà (`transform: scale()`), bố cục **Flexbox** cho khối tiện ích. |
| **Danh sách Khu trại** | `campsites.html` | **Bộ lọc địa điểm thuần CSS** kết hợp `input[type="radio"]:checked` và bộ chọn phủ định `:not([data-category="..."])` để ẩn/hiện thẻ trại tức thì. |
| **Chi tiết Khu trại** | `detail.html` | **Thư viện ảnh tương tác (Gallery Slider)** bằng `radio` + `label`, bảng giá kẻ sọc (`:nth-child(even)`), khung đặt phòng trượt cố định (`position: sticky`). |
| **Cẩm nang Du lịch** | `blog.html` | Bố cục tạp chí (Editorial Layout), trích dẫn `<blockquote>`, phân trang UI và cửa sổ đọc nhanh bài viết bằng pseudo-class `:target`. |
| **Liên hệ & Đặt lịch** | `contact.html` | **HTML5 Form Validation** (`required`, `pattern`, `minlength`) kết hợp `:not(:placeholder-shown):invalid` / `:valid` báo viền đỏ/xanh trực quan và hộp thoại xác nhận `:target`. |

---

## 🎨 3. Hệ thống Thiết kế (Design System)

Toàn bộ màu sắc, khoảng cách và bo góc được quản lý tập trung thông qua biến CSS (`:root`) tại tệp `assets/css/style.css`:

* **Màu chủ đạo (`--primary-color`):** `#2D5A27` (Xanh rêu rừng thông – đại diện cho thiên nhiên).
* **Màu nhấn (`--accent-color`):** `#D97736` (Cam đất lửa trại – tạo điểm nhấn cho nút bấm CTA).
* **Màu nền phụ (`--bg-light`):** `#F7F6F2` (Kem ấm tự nhiên – giúp dịu mắt khi đọc nội dung dài).
* **Kiểu chữ (Typography):** `Plus Jakarta Sans` (Google Fonts) với các trọng số `400`, `500`, `600`, `700`.

---

## 📁 4. Cấu trúc Thư mục Mã nguồn

```text
BTL_TKWEB_TKHTPM/
├── index.html              # Trang chủ
├── campsites.html          # Trang danh sách & Bộ lọc khu cắm trại
├── detail.html             # Trang chi tiết lều, thư viện ảnh & bảng giá
├── blog.html               # Trang tạp chí cẩm nang kinh nghiệm
├── contact.html            # Trang liên hệ, bản đồ & phiếu đặt lịch
├── assets/
│   └── css/
│       └── style.css       # Tệp định dạng CSS chung cho toàn bộ website
├── README.md               # Tài liệu tổng quan & hướng dẫn dự án
├── AI_LOG.md               # Nhật ký khai báo sử dụng công cụ AI
└── RELEASE_NOTES.md        # Ghi chú phiên bản phát hành
<<<<<<< HEAD

## 🚀 5. Hướng dẫn Cài đặt & Chạy Cục bộ

Dự án là website tĩnh thuần **HTML5/CSS3** nên không yêu cầu cài đặt môi trường máy chủ (Server) hay cơ sở dữ liệu phức tạp. Bạn có thể trải nghiệm theo một trong ba cách sau:

### Cách 1: Xem trực tuyến qua GitHub Pages (Khuyên dùng)
Truy cập trực tiếp đường dẫn đã triển khai trên mọi trình duyệt (máy tính hoặc điện thoại):
* **URL:** [https://tuan1143.github.io/BTL_TKWEB_TKHTPM/](https://tuan1143.github.io/BTL_TKWEB_TKHTPM/)

### Cách 2: Tải mã nguồn về máy và mở bằng trình duyệt
1. Mở **Terminal** (hoặc Git Bash / PowerShell) và chạy lệnh sao chép kho lưu trữ:
   ```bash
   git clone [https://github.com/tuan1143/BTL_TKWEB_TKHTPM.git](https://github.com/tuan1143/BTL_TKWEB_TKHTPM.git)

## ⚠️ 6. Giới hạn Hiện tại & Hướng Phát triển

### 6.1. Các giới hạn hiện tại (Current Limitations)
Do phạm vi và ràng buộc của Bài tập lớn A3 chỉ sử dụng **HTML5 và CSS3 thuần (Zero JavaScript)**, hệ thống hiện tại tồn tại một số giới hạn kỹ thuật sau:
* **Dữ liệu tĩnh (Static Data):** Toàn bộ thông tin về khu cắm trại, bảng giá và bài viết cẩm nang đang được lưu trữ cứng (hard-coded) trực tiếp trong các tệp `.html`, chưa có cơ chế tự động hóa render từ tệp dữ liệu JSON hoặc cơ sở dữ liệu.
* **Bộ lọc chưa kết hợp đa điều kiện:** Tại trang danh sách (`campsites.html`), bộ lọc khu vực địa lý (Đà Lạt, Ba Vì, Hồ Cốc) hoạt động tương tác thực tế, tuy nhiên các tùy chọn tiện ích dạng checkbox ở cột bên trái hiện chỉ đóng vai trò minh họa giao diện.
* **Tính toán giá tự động:** Tại khung đặt phòng trang chi tiết (`detail.html`), bảng tổng tạm tính hiển thị giá trị mẫu cho 1 đêm tiêu chuẩn, chưa tự động nhân tổng tiền khi người dùng thay đổi số đêm lưu trú, số lượng khách hoặc chọn dịch vụ bổ sung.
* **Lưu trữ & Xử lý biểu mẫu:** Biểu mẫu đăng ký đặt lịch (`contact.html`) đã kiểm tra hợp lệ dữ liệu đầu vào (`:valid` / `:invalid`) và hiển thị hộp thoại xác nhận giả lập (`:target`), nhưng chưa gửi dữ liệu về máy chủ (Backend) hoặc gửi email xác nhận tự động tới khách hàng.

### 6.2. Hướng phát triển trong tương lai (Future Roadmap)
Để nâng cấp **CampVibe Glamping** thành một hệ thống thương mại điện tử hoàn chỉnh đưa vào vận hành thực tế, dự án định hướng phát triển theo 3 giai đoạn:
* **Giai đoạn 1 — Tương tác động với JavaScript (ES6+):**
  * Tự động tính toán tổng chi phí đặt lều theo thời gian thực (dựa trên ngày nhận/trả lều, phụ thu cuối tuần/lễ Tết và dịch vụ đi kèm).
  * Nâng cấp bộ lọc đa điều kiện kết hợp tìm kiếm theo từ khóa, khoảng giá và tiện ích.
* **Giai đoạn 2 — Xây dựng Backend & Cơ sở dữ liệu:**
  * Phát triển API bằng Node.js (Express) hoặc PHP kết nối cơ sở dữ liệu (SQL Server / MySQL) để quản lý trạng thái lều trống theo ngày thực tế, tránh trùng lịch đặt.
  * Tích hợp cổng thanh toán trực tuyến (VNPay, MoMo, chuyển khoản VietQR) và tự động gửi email xác nhận đơn đặt phòng.
* **Giai đoạn 3 — Hệ thống Quản trị (Admin Dashboard):**
  * Xây dựng trang quản trị dành cho chủ khu cắm trại để thêm/sửa/xóa thông tin lều, cập nhật bảng giá theo mùa và thống kê doanh thu đặt lịch.
=======
>>>>>>> 8d0c81f9e71a81da0f254542a7472e7a98ba8dee
