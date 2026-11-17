# XÂY DỰNG WEBSITE BÁN MỸ PHẨM TRỰC TUYẾN

**Môn học:** PHÁT TRIỂN ỨNG DỤNG WEB VỚI MÃ NGUỒN MỞ
**Giảng viên hướng dẫn:** Nguyễn Ngọc Đan Thanh
**Lớp:** DA23TTB

---

## Thành viên nhóm

| Thành viên | Trang / Phần việc | Chức năng |
|------------|-------------------|-----------|
| Huỳnh Lê Ngọc Trinh | Khởi tạo dự án | Cài đặt CodeIgniter 4, cấu hình `.env`, Docker|
| | Cơ sở dữ liệu | Thiết kế các bảng và quan hệ khóa ngoại |
| | Admin: Quản lý sản phẩm | Xem danh sách, thêm, sửa, xóa sản phẩm, upload hình ảnh |
| | Admin: Quản lý danh mục | Xem danh sách, thêm, sửa, xóa danh mục |
| |Thanh toán | Nhập thông tin nhận hàng, xác nhận và tạo đơn hàng |
| | Giao diện Dashboard thống kê | Thống kê doanh thu, số đơn hàng, sản phẩm |
| |Kiểm thử | Kiểm tra các chức năng đăng nhập, tính tiền , ghi nhận và báo lỗi |
| Thạch Thị Ngọc Trâm | Cơ sở dữ liệu | Thiết kế các bảng và quan hệ khóa ngoại |
| | Trang chủ | Thiết kế và xây dựng giao diện trang chủ |
| | Giỏ hàng | Thêm, sửa số lượng, xóa sản phẩm trong giỏ, tính tổng tiền |
| | Giao diện trang Thanh toán | Nhập thông tin nhận hàng, xác nhận và tạo đơn hàng |
| | Admin: Dashboard thống kê | Thống kê doanh thu, số đơn hàng, sản phẩm |
| Trần Nguyễn Hoàng Ân | Đăng nhập / Đăng ký | Tạo tài khoản, đăng nhập, đăng xuất, phân quyền khách hàng / quản trị viên |
| | Cơ sở dữ liệu | Thiết kế các bảng và quan hệ khóa ngoại|
| | Admin: Quản lý đơn hàng | Xem danh sách, xem chi tiết, cập nhật trạng thái đơn hàng |
| | Admin: Quản lý khách hàng | Xem danh sách, xem thông tin, khóa / xóa tài khoản khách hàng |
| | Giao diện trang Quản lý sản phẩm, danh mục|
| | Kiểm thử | Kiểm tra các chức năng thêm xóa sửa hình ảnh, sản phẩm , ghi nhận và báo lỗi |

---
## Giới thiệu đề tài

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

## Công nghệ sử dụng

| Thành phần | Công nghệ |
|------------|-----------|
| Ngôn ngữ | PHP 8.2+ |
| Framework | CodeIgniter 4 |
| Cơ sở dữ liệu | MySQL |
| Giao diện | HTML, CSS, JavaScript, [Bootstrap] |
| Triển khai | Docker, Apache |
| Quản lý mã nguồn | Git, GitHub |

---

## Yêu cầu hệ thống

- PHP **8.2** trở lên, bật các extension: `intl`, `mbstring`, `json`, `mysqlnd`
- Composer 2
- MySQL / MariaDB
- (Tuỳ chọn) Docker Desktop

---

## Hướng dẫn cài đặt

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


