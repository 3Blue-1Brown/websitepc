# 💻 Nam Nguyễn PC & Workstation — Website Thương Mại Điện Tử Linh Kiện PC & Server

![Nam Nguyễn PC Banner](https://lh3.googleusercontent.com/d/1aJrob1zC9A9K5AuapaBU06zoPS8woQmv=s2500)

> **Website thương mại điện tử hiện đại, tối ưu tốc độ cao, chuyên kinh doanh Linh Kiện PC Gaming, Máy Tính Văn Phòng, Server & Workstation Doanh Nghiệp.**

---

## 🚀 THÔNG TIN DỰ ÁN & ĐƯỜNG DẪN TRUY CẬP

* **🌐 Website Sản Xuất (Live Production)**: [https://pcnamnguyen.onrender.com](https://pcnamnguyen.onrender.com)
* **🐙 Repository GitHub**: [https://github.com/pcnamnguyen/pcnamnguyen](https://github.com/pcnamnguyen/pcnamnguyen)
* **⚡ Nền tảng Hosting Web**: Render Web Service (Tự động Deploy khi Push nhánh `main`)
* **🗄️ Nền tảng Database**: Clever Cloud MySQL Managed Service (Region Montreal, Canada)

---

## ✨ TÍNH NĂNG NỔI BẬT

### 🛍️ Giao Diện Khách Hàng (Storefront)
* **Trang chủ & Banner Khuyến Mãi**: 
  * 3 Khung Banner Sale tỉ lệ 1:1 hình vuông được **quản lý động 100% từ trang Admin**.
  * Thuộc tính `object-fit: contain` hiển thị trọn vẹn 100% hình ảnh & chữ banner không bị cắt xém.
  * Bộ đồng hồ đếm ngược Flash Sale chạy thời gian thực.
* **Lọc & Tìm kiếm Sản phẩm Thông minh**:
  * Bấm vào từng Banner Sale để **lọc chính xác danh sách sản phẩm giảm giá** tương ứng (PC Gaming, Server/WS, Phụ kiện nâng cấp).
  * Tìm kiếm tức thì (Live Search Sync) theo Tên sản phẩm, Thương hiệu, Danh mục, Thông số kỹ thuật.
* **Xây Dựng Cấu Hình PC (PC Builder)**:
  * Công cụ tự phối ghép cấu hình máy tính theo nhu cầu.
  * Tự động tính tổng ngân sách & xuất file / gửi báo giá qua Zalo QR.
* **Giỏ Hàng & Đặt Hàng Nhanh**:
  * Giỏ hàng lưu trữ LocalStorage mượt mà.
  * Quy trình thanh toán đơn giản, lưu đơn hàng trực tiếp vào Database & ghi nhật ký hoạt động.

### 🛡️ Trang Quản Trị Hệ Thống (Admin Panel)
* **Đường dẫn Admin**: `https://pcnamnguyen.onrender.com/admin/login.html`
* **Tài khoản mặc định**: `admin` | **Mật khẩu**: `admin123`
* **Chức năng Admin**:
  * **Báo cáo Thống kê**: Xem tổng doanh thu, số lượng đơn hàng, số sản phẩm đang kinh doanh.
  * **Quản lý Sản phẩm (CRUD)**: Thêm mới, sửa thông tin, cập nhật giá khuyến mãi, chọn ảnh đại diện & ẩn/xóa sản phẩm.
  * **Quản lý Banner Động**: Thêm/sửa/xóa Banner từ link Google Drive hoặc đường dẫn ảnh tĩnh.
  * **Quản lý Đơn hàng**: Xem chi tiết khách hàng đặt, thay đổi trạng thái đơn hàng (Mới đặt, Đã xác nhận, Đang giao, Hoàn thành, Hủy).
  * **Nhật ký Hoạt động (Activity Logs)**: Ghi lại toàn bộ lịch sử thao tác của các tài khoản Admin.

---

## 🛠️ CÔNG NGHỆ SỬ DỤNG (TECH STACK)

| Phân Mục | Công Nghệ / Thư Viện |
| :--- | :--- |
| **Frontend** | HTML5, Vanilla CSS3 (Custom Design System, Glassmorphism, Micro-animations), JavaScript ES6+ (Fetch API, LocalStorage, Async/Await) |
| **Backend** | Node.js, Express.js RESTful API, JSON Web Token (JWT Authentication), `compression` (Gzip/Brotli ~70% payload size reduction) |
| **Database** | MySQL Managed Service trên Clever Cloud (`mysql2/promise` connection pool with 7 indexed query columns) |
| **Media & CDN** | Google Content Delivery Network (`lh3.googleusercontent.com`), Resource Preconnect & DNS Prefetching |
| **Deployment** | Render Web Service Auto-Deploy Continuous Integration |

---

## 🗄️ THÔNG TIN KẾT NỐI CƠ SỞ DỮ LIỆU (CLEVER CLOUD MYSQL)

* **Tên Addon Database**: `webpc-db`
* **Host / Server**: `bpxbnkamftkyaifgkxam-mysql.services.clever-cloud.com`
* **Port**: `3306`
* **Database Name**: `bpxbnkamftkyaifgkxam`
* **User**: `uifzbso0jkk48vaa`
* **Password**: `ZHzoNCQ1yHIELfX2h1MZ`

### 🔗 Liên kết Quản trị CSDL (phpMyAdmin):
1. **[Mở giao diện phpMyAdmin qua Clever Cloud Console](https://console.clever-cloud.com)**  
   *(Vào [console.clever-cloud.com](https://console.clever-cloud.com) ➔ Bấm **Personal space** ➔ Chọn **`webpc-db`** ➔ Bấm nút màu xanh **PHPMyAdmin**)*
2. **[Cổng đăng nhập phpMyAdmin độc lập](https://phpmyadmin.services.clever-cloud.com)**

---

## 💻 HƯỚNG DẪN CÀI ĐẶT & CHẠY DỰ ÁN CỤC BỘ (LOCAL SETUP)

### 1. Tải Mã Nguồn (Clone Repository)
```bash
git clone https://github.com/pcnamnguyen/pcnamnguyen.git
cd pcnamnguyen
```

### 2. Cài Đặt Thư Viện (Install Dependencies)
```bash
npm install
```

### 3. Cấu Hình Biến Môi Trường (Environment Variables)
Tạo tệp `backend/.env` với nội dung:
```env
PORT=3000
JWT_SECRET=namnguyen_pc_workstation_secret_key_2026
JWT_EXPIRES_IN=1h
JWT_REMEMBER_EXPIRES=30d

DB_HOST=bpxbnkamftkyaifgkxam-mysql.services.clever-cloud.com
DB_USER=uifzbso0jkk48vaa
DB_PASSWORD=ZHzoNCQ1yHIELfX2h1MZ
DB_NAME=bpxbnkamftkyaifgkxam
DB_PORT=3306
```

### 4. Khởi Chạy Server (Start Server)
```bash
npm start
```
Mở trình duyệt truy cập: `http://localhost:3000`

---

## 📂 CẤU TRÚC THƯ MỤC DỰ ÁN

```text
webpc1/
├── backend/
│   ├── app.js                 # Server Express chính (Routes, Static Files, Middleware)
│   ├── db.js                  # Khởi tạo MySQL Connection Pool kết nối Clever Cloud
│   ├── routes/                # Các tuyến API RESTful (/api/products, /api/banners, /api/orders...)
│   └── .env                   # Tệp chứa biến môi trường & mật khẩu DB
├── frontend/
│   ├── index.html             # Trang chủ (Flash Sale Banners, Slider, Sản phẩm nổi bật)
│   ├── products.html          # Trang danh sách sản phẩm, bộ lọc & tìm kiếm
│   ├── product_detail.html    # Trang chi tiết sản phẩm & thông số kỹ thuật
│   ├── pc-builder.html        # Trang xây dựng cấu hình PC
│   ├── cart.html              # Trang giỏ hàng
│   ├── checkout.html          # Trang đặt hàng & thanh toán
│   ├── admin/                 # Trang quản trị Admin (Dashboard, Sản phẩm, Đơn hàng, Banner)
│   ├── css/
│   │   └── style.css          # CSS thiết kế hệ thống giao diện
│   └── js/                    # Thư viện JavaScript hỗ trợ
├── docs/                      # Tài liệu kỹ thuật chi tiết dự án (TAI_LIEU_KY_THUAT.md)
└── README.md                  # Hướng dẫn & giới thiệu tổng quan dự án
```

---

📝 *Dự án được xây dựng và tối ưu hoàn chỉnh cho Nam Nguyễn PC & Workstation (2026).*
