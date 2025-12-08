---
title: "Báo cáo công việc Tuần 2"
date: "2025-09-15"
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---
### Mục tiêu Tuần 2:

* Tìm hiểu sâu về Mạng trong AWS (VPC, Subnet, Route Table, Internet Gateway).
* Hiểu và thực hành dịch vụ lưu trữ AWS Storage Service (S3) và các tính năng (Versioning, Lifecycle, Hosting).
* Triển khai một trang web tĩnh (static website) trên S3.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Học kiến trúc VPC: CIDR, Subnets (Public vs Private), Internet Gateway.<br>- **Thực hành:** Tạo một VPC tùy chỉnh với 1 Public Subnet và 1 Private Subnet. | 15/09/2025 | 15/09/2025 | <https://docs.aws.amazon.com/vpc/> |
| 3 | - Cấu hình Route Tables và Security Groups (Quy tắc Inbound/Outbound).<br>- Khởi tạo EC2 trong Public Subnet và thử kết nối SSH.<br>- Tìm hiểu cơ bản về NAT Gateway. | 16/09/2025 | 16/09/2025 | <https://docs.aws.amazon.com/vpc/> |
| 4 | - Học các khái niệm Amazon S3: Buckets, Objects, Classes (Standard, IA, Glacier).<br>- **Thực hành:** Tạo S3 Buckets thông qua Console và CLI. | 17/09/2025 | 17/09/2025 | <https://docs.aws.amazon.com/s3/> |
| 5 | - Tính năng nâng cao S3: Bật Versioning, Cấu hình Lifecycle Rules.<br>- Tìm hiểu về Bucket Policies và ACLs. | 18/09/2025 | 18/09/2025 | <https://docs.aws.amazon.com/s3/> |
| 6 | - **Mini-Project:** Host một trang web tĩnh trên Amazon S3.<br>- Upload file HTML/CSS.<br>- Cấu hình "Static website hosting" và mở quyền truy cập public. | 19/09/2025 | 19/09/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 2:

* Thiết kế và tạo thành công một Virtual Private Cloud (VPC) tùy chỉnh với phân đoạn mạng chính xác (Public/Private subnets).
* Cấu hình Security Groups để kiểm soát chặt chẽ lưu lượng truy cập (ví dụ: chỉ cho phép SSH từ IP cụ thể).
* Làm chủ các kiến thức cơ bản về Amazon S3:
    * Tạo bucket và quản lý đối tượng bằng cả Console và CLI.
    * Thực hiện bảo vệ dữ liệu bằng Versioning.
    * Tối ưu hóa chi phí bằng Lifecycle policies (chuyển dữ liệu sang Glacier).
* Host thành công một trang web tĩnh sử dụng S3 mà không cần máy chủ.