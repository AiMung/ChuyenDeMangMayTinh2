# Chuyên đề Mạng máy tính 2 (Advanced Computer Networking) 👨‍💻

[![Networking Academy Badge](https://credly.com)](https://www.credly.com/badges/bb47c25d-46df-43f7-8bcb-2ef3c4c74a41/public_url)
# Chuyên đề Mạng máy tính 2 (Advanced Computer Networking) 👨‍💻

<div align="left">
  <a href="https://credly.com" target="_blank">
    <img src="https://credly.com" width="150" alt="Networking Academy Badge">
  </a>
</div>

---
> Repository này lưu trữ các bài tập thực hành và báo cáo chi tiết cho môn học, tập trung vào quản trị hệ thống, mạng P2P và công nghệ Containerization với Docker.


---

### 👤 Thông tin sinh viên
- **Họ và tên:** Nguyễn Ái Mừng
- **Mã số sinh viên:** 2212420
- **Lớp:** CTK46MMT
- **Giảng viên hướng dẫn:** Thầy **LÊ THIÊN ANH**

---

## 📌 Giới thiệu Repository
Nội dung chính bao gồm các kiến thức về quản lý mã nguồn nâng cao với Git và triển khai hạ tầng dịch vụ sử dụng Docker trên môi trường Linux.

## 📁 Cấu trúc dự án
- `Lab01-GitKatas/`: Thực hành Git nâng cao.
- `Lab02-Docker/`:
    - `Lab02.2-Basics/`: Thao tác cơ bản, NAT Port, và liên kết container.
    - `Lab02.3-Volumes/`: Quản lý dữ liệu bền vững.
    - `Lab02.4-Dockerfile/`: Tự động hóa xây dựng Image.
    - `Lab02.5-Compose/`: Triển khai ứng dụng đa container.
- `Reports/`: Các file báo cáo chi tiết và hình ảnh minh chứng.

---

## 🛠 Chi tiết nội dung thực hành Lab 02

### 1. Lab 02.2: Thao tác cơ bản trên Container
*   **Quản lý Container:** Sử dụng `docker run` với các tham số `-i` (interactive), `-t` (terminal), và `-d` (daemon).
*   **Mạng và NAT Port:** Sử dụng flag `-p` để thực hiện mapping port (Ví dụ: `-p 8080:80`).
*   **Liên kết (Link):** Kết nối ứng dụng Web và Database bằng `--link`.
*   **Di chuyển Container:** Thực hiện `export`/`import` container thành file `.tar` hoặc sử dụng `save`/`load` image.

### 2. Lab 02.3: Quản lý dữ liệu (Docker Volume)
*   **Volumes:** Docker quản lý hoàn toàn, hỗ trợ backup an toàn.
*   **Bind Mounts:** Gắn kết trực tiếp thư mục từ máy host vào container.
*   **Tmpfs Mounts:** Lưu trữ trên RAM (không ghi vào ổ đĩa), tăng tốc độ truy xuất.
*   **Cú pháp:** Khuyến nghị dùng `--mount` thay cho `-v` để cấu hình rõ ràng.

### 3. Lab 02.4: Xây dựng Image với Dockerfile
Tự động hóa quy trình build image thông qua script với các chỉ thị:
*   `FROM`, `RUN`, `CMD`, `ENTRYPOINT`, `ENV`, `EXPOSE`, `COPY`, `ADD`.
*   **Thực hành:** Xây dựng thành công Image cho dịch vụ **Apache** trên nền Ubuntu.

### 4. Lab 02.5: Docker Compose
Điều phối ứng dụng đa container thông qua tệp cấu hình YAML:
*   **Quy trình:** Dockerfile → `docker-compose.yml` → `docker-compose up`.
*   **Tính năng:** 
    *   `depends_on`: Quản lý thứ tự khởi chạy dịch vụ.
    *   `scale`: Tăng số lượng container nhanh chóng.
    *   Quản lý tập trung Network, Volume và Environment.

---

## 💻 Môi trường thực hiện
*   **Hệ điều hành:** Ubuntu 22.04 LTS.
*   **Công cụ:** 
    *   **Docker Engine:** Quản lý container.
    *   **Docker Compose:** Điều phối dịch vụ.
    *   **Git:** Quản lý mã nguồn.

---
*Cập nhật lần cuối: 14/04/2026*
