# Xây dựng website bán mỹ phẩm trực tuyến

**Môn học:** Phát triển ứng dụng web mã nguồn mở

**Giảng viên hướng dẫn:** Nguyễn Ngọc Dan Thanh

**Lớp:** DA23TTB
---

## 👥 Thành viên nhóm

| STT | Họ và tên | MSSV | Vai trò / Phần việc phụ trách |
|:---:|-----------|:----:|-------------------------------|
| 1 | Huỳnh Lê Ngọc Trinh  | 110123058| Backend, Database|
| 2 | Thạch Thị Ngọc Trâm | 110123057 | Giao diện, Frontend |
| 3 | Trần Nguyễn Hoàng Ân| 110123069| Kiểm thử, Tài liệu |
---

## 📖 Giới thiệu đề tài


### Chức năng chính

- Xem danh sách và chi tiết sản phẩm mỹ phẩm
- Tìm kiếm, lọc sản phẩm theo danh mục / thương hiệu
- Giỏ hàng và đặt hàng
- Đăng ký, đăng nhập tài khoản
- Trang quản trị (quản lý sản phẩm, đơn hàng, người dùng)
- [Bổ sung thêm chức năng của nhóm]

---

## 🛠 Công nghệ sử dụng

| Thành phần | Công nghệ |
|------------|-----------|
| Ngôn ngữ | PHP 8.2+ |
| Framework | CodeIgniter 4 |
| Cơ sở dữ liệu | MySQL |
| Giao diện | HTML, CSS, JavaScript, [Bootstrap] |
| Triển khai | Docker, Apache |
| Quản lý mã nguồn | Git, GitHub |

---

## ⚙️ Yêu cầu hệ thống

- PHP **8.2** trở lên, bật các extension: `intl`, `mbstring`, `json`, `mysqlnd`
- Composer 2
- MySQL / MariaDB
- (Tuỳ chọn) Docker Desktop

---

## 🚀 Hướng dẫn cài đặt
### Chạy bằng Docker

```bash
docker compose up --build
```

---

## 📁 Cấu trúc thư mục

```
├── app/          # Controllers, Models, Views, Config
├── public/       # index.php, CSS, JS, hình ảnh
├── writable/     # Cache, logs, uploads
├── tests/        # Kiểm thử
├── Dockerfile
└── composer.json
```

## 📝 Phân công công việc

| Thành viên | Vai trò | Công việc đã thực hiện |
|------------|---------|------------------------|
| Huỳnh Lê Ngọc Trinh| Backend | Khởi tạo dự án CodeIgniter 4, thiết kế cơ sở dữ liệu, xây dựng chức năng đăng nhập / đăng ký, giỏ hàng và thanh toán, cấu hình Docker, Xây dựng chức năng quản trị: quản lý sản phẩm, danh mục, đơn hàng, người dùng và dashboard thống kê |
| Thạch Thị Ngọc Trâm | Frontend | Thiết kế giao diện trang chủ, danh sách sản phẩm, chi tiết sản phẩm, giao diện responsive bằng HTML, CSS, JavaScript |
| Trần Nguyễn Hoàng Ân | Kiểm thử, Tài liệu | Kiểm thử các chức năng, ghi nhận và báo lỗi, viết báo cáo, chụp ảnh demo, soạn slide thuyết trình |

## 📚 Tài liệu tham khảo

- [CodeIgniter 4 User Guide](https://codeigniter.com/user_guide/)
- [PHP Manual](https://www.php.net/manual/)
