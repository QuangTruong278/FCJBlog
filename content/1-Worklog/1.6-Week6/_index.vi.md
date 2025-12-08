---
title: "Báo cáo công việc Tuần 6"
date: "2025-10-13"
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu Tuần 6:

* Hiểu về Amazon Simple Email Service (SES) và các trường hợp sử dụng (Giao dịch vs Tiếp thị).
* Xác minh danh tính (Email/Domain) và hiểu về các giới hạn của chế độ Sandbox.
* Gửi email bằng lập trình sử dụng AWS SDK (Boto3 với Python) trên EC2.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Giới thiệu về Amazon SES.<br>- **Thực hành:** Xác minh một Email Identity (Người gửi và Người nhận) trong SES Console.<br>- Tìm hiểu khái niệm chế độ "SES Sandbox". | 13/10/2025 | 13/10/2025 | <https://docs.aws.amazon.com/ses/> |
| 3 | - Cấu hình thông tin xác thực SMTP cho SES.<br>- Tìm hiểu quy trình yêu cầu truy cập Production (thoát khỏi Sandbox). | 14/10/2025 | 14/10/2025 | <https://docs.aws.amazon.com/ses/> |
| 4 | - **Lập trình:** Viết một script Python đơn giản sử dụng thư viện `boto3` để gửi email test thông qua SES API.<br>- Xử lý các ngoại lệ lỗi (ví dụ: MessageRejected). | 15/10/2025 | 15/10/2025 | <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html> |
| 5 | - **Tích hợp:** Triển khai script Python lên một EC2 instance.<br>- Cấu hình IAM Role cho EC2 để cấp quyền `ses:SendEmail` (thay vì dùng SMTP credentials cố định). | 16/10/2025 | 16/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Kiểm thử:** Chạy script trên EC2 để kích hoạt thông báo email tự động.<br>- Giám sát thống kê gửi nhận trong SES Console (Tỷ lệ gửi thành công, Bounce rate). | 17/10/2025 | 17/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 6:

* Cấu hình thành công môi trường Amazon SES và xác minh các danh tính email.
* Hiểu và áp dụng các phương pháp bảo mật tốt nhất bằng cách sử dụng IAM Roles cho EC2 để cấp quyền gửi email.
* Phát triển được script tự động hóa bằng Python sử dụng AWS SDK (Boto3) để tương tác với dịch vụ AWS.
* Tích hợp khả năng thông báo qua email vào hạ tầng, cho phép gửi cảnh báo tự động.