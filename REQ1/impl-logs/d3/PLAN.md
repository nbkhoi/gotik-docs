# Ngày 2

>
> - **Mục tiêu:**
>   - Thiết lập Bitbucket Pipelines để hỗ trợ quy trình CI/CD an toàn và hiệu quả. 
>   - Đảm bảo các cấu hình bảo mật trên Bitbucket, Jira, và Confluence đáp ứng các yêu cầu về an toàn dữ liệu và quyền truy cập.
> - **Definition of Done:**
>   - Bitbucket Pipelines đã được cấu hình và chạy thành công trên nhánh `develop` cũng như các nhánh `feature/*`.
>   - Cấu hình bảo mật trên Bitbucket, Jira, và Confluence đã được kiểm tra và đảm bảo an toàn.
>   - Thực hiện thử nghiệm CI/CD bằng cách commit và push mã nguồn mới lên nhánh `feature/*`.
>   - Thực hiện thử nghiệm CI/CD bằng cách tạo pull request và merge vào nhánh `develop`.

# 1. Bitbucket Pipelines - CI/CD

## 1.1 Prerequisites

- [x] **Chuẩn bị thông tin cần thiết**:
  - [x] Tài khoản Bitbucket đã được kích hoạt.
  - [x] Tài khoản Bitbucket của thành viên đã được mời vào tổ chức.

## 1.2 Action checklist

- [x] **1. Chuẩn bị source code mẫu:**
  - [x] Clone repository từ Bitbucket về máy local.
  - [x] Tạo branch `develop` và `feature/branch-name` để thực hiện thử nghiệm CI/CD.
  - [x] Chuẩn bị Spring Boot project mẫu để thực hiện CI/CD.
  - [x] Commit và push mã nguồn lên Bitbucket.

- [x] **2. Cấu hình Bitbucket Pipelines:**
  - [x] Tạo file `bitbucket-pipelines.yml` trong thư mục gốc của repository.
  - [x] Cấu hình pipeline cho các bước build, test. `// deploy để lại cho giai đoạn sau`
  - [x] Commit và push file cấu hình lên Bitbucket.
  - [x] Kiểm tra pipeline chạy thành công trên nhánh `feature/branch-name`.
  - [x]Tạo pull request từ `feature/branch-name` vào `develop`.
  - [x] Merge nhánh `feature/branch-name` vào `develop`.
  - [x] Kiểm tra pipeline chạy thành công trên nhánh `develop`.