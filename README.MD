🏕️ CampVibe - Website Đặt Lịch & Trải Nghiệm Cắm Trại Cao Cấp (Glamping)

Bài tập lớn A3 — Học phần FIT4014: Thiết kế web và triển khai hệ thống phần mềm

Trường Đại học Đại Nam | Khoa Công nghệ Thông tin

🔗 1. Liên kết Bàn giao & Triển khai

🌐 Website trực tuyến (Live Demo):

📂 Kho mã nguồn (Repository):

🏷️ Phiên bản phát hành (Release Tag): v1.0.0

📝 Nhật ký sử dụng AI: Xem chi tiết tại AI_LOG.md

📋 Ghi chú phiên bản: Xem chi tiết tại RELEASE_NOTES.md

👤 2. Thông tin Sinh viên Thực hiện

Hạng mục

Nội dung

Sinh viên thực hiện

[Điền Họ và Tên của bạn]

Mã sinh viên

1771020716

Lớp / Ngành

[Điền Lớp của bạn] – Công nghệ Thông tin

Giảng viên hướng dẫn

ThS. Lê Thái Bảo

Học kỳ / Năm học

Học kỳ 1 – Năm học 2026–2027

🎯 3. Tổng quan & Mục tiêu Dự án

CampVibe (kết hợp giữa Camp – cắm trại và Vibe – không khí, cảm xúc) là website giới thiệu và đặt lịch nghỉ dưỡng cắm trại cao cấp (Glamping) tại các điểm đến nổi tiếng của Việt Nam như Đà Lạt, Ba Vì và Hồ Cốc.

Mục tiêu thiết kế & Kỹ thuật:

Chuẩn Semantic HTML5: Sử dụng hệ thống thẻ ngữ nghĩa rõ ràng (<header>, <nav>, <main>, <section>, <article>, <aside>, <footer>) giúp tối ưu cấu trúc tài liệu và khả năng truy cập (Accessibility).

100% CSS3 Thuần (Zero JavaScript): Toàn bộ hiệu ứng tương tác (Menu điện thoại, Bộ lọc sản phẩm theo khu vực, Thư viện chuyển đổi ảnh, Modal đọc bài viết, Kiểm tra hợp lệ Form) đều được xây dựng bằng kỹ thuật CSS hiện đại mà không phụ thuộc thư viện bên ngoài.

Responsive Đa thiết bị: Tương thích mượt mà trên mọi độ phân giải màn hình từ điện thoại di động (375px), máy tính bảng (768px) đến máy tính để bàn (1440px).

✨ 4. Các Chức năng & Kỹ thuật CSS Nổi bật

Trang / Thành phần

Tệp nguồn

Kỹ thuật HTML5 / CSS3 áp dụng

Thanh điều hướng (Header)

index.html & style.css

position: sticky, backdrop-filter: blur(), kỹ thuật Checkbox Hack (input[type="checkbox"]:checked) tạo Menu Hamburger trên Mobile.

Trang chủ (Home)

index.html

CSS Grid Bento Layout (grid-column: span 2, grid-row: span 2), hiệu ứng phóng to ảnh mượt mà (transform: scale()), bố cục Flexbox cho khối tiện ích.

Danh sách Khu trại

campsites.html

Bộ lọc địa điểm thuần CSS kết hợp input[type="radio"]:checked và bộ chọn phủ định :not([data-category="..."]) để ẩn/hiện thẻ trại tức thì.

Chi tiết Khu trại

detail.html

Thư viện ảnh tương tác (Gallery Slider) bằng radio + label, bảng giá kẻ sọc (:nth-child(even)), khung đặt phòng trượt cố định (position: sticky).

Cẩm nang Du lịch

blog.html

Bố cục tạp chí (Editorial Layout), trích dẫn <blockquote>, phân trang UI và cửa sổ đọc nhanh bài viết bằng pseudo-class :target.

Liên hệ & Đặt lịch

contact.html

HTML5 Form Validation (required, pattern, minlength) kết hợp :not(:placeholder-shown):invalid / :valid báo viền đỏ/xanh trực quan và hộp thoại xác nhận :target.

🎨 5. Hệ thống Thiết kế (Design System)

Toàn bộ màu sắc, khoảng cách và bo góc được quản lý tập trung thông qua biến CSS (:root) tại tệp assets/css/style.css:

Màu chủ đạo (--primary-color): #2D5A27 (Xanh rêu rừng thông – đại diện cho thiên nhiên).

Màu nhấn (--accent-color): #D97736 (Cam đất lửa trại – tạo điểm nhấn cho nút bấm CTA).

Màu nền phụ (--bg-light): #F7F6F2 (Kem ấm tự nhiên – giúp dịu mắt khi đọc nội dung dài).

Kiểu chữ (Typography): Plus Jakarta Sans (Google Fonts) với các trọng số 400, 500, 600, 700.

📁 6. Cấu trúc Thư mục Mã nguồn

BTL_TKWEB_TKHTPM/
├── index.html              # Trang chủ
├── campsites.html          # Trang danh sách & Bộ lọc khu cắm trại
├── detail.html             # Trang chi tiết lều, thư viện ảnh & bảng giá
├── blog.html               # Trang tạp chí cẩm nang kinh nghiệm
├── contact.html            # Trang liên hệ, bản đồ & phiếu đặt lịch
├── assets/
│   └── css/
│       └── style.css       # Tệp định dạng CSS chung cho toàn bộ website
├── docs/                   # Thư mục lưu trữ Wireframe & minh chứng kiểm thử
├── README.md               # Tài liệu tổng quan & hướng dẫn dự án
├── AI_LOG.md               # Nhật ký khai báo sử dụng công cụ AI
└── RELEASE_NOTES.md        # Ghi chú phiên bản phát hành


🚀 7. Hướng dẫn Cài đặt & Chạy Cục bộ

Dự án là website tĩnh thuần HTML5/CSS3 nên không yêu cầu cài đặt môi trường server phức tạp:

Cách 1 (Xem trực tuyến): Truy cập trực tiếp đường dẫn GitHub Pages:

Cách 2 (Chạy trên máy cá nhân):

# Clone kho lưu trữ về máy
git clone https://github.com/tuan1143/BTL_TKWEB_TKHTPM.git

# Di chuyển vào thư mục dự án
cd BTL_TKWEB_TKHTPM


Sau đó nhấp đúp chuột vào tệp index.html để mở bằng trình duyệt web bất kỳ (Chrome, Edge, Safari) hoặc mở bằng tiện ích Live Server trên Visual Studio Code.

📜 8. Nguồn Tài nguyên Bên ngoài

Hình ảnh minh họa: Thư viện ảnh miễn phí bản quyền Unsplash.

Phông chữ: Google Fonts - Plus Jakarta Sans.

Bản đồ nhúng: Google Maps Embed API.