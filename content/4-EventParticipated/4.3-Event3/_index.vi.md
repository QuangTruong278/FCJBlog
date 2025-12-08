---
title: "Báo cáo sự kiện: DevOps on AWS"
date: "`r Sys.Date()`"
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---
# Báo cáo tổng hợp: “Hội thảo DevOps on AWS”

### Mục tiêu sự kiện

- Hiểu về văn hóa DevOps, các nguyên tắc cốt lõi và các chỉ số đo lường hiệu quả (DORA metrics).
- Làm chủ bộ công cụ AWS Developer Tools để xây dựng quy trình CI/CD tự động.
- Học về Cơ sở hạ tầng dưới dạng mã (IaC) sử dụng AWS CloudFormation và CDK.
- Khám phá các dịch vụ Container (ECS, EKS, App Runner) và công cụ giám sát (CloudWatch, X-Ray).

### Diễn giả

- **Đội ngũ Kiến trúc sư Giải pháp AWS** (AWS Solutions Architects - Vietnam)

### Nội dung chính (Highlights)

#### Tư duy DevOps & Dịch vụ CI/CD
- **Chỉ số đo lường:** Mở đầu bằng tầm quan trọng của các chỉ số DORA (Tần suất triển khai, Thời gian phục hồi, v.v.) để đánh giá độ trưởng thành của DevOps.
- **Tự động hóa Pipeline:** Đi sâu vào quy trình đầy đủ:
    - **Source:** CodeCommit & chiến lược Git (Trunk-based vs GitFlow).
    - **Build & Test:** Sử dụng CodeBuild để biên dịch và chạy unit tests.
    - **Deploy:** Các chiến lược Blue/Green và Canary với CodeDeploy để giảm thiểu thời gian chết (downtime).
    - **Điều phối:** Kết nối mọi thứ bằng CodePipeline.

#### Cơ sở hạ tầng dưới dạng mã (IaC)
- **CloudFormation vs CDK:** So sánh rõ ràng giữa việc định nghĩa hạ tầng bằng template JSON/YAML (CloudFormation) và sử dụng ngôn ngữ lập trình quen thuộc như TypeScript/Python (CDK).
- **Phát hiện sai lệch (Drift Detection):** Cách phát hiện khi hạ tầng thực tế bị thay đổi so với định nghĩa trong mã.

#### Dịch vụ Container
- **Lựa chọn công cụ:** Hướng dẫn khi nào nên dùng **Amazon ECS** (đơn giản, chuẩn AWS), **Amazon EKS** (chuẩn Kubernetes) hay **App Runner** (quản lý hoàn toàn/đơn giản nhất).
- **Registry:** Sử dụng Amazon ECR để lưu trữ image an toàn và quét lỗ hổng bảo mật.

#### Giám sát & Khả năng quan sát (Observability)
- **Tầm nhìn toàn diện (Full-stack):** Không chỉ là logs. Đó là sự kết hợp giữa Metrics, Logs và Traces (dùng AWS X-Ray) để gỡ lỗi hiệu quả cho các microservices phân tán.

### Bài học rút ra (Key Takeaways)

#### Tự động hóa là then chốt
- Triển khai thủ công rất dễ gây lỗi. Mục tiêu là tự động hóa mọi thứ từ cấp phát hạ tầng (IaC) đến triển khai mã nguồn (CI/CD).

#### Hạ tầng bất biến (Immutable Infrastructure)
- Qua phần Container, tôi hiểu giá trị của hạ tầng bất biến—đóng gói ứng dụng và dependencies vào Docker container đảm bảo nó chạy giống hệt nhau ở mọi môi trường.

#### Shift Left
- Kiểm thử và quét bảo mật nên được thực hiện sớm trong pipeline (tại bước CodeBuild/ECR), chứ không phải đợi sau khi đã deploy.

### Ứng dụng vào công việc

- **Cải tiến Pipeline:** Tôi sẽ thử áp dụng chiến lược deploy "Blue/Green" cho dự án thực tập hiện tại bằng CodeDeploy để đảm bảo zero downtime.
- **Thử nghiệm AWS CDK:** Thay vì thao tác trên console, tôi sẽ viết script CDK để khởi tạo VPC và EC2 cho bài tập tiếp theo.
- **Kích hoạt X-Ray:** Tôi dự định gắn AWS X-Ray vào ứng dụng để trực quan hóa bản đồ dịch vụ (service maps) và tìm điểm nghẽn về độ trễ.

### Trải nghiệm sự kiện

Hội thảo **"DevOps on AWS"** kéo dài cả ngày mang lại kiến thức rất toàn diện và xâu chuỗi được nhiều vấn đề.

#### Từ lý thuyết đến thực hành
Sự chuyển tiếp từ lý thuyết **DevOps Mindset** buổi sáng sang thực hành cấu hình **CI/CD Pipeline** giúp tôi hiểu rõ *tại sao* cần dùng những công cụ này, chứ không chỉ là *làm thế nào*.

#### Sự rõ ràng về Container
Tôi từng khá bối rối giữa ECS và EKS. Phần phân tích buổi chiều giúp tôi hiểu rõ: ECS dành cho sự điều phối "theo chuẩn AWS" còn EKS dành cho "chuẩn Kubernetes".

#### Demo trực quan
Phần demo về **Full-stack observability** sử dụng CloudWatch và X-Ray thực sự mở mang tầm mắt. Việc nhìn thấy một request được truy vết từ Load Balancer xuống tận câu lệnh Database cho thấy sức mạnh của việc giám sát hiện đại.

#### Một số hình ảnh tại sự kiện
![](Hinh1.jpg) ![](Hinh2.jpg) ![](Hinh3.jpg) ![](Hinh4.jpg) ![](Hinh5.jpg)

> Tổng kết lại, sự kiện này đã trang bị bộ công cụ thiết yếu cho một Kỹ sư Cloud hiện đại: CI/CD, IaC, Containers và Monitoring.