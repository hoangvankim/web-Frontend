# BÁO CÁO PHÂN TÍCH CẤU TRÚC WEBSITE THỰC TẾ (DEV.TO / TECH PORTAL)

## 1. Trang web phân tích
- **Tên trang**: Trang báo / Cộng đồng công nghệ **Dev.to** & **TechCrunch**
- **Mục tiêu phân tích**: Tìm hiểu cách bố trí các thành phần cơ bản của một trang web tin tức / cổng thông tin hiện đại.

---

## 2. Phân tích chi tiết từng phần của trang web

### • Header (Phần đầu trang)
- **Vị trí**: Đặt tại vị trí cao nhất trên trang web.
- **Vai trò & Thành phần**:
  - Chứa Logo nhận diện thương hiệu nổi bật (`DEV` / `TechPortal`).
  - Ô tìm kiếm từ khóa nhanh để người dùng tra cứu tài liệu/bài viết.
  - Nút đăng ký/đăng nhập thành viên ở góc phải.
- **Cách bố trí**: Sử dụng Flexbox dàn ngang, căn đều 2 bên (`justify-content: space-between; align-items: center`).

### • Navigation Menu (Thanh điều hướng)
- **Vị trí**: Nằm liền kề Header, cố định trên đầu trang khi cuộn (`position: sticky`).
- **Thành phần**: Có ít nhất 4 mục điều hướng chính:
  1. *Trang chủ (Home)*
  2. *Tin tức công nghệ (Latest News)*
  3. *Lập trình & Hướng dẫn (Tutorials)*
  4. *Diễn đàn thảo luận (Community)*
  5. *Liên hệ (Contact)*
- **Cách bố trí**: Dạng danh sách nằm ngang (`display: flex; gap: 20px`), có hiệu ứng đổi màu khi hover.

### • Content Section (Khu vực nội dung chính)
- **Bố cục chính**: Sử dụng bố cục đa cột (Grid hoặc Flexbox) chia làm 2 phần cân đối:
  - **Cột Nội dung chính (Main Content - 70%)**: Chứa danh sách các bài viết dạng Card. Mỗi bài viết gồm: Hình ảnh minh họa (thumbnail), Tiêu đề bài viết, Thông tin tác giả & ngày đăng, Đoạn trích dẫn ngắn và nút "Đọc tiếp".
  - **Cột Nội dung phụ (Sidebar - 30%)**: Hiển thị danh mục chuyên mục phổ biến, các hashtag nổi bật, thông báo và tin tức xem nhiều nhất.

### • Footer (Phần chân trang)
- **Vị trí**: Nằm ở đáy trang web, sử dụng tông màu tối để tách biệt với phần nội dung.
- **Thành phần**:
  - Thông tin bản quyền (`© 2026 TechPortal. All rights reserved`).
  - Danh sách liên kết nhanh: Điều khoản sử dụng, Chính sách bảo mật, Tuyển dụng.
  - Các biểu tượng mạng xã hội (Facebook, Twitter, GitHub, LinkedIn).
- **Cách bố trí**: Bố cục 2 hoặc 3 cột bằng Flexbox, căn đều khoảng cách và căn giữa trên thiết bị di động.

---

## 3. Bản triển khai tái hiện (Rebuild)
Mã nguồn triển khai lại cấu trúc trên đã được hoàn thiện trong hai tệp `index.html` và `style.css`.
