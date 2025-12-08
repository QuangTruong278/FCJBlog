---
title: "Báo cáo công việc Tuần 11"
date: "2025-11-17"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---
### Mục tiêu Tuần 11:

* Triển khai khả năng quan sát (observability) cho hạ tầng AWS.
* Cấu hình CloudWatch Alarms để phát hiện sự cố chủ động.
* Tập trung logs và trực quan hóa các chỉ số trên Dashboards.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Khám phá các khái niệm Amazon CloudWatch: Namespaces, Metrics, Dimensions.<br>- Kiểm tra các chỉ số EC2 tiêu chuẩn (CPU, Status Checks, Network). | 17/11/2025 | 17/11/2025 | <https://docs.aws.amazon.com/cloudwatch/> |
| 3 | - **Thực hành:** Tạo một CloudWatch Alarm.<br>- Điều kiện: Gửi email thông báo (qua SNS topic) nếu CPU Utilization > 80% trong 5 phút. | 18/11/2025 | 18/11/2025 | <https://docs.aws.amazon.com/cloudwatch/> |
| 4 | - Tìm hiểu về CloudWatch Logs.<br>- Cài đặt và cấu hình Unified CloudWatch Agent trên EC2 để đẩy logs hệ điều hành (syslog/messages) lên CloudWatch. | 19/11/2025 | 19/11/2025 | <https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Install-CloudWatch-Agent.html> |
| 5 | - Cấu hình Custom Metrics: Giám sát dung lượng RAM và Ổ cứng (Disk Space) - các chỉ số không có sẵn mặc định. | 20/11/2025 | 20/11/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Dashboarding:** Tạo một CloudWatch Dashboard tập trung.<br>- Thêm các widget hiển thị CPU, Memory của EC2, lượng gọi API Gateway, và lỗi Lambda. | 21/11/2025 | 21/11/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 11:

* Thiết lập hệ thống giám sát chủ động cho các thành phần hạ tầng quan trọng.
* Cấu hình cảnh báo tự động (Alarms + SNS) giúp giảm thời gian phản hồi sự cố.
* Có được cái nhìn sâu hơn vào hiệu suất nội tại của hệ thống (RAM/Disk) nhờ CloudWatch Agent.
* Xây dựng Dashboard vận hành chuyên nghiệp để trực quan hóa sức khỏe hệ thống theo thời gian thực.