---
title: "Báo cáo công việc Tuần 8"
date: "2025-10-27"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu Tuần 8:

* Hiểu về văn hóa DevOps và khái niệm Tích hợp liên tục/Triển khai liên tục (CI/CD).
* Làm quen với bộ công cụ AWS Developer Tools (CodeCommit, CodeBuild, CodeDeploy, CodePipeline).
* Xây dựng một pipeline tự động hoàn toàn để triển khai thay đổi code lên EC2.

### Các nhiệm vụ thực hiện trong tuần:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Giới thiệu về CI/CD pipelines.<br>- Tạo Git repository trên AWS CodeCommit (hoặc kết nối GitHub).<br>- Push source code web mẫu lên repository. | 27/10/2025 | 27/10/2025 | <https://docs.aws.amazon.com/codecommit/> |
| 3 | - Cấu hình AWS CodeBuild:<br>- Tạo file `buildspec.yml` để định nghĩa lệnh build (ví dụ: cài dependencies, chạy test).<br>- Chạy thử một bản build thủ công. | 28/10/2025 | 28/10/2025 | <https://docs.aws.amazon.com/codebuild/> |
| 4 | - Cấu hình AWS CodeDeploy:<br>- Tạo file `appspec.yml` để định nghĩa hướng dẫn deploy.<br>- Cài đặt CodeDeploy Agent trên EC2 đích. | 29/10/2025 | 29/10/2025 | <https://docs.aws.amazon.com/codedeploy/> |
| 5 | - **Tích hợp:** Tạo Pipeline trong AWS CodePipeline.<br>- Liên kết các giai đoạn: Source (CodeCommit) -> Build (CodeBuild) -> Deploy (CodeDeploy). | 30/10/2025 | 30/10/2025 | <https://docs.aws.amazon.com/codepipeline/> |
| 6 | - **Kiểm thử:** Push một thay đổi code (ví dụ: đổi text trang web) lên repo.<br>- Quan sát pipeline tự động kích hoạt và cập nhật server mà không cần can thiệp thủ công. | 31/10/2025 | 31/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được trong Tuần 8:

* Có được hiểu biết thực tế về quy trình làm việc CI/CD trên AWS.
* Thiết lập thành công kho quản lý mã nguồn sử dụng AWS CodeCommit.
* Tự động hóa quy trình build bằng CodeBuild và deploy bằng CodeDeploy.
* Xây dựng một pipeline CI/CD hoàn chỉnh bằng AWS CodePipeline.
* Giảm đáng kể thời gian triển khai và lỗi do con người nhờ tự động hóa quy trình release.