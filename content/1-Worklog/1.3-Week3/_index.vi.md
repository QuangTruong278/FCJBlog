---
title: "Báo cáo công việc Tuần 3"
date: "2025-09-22"
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---
### Mục tiêu Tuần 3:

* Tìm hiểu về Cơ sở dữ liệu quan hệ được quản lý trên AWS (Amazon RDS).
* Cấu hình bảo mật mạng giữa Compute (EC2) và Database (RDS).
* Triển khai một ứng dụng web động đơn giản kết nối với cơ sở dữ liệu.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Học các khái niệm RDS (Multi-AZ, Read Replicas, Backups, Maintenance Window).<br>- **Thực hành:** Tạo một MySQL RDS instance (Free Tier). | 22/09/2025 | 22/09/2025 | <https://docs.aws.amazon.com/rds/> |
| 3 | - Cấu hình Security Groups: Cho phép lưu lượng từ EC2 Security Group vào RDS Security Group trên cổng 3306.<br>- Tìm hiểu về RDS endpoints. | 23/09/2025 | 23/09/2025 | <https://docs.aws.amazon.com/rds/> |
| 4 | - Cài đặt LAMP stack (Linux, Apache, MySQL/MariaDB, PHP) trên một EC2 instance.<br>- Chuẩn bị một script PHP kết nối mẫu. | 24/09/2025 | 24/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Thực hành:** Kết nối ứng dụng PHP trên EC2 tới RDS endpoint.<br>- Xử lý sự cố kết nối (Troubleshoot VPC, Subnets, SG). | 25/09/2025 | 25/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Tìm hiểu về RDS Snapshots (Manual vs Automated).<br>- **Thực hành:** Tạo snapshot thủ công và khôi phục (restore) ra một DB instance mới. | 26/09/2025 | 26/09/2025 | <https://docs.aws.amazon.com/rds/> |

### Kết quả đạt được trong Tuần 3:

* Khởi tạo thành công một cơ sở dữ liệu MySQL được quản lý hoàn toàn bằng Amazon RDS.
* Thực hiện các biện pháp bảo mật tốt nhất bằng cách chỉ giới hạn quyền truy cập cơ sở dữ liệu cho Web Server (EC2) thông qua Security Group.
* Triển khai thành công ứng dụng web động (LAMP stack) trên EC2.
* Thiết lập kết nối thành công giữa Tầng Ứng dụng (App Tier) và Tầng Dữ liệu (Data Tier).
* Thực hiện các thao tác sao lưu và khôi phục cơ sở dữ liệu bằng RDS Snapshots.