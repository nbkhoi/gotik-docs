# Ngày 1

> - **Mục tiêu:** Hoàn thành thiết lập Google Workspace, cấu hình email, Google Drive, và Google Calendar, Bitbucket cho dự án Gotik.
> - **Definition of Done:**
>   - Hệ thống Google Workspace và Bitbucket được thiết lập và bảo mật đầy đủ.
>   - Email, Google Drive, và Google Calendar đã được cấu hình cho nhóm dự án.
>   - Tất cả thành viên nhóm đều có tài khoản email và quyền truy cập vào Google Drive.
>   - Bitbucket invitations đã được gửi đến tất cả các email đã cấp cho từng thành viên nhóm phát triển.
>   - Phân quyền truy cập đã được cấu hình cho Google Drive và Bitbucket.

## 1. Google Workspace - Email, Calendar, and File Sharing

### 1.2 Prerequisites

- [x] **Chuẩn bị thông tin cần thiết**:
  - Tên doanh nghiệp.
  - Số lượng người dùng ban đầu.
  - Tên miền sẵn có (và quyền truy cập để quản lý DNS).
  - Thông tin liên hệ của người quản trị.

---

### 1.2 Action checklist

- [x] **1. Tạo tài khoản Google Workspace**:
  - [x] Đăng ký Google Workspace cho doanh nghiệp.
  - [x] Thiết lập hệ thống quản trị người dùng và tạo miền `@gotik.vn`.
  - [x] Xác minh quyền sở hữu tên miền và hoàn thành cấu hình cho việc gửi và nhận email.

- [x] **2. Cấu hình email cho nhóm dự án**:
  - [x] Tạo tài khoản email cho 8 thành viên nhóm với tên miền công ty `@gotik.vn`.
  - [x] Kích hoạt xác thực hai yếu tố (2FA) cho mỗi tài khoản.

- [x] ~~**3. Thiết lập Google Drive**:~~
  - [ ] ~~Tạo và cấu trúc Google Drive dùng chung cho nhóm với các thư mục như **Dự án**, **Tài liệu kỹ thuật**, **Tài liệu hướng dẫn**, **Cuộc họp**.~~
  - [ ] ~~Phân quyền truy cập dựa theo vai trò và trách nhiệm của từng thành viên.~~
  > *Note:* Gói Google Workspace Starter không hỗ trợ không gian lưu trữ chung trên Google Drive. (Xem chi tiết: [Google Workspace - So sánh gói](https://workspace.google.com/intl/vi/pricing.html))

- [x] **4. Cấu hình Google Calendar**:
  - [x] Tạo lịch nhóm để quản lý cuộc họp và sự kiện quan trọng.
  - [x] Chia sẻ quyền chỉnh sửa và xem lịch dựa trên vai trò của từng thành viên.
  - [x] Thiết lập thông báo để đảm bảo không bỏ lỡ cuộc họp và sự kiện quan trọng.

- [x] **5. Kiểm tra và bảo mật**:
  - [x] Đảm bảo tất cả thông tin được cấu hình đúng và an toàn.
  - [x] Kiểm tra lại xác thực hai yếu tố (2FA) để đảm bảo tính an toàn.

- [x] **6. Chia sẻ thông tin với thành viên**:
  - [x] Gửi email thông báo về tài khoản Google Workspace.
  - [x] Hướng dẫn cách truy cập và sử dụng email, Google Drive, và Google Calendar.

## 2. Bitbucket - Source Code Management

### 2.1 Prerequisites

- [x] **Chuẩn bị thông tin cần thiết**:
  - Tên tổ chức Bitbucket.
  - Số lượng người dùng ban đầu.
  - Thông tin liên hệ của người quản trị.

---

### 2.2 Action checklist

- [x] **1. Tạo tài khoản Bitbucket cho doanh nghiệp**:
  - [x] Đăng ký tài khoản Bitbucket cho doanh nghiệp và thiết lập tổ chức Gotik.
  - [x] Mời tất cả thành viên vào tổ chức với quyền truy cập phù hợp.

- [x] **2. Cấu hình kho lưu trữ mã nguồn**:
  - [x] Tạo kho lưu trữ cho dự án Gotik với các nhánh chính `master`, `develop`, và nhánh tính năng (`feature`).
  - [x] Quy định rõ ràng về việc tạo, gộp và review nhánh để đảm bảo tính minh bạch.

- [x] **3. Phân quyền**:
  - [x] Phân quyền cho các thành viên với các mức truy cập phù hợp với vai trò (admin, developer, viewer).

- [x] **4. Cấu hình chính sách bảo mật**:
  - [x] Cấu hình bảo mật cho kho mã nguồn, bao gồm yêu cầu xác thực 2 bước và quản lý quyền truy cập.
  - [x] Đảm bảo có kế hoạch backup định kỳ mã nguồn nhằm tránh mất mát dữ liệu.

---
