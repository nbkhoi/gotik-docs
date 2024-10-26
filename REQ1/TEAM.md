# Thiết Lập Bộ Công Cụ Cộng Tác và Quản Lý Dự Án - Cấu Trúc Team và Phân Vai Trò

---
>
> - **Title:** Thiết Lập Bộ Công Cụ Cộng Tác và Quản Lý Dự Án - Cấu Trúc Team và Phân Vai Trò
> - **Project:** Gotik  
> - **Date:** 2024-10-24  
> - **Status:** Draft  
> - **Version:** 1.0
> - **Version History:**
>
>   | Phiên bản | Ngày       | Người tạo        | Nội dung cập nhật              |
>   |-----------|------------|------------------|---------------------------------|
>   | 1.0       | 2024-10-24 | Nguyễn Bảo Khôi  | Bản nháp ban đầu                |
>
---

## Xác định các vai trò

### 1. **System Administrator kiêm DevOps Engineer (1 người)**

**Vai trò chính:**

- **Thiết lập hệ thống:**
  - Cài đặt và quản lý các công cụ chính như AWS WorkMail hoặc Google Workspace, Jira, Confluence, Bitbucket, và Slack.
- **Tích hợp công cụ:**
  - Cấu hình tích hợp giữa các công cụ để luân chuyển thông tin dễ dàng, ví dụ tích hợp Jira với Bitbucket và gửi thông báo từ Bitbucket sang Slack.
- **Thiết lập CI/CD:**
  - Thiết lập và quản lý Bitbucket Pipelines để tự động hóa việc build và triển khai mã nguồn.
- **Quản lý quyền truy cập và bảo mật:**
  - Đảm bảo tất cả các công cụ đều được cấu hình bảo mật và phân quyền truy cập đúng theo vai trò.

**Kỹ năng cần có:**

- Quản trị hệ thống (cấu hình email, quản lý quyền truy cập).
- Kỹ năng về DevOps (cấu hình CI/CD, quản lý Pipelines).
- Kiến thức về bảo mật hệ thống.

---

### 2. **Project Manager kiêm Training và Documentation Specialist (1 người)**

**Vai trò chính:**

- **Thiết lập dự án:**
  - Cấu hình Jira để quản lý dự án, theo dõi công việc, tạo quy trình làm việc và phân công task cho nhóm.
- **Quản lý tài liệu:**
  - Tạo cấu trúc và quản lý tài liệu dự án trong Confluence, bao gồm tài liệu yêu cầu, kiến trúc, và hướng dẫn kỹ thuật.
- **Đào tạo nhóm:**
  - Hướng dẫn các thành viên cách sử dụng Jira, Confluence, và Slack để đảm bảo mọi người đều hiểu cách làm việc với hệ thống mới.
- **Truyền thông:**
  - Quản lý giao tiếp giữa các thành viên trong nhóm qua Slack và đảm bảo quy trình liên lạc rõ ràng, hiệu quả.

**Kỹ năng cần có:**

- Kinh nghiệm quản lý dự án với Jira.
- Kỹ năng quản lý tài liệu trong Confluence.
- Kỹ năng truyền thông và đào tạo nhóm.

---

### 3. **Developer**

**Vai trò chính:**

- **Thử nghiệm môi trường:**
  - Thực hiện các thao tác như commit mã nguồn, tạo pull request trong Bitbucket, và kiểm tra quá trình CI/CD để đảm bảo môi trường phát triển hoạt động trơn tru.
- **Góp ý cải thiện:**
  - Phối hợp với DevOps Engineer để tinh chỉnh quy trình tự động hóa build và deploy.
  
**Kỹ năng cần có:**

- Kinh nghiệm làm việc với Bitbucket và Pipelines.
- Hiểu biết về Git và quy trình quản lý mã nguồn.

---

## Tóm tắt

### Tối thiểu 2 người có thể thực hiện thiết lập môi trường

1. **Người 1: System Administrator and DevOps Engineer**
   - Đảm nhiệm toàn bộ việc thiết lập và quản lý các công cụ hệ thống (email, quản lý mã nguồn, CI/CD) và bảo mật.

2. **Người 2: Project Manager kiêm Training & Documentation Specialist**
   - Đảm bảo quản lý dự án, tài liệu, và giao tiếp trong nhóm, đồng thời đào tạo các thành viên sử dụng hệ thống mới.

### Tùy chọn

- **Developer:** Tham gia sớm để thử nghiệm việc tích hợp mã nguồn và CI/CD ngay trong giai đoạn thiết lập.

---
