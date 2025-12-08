---
title: "Báo cáo công việc Tuần 7"
date: "2025-10-20"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---
### Mục tiêu Tuần 7:

* Chuyển đổi từ cấu hình thủ công ("ClickOps") sang Hạ tầng dưới dạng mã (IaC).
* Học các kiến thức cơ bản về Terraform: Providers, Resources, Variables, và State.
* Tự động hóa việc khởi tạo tài nguyên VPC và EC2 bằng Terraform.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Giới thiệu về khái niệm IaC.<br>- Cài đặt Terraform và cấu hình AWS credentials trên máy cá nhân.<br>- Học cú pháp HCL (HashiCorp Configuration Language). | 20/10/2025 | 20/10/2025 | <https://developer.hashicorp.com/terraform/intro> |
| 3 | - **Coding:** Viết file `vpc.tf` để tạo VPC, Subnet, Internet Gateway, và Route Table.<br>- Tìm hiểu về Terraform Providers (`aws`). | 21/10/2025 | 21/10/2025 | <https://registry.terraform.io/providers/hashicorp/aws/latest/docs> |
| 4 | - **Coding:** Viết file `main.tf` để khởi chạy EC2 instance bên trong VPC đã tạo.<br>- Sử dụng `variables.tf` để tham số hóa các giá trị (Region, AMI ID, Instance Type). | 22/10/2025 | 22/10/2025 | <https://developer.hashicorp.com/terraform/language> |
| 5 | - Hiểu quy trình làm việc Terraform: `init`, `plan`, `apply`, `destroy`.<br>- Tìm hiểu về `terraform.tfstate` và cách quản lý file trạng thái. | 23/10/2025 | 23/10/2025 | <https://developer.hashicorp.com/terraform/cli/commands> |
| 6 | - **Mini-Project:** Tái tạo kiến trúc Tuần 2 (VPC + EC2) hoàn toàn bằng mã Terraform.<br>- Kiểm tra việc triển khai qua AWS Console và sau đó hủy tài nguyên chỉ bằng một lệnh. | 24/10/2025 | 24/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 7:

* Chuyển đổi thành công từ thao tác thủ công trên Console sang quản lý hạ tầng bằng mã Terraform.
* Nắm vững quy trình làm việc cốt lõi của Terraform (`init` -> `plan` -> `apply` -> `destroy`).
* Tạo được mã nguồn hạ tầng có khả năng tái sử dụng nhờ Variables.
* Triển khai môi trường VPC và EC2 hoàn chỉnh chỉ trong vài phút bằng một dòng lệnh.
* Hiểu được tầm quan trọng của việc quản lý State (trạng thái) trong IaC.