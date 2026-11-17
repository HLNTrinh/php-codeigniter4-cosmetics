# XÂY DỰNG WEBSITE BÁN MỸ PHẨM TRỰC TUYẾN

**Môn học:** PHÁT TRIỂN ỨNG DỤNG WEB VỚI MÃ NGUỒN MỞ
**Giảng viên hướng dẫn:** Nguyễn Ngọc Đan Thanh
**Lớp:** DA23TTB

---

## 👥 Thành viên nhóm

| STT | Họ và tên | MSSV | Vai trò / Phần việc phụ trách |
|:---:|-----------|:----:|-------------------------------|
| 1 | Huỳnh Lê Ngọc Trinh | 110123058 |  Backend, Database|
| 2 | Thạch Thị Ngọc Trâm| 110123057 |  Giao diện, Frontend|
| 3 | Trần Nguyễn Hoàng Ân | 110123069 | Kiểm thử, Tài liệu |
---
## 📖 Giới thiệu đề tài

### Lý do chọn đề tài

Thị trường mỹ phẩm ngày càng phát triển, người tiêu dùng có xu hướng tìm hiểu và mua sắm trực tuyến thay vì đến cửa hàng. Tuy nhiên, nhiều cửa hàng nhỏ vẫn quản lý sản phẩm và đơn hàng thủ công, dễ sai sót và khó mở rộng. Vì vậy, nhóm chọn xây dựng một website bán mỹ phẩm giúp khách hàng mua sắm thuận tiện, đồng thời giúp chủ cửa hàng quản lý kinh doanh hiệu quả hơn.

### Mục tiêu

- Xây dựng website bán mỹ phẩm hoàn chỉnh bằng framework **CodeIgniter 4** theo mô hình MVC.
- Cho phép khách hàng xem sản phẩm, đặt hàng và theo dõi đơn hàng dễ dàng.
- Cung cấp trang quản trị để quản lý sản phẩm, danh mục, đơn hàng và người dùng.
- Triển khai dự án bằng **Docker** để chạy ổn định trên nhiều môi trường.

### Đối tượng sử dụng

| Đối tượng | Vai trò |
|-----------|---------|
| Khách truy cập | Xem sản phẩm, tìm kiếm, đăng ký tài khoản |
| Khách hàng | Thêm vào giỏ hàng, thanh toán, xem lịch sử đơn hàng, quản lý hồ sơ |
| Quản trị viên | Quản lý sản phẩm, danh mục, đơn hàng, người dùng và xem thống kê |

### Chức năng chính

- **Khách truy cập:** xem trang chủ, danh sách và chi tiết sản phẩm, tìm kiếm và lọc theo danh mục, đăng ký và đăng nhập.
- **Khách hàng:** quản lý giỏ hàng, đặt hàng và thanh toán, xem lịch sử đơn hàng, cập nhật hồ sơ cá nhân, lưu sản phẩm yêu thích.
- **Quản trị viên:** dashboard thống kê, thêm / sửa / xoá sản phẩm và danh mục, xử lý đơn hàng, quản lý tài khoản người dùng.

### Phạm vi đề tài

Dự án tập trung vào các chức năng cốt lõi của một website thương mại điện tử. Các tính năng nâng cao như thanh toán trực tuyến qua cổng thanh toán, gợi ý sản phẩm bằng AI hay ứng dụng di động chưa nằm trong phạm vi của đề tài này.

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

### Cách 1: Chạy trực tiếp

```bash
git clone https://github.com/HLNTrinh/php-codeigniter4-cosmetics.git
cd php-codeigniter4-cosmetics
composer install
cp env .env
```

Mở file `.env` và chỉnh `baseURL` cùng thông tin database:

```ini
app.baseURL = 'http://localhost:8080/'

database.default.hostname = localhost
database.default.database = [tên_database]
database.default.username = root
database.default.password =
database.default.DBDriver = MySQLi
```

Chạy migration (nếu có) và khởi động server:

```bash
php spark migrate
php spark serve
```

Truy cập: http://localhost:8080

### Cách 2: Chạy bằng Docker

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

---



## 📝 Phân công công việc

| Thành viên | Vai trò | Công việc đã thực hiện |
|------------|---------|------------------------|
| Huỳnh Lê Ngọc Trinh | Backend | Khởi tạo dự án CodeIgniter 4, thiết kế cơ sở dữ liệu, xây dựng chức năng đăng nhập / đăng ký, giỏ hàng và thanh toán, cấu hình Docker, Xây dựng chức năng quản trị: quản lý sản phẩm, danh mục, đơn hàng, người dùng và dashboard thống kê|
| Thạch Thị Ngọc Trâm | Frontend | Thiết kế giao diện trang chủ, danh sách sản phẩm, chi tiết sản phẩm, giao diện responsive bằng HTML, CSS, JavaScript |
| Trần Nguyễn Hoàng Ân | Kiểm thử, Tài liệu | Kiểm thử các chức năng, ghi nhận và báo lỗi, viết báo cáo, chụp ảnh demo, soạn slide thuyết trình |
---