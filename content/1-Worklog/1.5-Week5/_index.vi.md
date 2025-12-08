---
title: "Báo cáo công việc Tuần 5"
date: "2025-10-06"
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Mục tiêu Tuần 5:

* Nắm vững các khái niệm về Quản lý Định danh và Truy cập (IAM).
* Triển khai "Nguyên tắc đặc quyền tối thiểu" (Principle of Least Privilege) cho người dùng và dịch vụ.
* Bảo mật tài nguyên AWS bằng cách sử dụng IAM Roles thay vì lưu trữ key dài hạn.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Học các thành phần cốt lõi IAM: Users, Groups, Policies (Cấu trúc JSON).<br>- **Thực hành:** Tạo IAM Groups (Dev, Admin) và gán các managed policies. | 06/10/2025 | 06/10/2025 | <https://docs.aws.amazon.com/iam/> |
| 3 | - Tìm hiểu về IAM Roles và Service-Linked Roles.<br>- **Kịch bản:** Tạo một IAM Role cho phép EC2 truy cập S3 buckets (Read/Write) mà không cần Access Keys. | 07/10/2025 | 07/10/2025 | <https://docs.aws.amazon.com/iam/> |
| 4 | - **Thực hành:** Gắn IAM Role đã tạo vào một EC2 instance đang chạy.<br>- SSH vào EC2 và kiểm tra quyền truy cập S3 qua AWS CLI (`aws s3 ls`). | 08/10/2025 | 08/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Tăng cường bảo mật tài khoản:<br>- Bật MFA (Multi-Factor Authentication) cho tài khoản Root và IAM users.<br>- Cấu hình Password Policy (độ dài, độ phức tạp). | 09/10/2025 | 09/10/2025 | <https://docs.aws.amazon.com/iam/> |
| 6 | - Ôn tập Mô hình Trách nhiệm chung (Shared Responsibility Model).<br>- Khám phá AWS CloudTrail để kiểm toán các lệnh gọi API (ai đã làm gì, khi nào). | 10/10/2025 | 10/10/2025 | <https://aws.amazon.com/compliance/shared-responsibility-model/> |

### Kết quả đạt được trong Tuần 5:

* Hiểu sâu về Mô hình Trách nhiệm chung của AWS và logic hoạt động của IAM.
* Triển khai các ranh giới phân quyền chặt chẽ bằng cách sử dụng IAM Policies và Groups.
* Thay thế thành công việc sử dụng hard-coded credentials (Access/Secret Keys) bằng IAM Roles an toàn hơn cho việc truy cập dịch vụ từ EC2.
* Nâng cao bảo mật tài khoản bằng cách bắt buộc sử dụng MFA và chính sách mật khẩu mạnh.
* Xác minh giao tiếp an toàn giữa các dịch vụ (EC2 gọi sang S3) mà không để lộ thông tin xác thực.