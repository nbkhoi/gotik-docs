# Requirement Document

> - **Project:** Gotik
> - **Title:** Thiết lập bộ công cụ cộng tác và quản lý dự án
> - **Date:** 2024-10-24
> - **Version:** 1.0
> - **Status:** Draft

## 1. Mô tả yêu cầu

Thiết lập và cấu hình Bộ công cụ cộng tác và quản lý dự án bao gồm Git, Jira, Confluence, Slack, và Google Workspace nhằm hỗ trợ nhóm phát triển 6 thành viên thực hiện dự án Gotik hiệu quả. Bộ công cụ cần đảm bảo tính đồng bộ, an toàn, dễ sử dụng và hỗ trợ tối ưu cho việc quản lý mã nguồn, theo dõi tiến độ, giao tiếp và chia sẻ tài liệu trong nhóm.

## 2. Mục tiêu

- Cung cấp một môi trường phát triển cộng tác hiệu quả.
- Đảm bảo quản lý mã nguồn rõ ràng, theo dõi tiến độ, quản lý nhiệm vụ và giao tiếp giữa các thành viên dự án.
- Đảm bảo bảo mật và quản lý quyền truy cập chặt chẽ.

## 3. Các yêu cầu cụ thể

### 3.1. Google Workspace - Email, Calendar, and File Sharing

- **Chức năng:** Quản lý email, lịch làm việc, và chia sẻ tài liệu trong nhóm.

- **Yêu cầu**

  - Tạo tài khoản Google Workspace cho doanh nghiệp.
  - Tạo hệ thống email với tên miền `@gotik.vn`.
  - Cấp tài khoản email cho tất cả thành viên dự án với tên miền công ty `@gotik.vn`.
  - Tạo Google Drive để lưu trữ tài liệu dự án, chia sẻ quyền truy cập phù hợp.
  - Thiết lập Google Calendar để quản lý các cuộc họp và sự kiện quan trọng.
  - Cấu hình bảo mật email (2FA) và lọc spam.

### 3.2. Git - Source Code Management

- **Chức năng:** Quản lý mã nguồn, theo dõi thay đổi code, hỗ trợ pull request, review code.

- **Yêu cầu**

  - Tạo tài khoản Bitbucket cho doanh nghiệp.
  - Lưu trữ mã nguồn trên nền tảng **Bitbucket**.
  - Cấu hình các nhánh chính `master`, `develop`, và sử dụng branching model hợp lý.
  - Mời thành viên vào kho lưu trữ với các quyền truy cập phù hợp. Email thành viên phải là email đã được cấp với tên miền `@gotik.vn`.
  - Đảm bảo phân quyền cho các thành viên.

### 3.3. Jira - Project Management

- **Chức năng:** Quản lý nhiệm vụ, theo dõi tiến độ, hỗ trợ Scrum/Kanban.

- **Yêu cầu**

  - Tạo tài khoản Atlassian cho doanh nghiệp.
  - Tạo tổ chức Gotik trên Jira.
  - Tạo dự án cho Gotik trên Jira với cấu trúc board Kanban hoặc Scrum.
  - Xác định các issue types, statuses, workflows, và custom fields cần thiết.
  - Tích hợp với Git để theo dõi commit và pull request liên quan đến các nhiệm vụ.
  - Phân quyền cho các thành viên nhóm.

### 3.4. Confluence - Documentation

- **Chức năng:** Quản lý tài liệu, chia sẻ thông tin giữa các thành viên nhóm.

- **Yêu cầu**

  - Tạo không gian làm việc (space) cho dự án Gotik.
  - Tạo cấu trúc tài liệu cho các tài liệu yêu cầu dự án, kiến trúc hệ thống, tài liệu hướng dẫn kỹ thuật.
  - Phân quyền cho các thành viên nhóm.
  - Tích hợp với Jira để liên kết tài liệu và nhiệm vụ.

### 3.5. Slack - Communication & Collaboration

- **Chức năng:** Giao tiếp nhanh, trao đổi thông tin, hỗ trợ tích hợp với các công cụ khác.

- **Yêu cầu**

  - Đăng ký tài khoản Slack cho doanh nghiệp.
  - Tạo workspace cho dự án Gotik.
  - Mời thành viên vào workspace. Email thành viên phải là email đã được cấp với tên miền `@gotik.vn`.
  - Tạo các kênh như `#general`, `#dev`, `#qa`, `#management` để đảm bảo giao tiếp phân loại.
  - Tích hợp với Jira, Bitbucket, Google Calendar để thông báo tự động.
  - Thiết lập bot hỗ trợ họp stand-up tự động. (Optional)

---

- **Người viết:**
  - **Họ tên:** Nguyễn Bảo Khôi
  - **Vai trò:** Technical Leader
  - **Email:**

- **Người phê duyệt:**
  - **Họ tên:** Phạm Trần Phương Thùy
  - **Vai trò:** Project Manager
  - **Email:**