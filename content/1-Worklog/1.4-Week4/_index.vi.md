---
title: "Báo cáo công việc Tuần 4"
date: "2025-09-29"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
### Mục tiêu Tuần 4:

* Triển khai tính sẵn sàng cao (High Availability - HA) và khả năng mở rộng (Scalability) cho ứng dụng web.
* Làm chủ cấu hình Application Load Balancer (ALB) và Auto Scaling Group (ASG).
* Thực hiện stress test để kiểm chứng khả năng tự động mở rộng.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Tìm hiểu các loại Elastic Load Balancing (ELB): ALB vs NLB.<br>- Tạo Target Groups và đăng ký targets.<br>- **Thực hành:** Tạo một Application Load Balancer. | 29/09/2025 | 29/09/2025 | <https://docs.aws.amazon.com/elasticloadbalancing/> |
| 3 | - Hiểu về Amazon Machine Image (AMI).<br>- **Thực hành:** Tạo AMI tùy chỉnh từ Web Server (EC2) đã tạo ở Tuần 3 (đã cài sẵn LAMP stack). | 30/09/2025 | 30/09/2025 | <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html> |
| 4 | - Học về Launch Templates và Auto Scaling Groups (ASG).<br>- Cấu hình Scaling Policies (ví dụ: Target Tracking Scaling khi CPU > 50%). | 01/10/2025 | 01/10/2025 | <https://docs.aws.amazon.com/autoscaling/> |
| 5 | - **Tích hợp:** Gắn Auto Scaling Group vào Application Load Balancer.<br>- Đảm bảo cấu hình Health Check chính xác. | 02/10/2025 | 02/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Stress Test:** Giả lập lượng truy cập lớn vào ALB DNS.<br>- Quan sát EC2 instances tự động scale out (thêm máy mới).<br>- Kiểm chứng khả năng "Self-healing" bằng cách tắt thủ công một instance. | 03/10/2025 | 03/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 4:

* Tạo thành công một AMI (Amazon Machine Image) tùy chỉnh để triển khai ứng dụng nhanh chóng.
* Thiết kế và xây dựng kiến trúc có tính sẵn sàng cao sử dụng Application Load Balancer (ALB) để phân phối tải.
* Cấu hình Auto Scaling Group (ASG) đảm bảo ứng dụng có thể chịu được các mức tải khác nhau.
* Kiểm chứng tính đàn hồi (elasticity) của hệ thống:
    * **Scale-out:** Tự động thêm server khi CPU tăng cao.
    * **High Availability:** Tự động thay thế các server bị lỗi hoặc bị tắt.