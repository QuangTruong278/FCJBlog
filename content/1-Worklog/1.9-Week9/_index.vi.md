---
title: "Báo cáo công việc Tuần 9"
date: "2025-11-03"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---
### Mục tiêu Tuần 9:

* Hiểu về công nghệ Containerization và Docker.
* Học cách viết Dockerfile để đóng gói ứng dụng.
* Sử dụng Amazon Elastic Container Registry (ECR) để lưu trữ và quản lý Docker images.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Giới thiệu về Containers so với Máy ảo (VM).<br>- Cài đặt Docker Engine trên EC2 instance (hoặc máy cá nhân).<br>- Học các lệnh Docker cơ bản (`run`, `ps`, `images`, `stop`). | 03/11/2025 | 03/11/2025 | <https://docs.docker.com/get-started/> |
| 3 | - **Thực hành:** Viết `Dockerfile` cho một ứng dụng web đơn giản (Python/Node.js).<br>- Build Docker image trên máy local. | 04/11/2025 | 04/11/2025 | <https://docs.docker.com/engine/reference/builder/> |
| 4 | - Giới thiệu về Amazon ECR.<br>- Tạo một private repository trong Amazon ECR.<br>- Cấu hình AWS CLI để xác thực Docker với ECR. | 05/11/2025 | 05/11/2025 | <https://docs.aws.amazon.com/AmazonECR/> |
| 5 | - **Thực hành:** Gắn thẻ (Tag) cho Docker image và đẩy (Push) lên Amazon ECR repository.<br>- Kiểm tra image trên AWS Console. | 06/11/2025 | 06/11/2025 | <https://docs.aws.amazon.com/AmazonECR/> |
| 6 | - **Triển khai:** Khởi chạy một EC2 instance mới.<br>- Kéo (Pull) image từ ECR về và chạy container.<br>- Kiểm tra ứng dụng hoạt động bình thường. | 07/11/2025 | 07/11/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 9:

* Hiểu rõ lợi ích của container hóa so với ảo hóa truyền thống.
* Đóng gói thành công ứng dụng cũ bằng Docker (viết Dockerfile tối ưu).
* Nắm vững quy trình build, tag và push image lên registry.
* Sử dụng Amazon ECR làm nơi lưu trữ Docker image an toàn và riêng tư.
* Triển khai ứng dụng từ container image, đảm bảo tính nhất quán giữa các môi trường.