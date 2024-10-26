# Thiết Lập Bộ Công Cụ Cộng Tác và Quản Lý Dự Án - Tài Liệu Phạm Vi Công Việc (SoW)

---
>
> - **Title:** Thiết Lập Bộ Công Cụ Cộng Tác và Quản Lý Dự Án - Tài Liệu Phạm Vi Công Việc (SoW)
> - **Project:** Gotik  
> - **Date:** 2024-10-24  
> - **Status:** Draft  
> - **Version:** 1.2  
> - **Version History:**
>
>   | Phiên bản | Ngày       | Người tạo        | Nội dung cập nhật              |
>   |-----------|------------|------------------|---------------------------------|
>   | 1.0       | 2024-10-24 | Nguyễn Bảo Khôi  | Bản nháp ban đầu                |
>   | 1.1       | 2024-10-26 | Nguyễn Bảo Khôi  | Cập nhật tổng quan và bổ sung hướng dẫn chi tiết |
>   | 1.2       | 2024-10-26 | Nguyễn Bảo Khôi  | Bổ sung hướng dẫn cụ thể cho từng công cụ |
>

---

## 1. Google Workspace - Email, Calendar, and File Sharing

**Tổng quan:**  
Google Workspace cung cấp giải pháp quản lý email, tài liệu, và lịch làm việc, giúp nhóm dự án Gotik dễ dàng chia sẻ tài liệu và lên lịch các cuộc họp quan trọng. Đảm bảo tính bảo mật và dễ sử dụng cho tất cả thành viên.

**Phạm vi công việc:**

1. **Tạo tài khoản Google Workspace:**
   - Đăng ký Google Workspace cho doanh nghiệp, thiết lập hệ thống quản trị người dùng và tạo miền `@gotik.vn`.
   - Xác minh quyền sở hữu tên miền và hoàn thành cấu hình cho việc gửi và nhận email.

2. **Cấu hình email cho nhóm dự án:**
   - Tạo tài khoản email cho 8 thành viên nhóm với tên miền công ty `@gotik.vn`.
   - Cấu hình chữ ký email công ty, lọc thư rác, và kích hoạt xác thực hai yếu tố (2FA) cho mỗi tài khoản.
   - **Hướng dẫn bảo mật:** Định kỳ kiểm tra bảo mật và thực hiện kiểm tra lại xác thực hai yếu tố (2FA) để đảm bảo tính an toàn.

3. **Thiết lập Google Drive:**
   - Tạo và cấu trúc Google Drive dùng chung cho nhóm với các thư mục như **Dự án**, **Tài liệu kỹ thuật**, **Tài liệu hướng dẫn**, **Cuộc họp**.
     > Thùy cung cấp thêm chi tiết về cấu trúc thư mục và quản lý tài liệu non-tech trên Google Drive.
   - **Chính sách phân quyền:** Phân quyền truy cập dựa theo vai trò và trách nhiệm của từng thành viên, đảm bảo tính bảo mật cho tài liệu quan trọng.
     > Thùy cung cấp hướng dẫn cụ thể về cách phân quyền truy cập và quản lý tài liệu trên Google Drive.
4. **Cấu hình Google Calendar:**
   - Tạo lịch nhóm để quản lý cuộc họp và sự kiện quan trọng.
   - **Chia sẻ quyền chỉnh sửa:** Quyền chỉnh sửa và xem lịch sẽ được phân bổ dựa trên vai trò của từng thành viên.
   - **Thiết lập thông báo:** Đặt các thông báo và nhắc nhở để đảm bảo không bỏ lỡ cuộc họp và sự kiện quan trọng.

---

## 2. Git - Source Code Management

**Tổng quan:**  
Bitbucket cung cấp nền tảng quản lý mã nguồn cho dự án Gotik, cho phép nhóm phát triển làm việc đồng thời trên mã nguồn, theo dõi lịch sử thay đổi và thực hiện review code.

**Phạm vi công việc:**

1. **Tạo tài khoản Bitbucket cho doanh nghiệp:**
   - Đăng ký tài khoản Bitbucket cho doanh nghiệp và thiết lập tổ chức Gotik.
   - Mời tất cả thành viên vào tổ chức với quyền truy cập phù hợp.

2. **Cấu hình kho lưu trữ mã nguồn:**
   - Tạo kho lưu trữ cho dự án Gotik với các nhánh chính `master`, `develop`, và nhánh tính năng (`feature`) theo mô hình branching chuẩn:
     - `master`: Chứa mã nguồn đã được kiểm tra và phát hành.
     - `develop`: Nhánh phát triển chính.
     - `feature`: Nhánh phụ để phát triển tính năng mới.
   - **Chính sách nhánh:** Quy định rõ ràng về việc tạo, gộp và review nhánh để đảm bảo tính minh bạch.

3. **Phân quyền:**
   - Phân quyền cho các thành viên với các mức truy cập phù hợp với vai trò (admin, developer, viewer).

4. **Cấu hình chính sách bảo mật:**
   - Cấu hình bảo mật cho kho mã nguồn, bao gồm yêu cầu xác thực 2 bước và quản lý quyền truy cập.
   - **Chính sách backup:** Đảm bảo có kế hoạch backup định kỳ mã nguồn nhằm tránh mất mát dữ liệu.

---

## 3. Jira - Project Management

**Tổng quan:**  
Jira hỗ trợ quản lý nhiệm vụ, theo dõi tiến độ và quy trình làm việc, giúp nhóm dự án tổ chức nhiệm vụ và duy trì tiến độ.

**Phạm vi công việc:**

1. **Tạo tài khoản Atlassian và tổ chức Gotik:**
   - Đăng ký tài khoản Atlassian và tạo tổ chức Gotik trên Jira.

2. **Thiết lập dự án trên Jira:**
   - Tạo dự án Jira cho Gotik với các cấu hình bảng Scrum hoặc Kanban dựa trên nhu cầu của nhóm.
   - **Tạo issue types:** Bao gồm các loại nhiệm vụ như Bug, Task, Story, với các trạng thái (status) như To Do, In Progress, Done.

3. **Cấu hình các issue types và workflows:**
   - Xác định và tạo các loại nhiệm vụ (issue types), trạng thái (statuses), và quy trình công việc (workflows) phù hợp.
   - **Trường tùy chỉnh:** Thêm các trường tùy chỉnh như mức độ ưu tiên (Priority), thời gian ước tính, để theo dõi chi tiết nhiệm vụ.

4. **Tích hợp Git với Jira:**
   - Thiết lập tích hợp giữa Bitbucket và Jira để liên kết commit, pull request với nhiệm vụ.
   - **Liên kết nhiệm vụ:** Đảm bảo các pull request và thay đổi mã nguồn đều được liên kết với nhiệm vụ trên Jira.

5. **Phân quyền:**
   - Phân quyền cho các thành viên nhóm theo vai trò (Project Manager, Developer, ~~QA~~) và kiểm tra định kỳ để đảm bảo phân quyền chính xác.

---

## 4. Confluence - Documentation

**Tổng quan:**  
Confluence là nền tảng lưu trữ tài liệu, cho phép đội ngũ dễ dàng quản lý, chia sẻ và cập nhật tài liệu kỹ thuật, tài liệu yêu cầu, và hướng dẫn sử dụng.

**Phạm vi công việc:**

1. **Tạo không gian làm việc (space) cho dự án Gotik:**
   - Tạo space trên Confluence cho dự án Gotik và cấu trúc các trang tài liệu hợp lý.

2. **Tạo cấu trúc tài liệu:**
   - Xây dựng cấu trúc tài liệu bao gồm: **Yêu cầu dự án**, **Kiến trúc hệ thống**, **Hướng dẫn kỹ thuật**, **Tài liệu tham khảo**.
   - **Template tài liệu:** Cung cấp mẫu tài liệu cho từng phần để đảm bảo tính nhất quán.

3. **Phân quyền:**
   - Phân quyền cho các thành viên trong nhóm với quyền đọc, chỉnh sửa hoặc quản lý tài liệu phù hợp với vai trò.

4. **Tích hợp Confluence với Jira:**
   - Liên kết tài liệu trên Confluence với nhiệm vụ trên Jira để dễ dàng cập nhật và theo dõi tài liệu.

---

## 5. Slack - Communication & Collaboration

**Tổng quan:**  
Slack cung cấp nền tảng giao tiếp trực tuyến, hỗ trợ nhóm trao đổi nhanh chóng, nhận thông báo từ các công cụ và tăng cường hiệu quả làm việc nhóm.

**Phạm vi công việc:**

1. **Đăng ký và thiết lập workspace trên Slack:**
   - Đăng ký tài khoản Slack và tạo workspace cho dự án Gotik.
   - Mời các thành viên vào workspace, sử dụng email có tên miền `@gotik.vn`.

2. **Tạo và quản lý các kênh giao tiếp:**
   - Tạo các kênh như `#general`, `#dev`, ~~`#qa`~~, `#management` cho các cuộc trao đổi theo nhóm và nhiệm vụ.
   - **Hướng dẫn giao tiếp:** Khuyến khích sử dụng thread cho các chủ đề thảo luận riêng trong từng kênh để giảm thiểu nhiễu thông tin.

3. **Tích hợp Slack với các công cụ khác:**
   - Tích hợp Slack với Jira, Bitbucket, và Google Calendar để thông báo tự động khi có thay đổi hoặc sự kiện.
   - **Thông báo tự động:** Thiết lập thông báo định kỳ và tích hợp nhắc nhở cuộc họp tự động.

4. **Thiết lập bot hỗ trợ họp tự động (optional):**
   - Cấu hình bot để thực hiện báo cáo công việc hàng ngày cho nhóm, giúp nhóm duy trì tiến độ (tùy chọn).
