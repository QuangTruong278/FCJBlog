---
title: "Báo cáo công việc Tuần 10"
date: "2025-11-10"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---
### Mục tiêu Tuần 10:

* Khám phá điện toán Serverless và kiến trúc hướng sự kiện (Event-driven).
* Xây dựng một RESTful API sử dụng Amazon API Gateway và AWS Lambda.
* Tích hợp các hàm Serverless với các dịch vụ AWS khác (như SES từ Tuần 6).

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Giới thiệu về Serverless: Các khái niệm AWS Lambda (Triggers, Runtimes, Layers).<br>- **Thực hành:** Tạo hàm Lambda "Hello World" đơn giản (Python/Node.js). | 10/11/2025 | 10/11/2025 | <https://docs.aws.amazon.com/lambda/> |
| 3 | - Test Lambda với các event test tùy chỉnh trong Console.<br>- Tìm hiểu về IAM Roles cho Lambda (Execution Role). | 11/11/2025 | 11/11/2025 | <https://docs.aws.amazon.com/lambda/> |
| 4 | - Giới thiệu về Amazon API Gateway.<br>- **Thực hành:** Tạo một REST API.<br>- Tạo Resources và Methods (GET/POST). | 12/11/2025 | 12/11/2025 | <https://docs.aws.amazon.com/apigateway/> |
| 5 | - **Tích hợp:** Kết nối API Gateway với hàm Lambda (Lambda Proxy Integration).<br>- Triển khai (Deploy) API ra một Stage (dev/prod). | 13/11/2025 | 13/11/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Thực hành nâng cao:** Chuyển đổi script gửi email (Tuần 6) lên chạy trên Lambda.<br>- Kích hoạt hàm Lambda thông qua việc gọi API để gửi email tự động. | 14/11/2025 | 14/11/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 10:

* Triển khai code thành công mà không cần khởi tạo hay quản lý máy chủ (Serverless).
* Tạo được một API public endpoint có khả năng mở rộng bằng Amazon API Gateway.
* Kết hợp Serverless (Lambda) với SES để tạo hệ thống thông báo email hướng sự kiện.
* Hiểu rõ lợi ích chi phí của mô hình "Dùng bao nhiêu trả bấy nhiêu" trong Serverless.