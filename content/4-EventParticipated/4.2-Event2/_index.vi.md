---
title: "Báo cáo sự kiện: AI/ML/GenAI on AWS"
date: "`r Sys.Date()`"
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---
# Báo cáo tổng hợp: “Hội thảo AI/ML/GenAI on AWS”

### Mục tiêu sự kiện

- Có cái nhìn tổng quan về bối cảnh AI/ML tại thị trường Việt Nam.
- Hiểu về khả năng Machine Learning toàn diện (end-to-end) của Amazon SageMaker.
- Đi sâu vào Generative AI với Amazon Bedrock (Foundation Models, Agents, Guardrails).
- Học cách triển khai thực tế thông qua các bài demo trực tiếp trên SageMaker Studio và Bedrock.

### Diễn giả

- **Đội ngũ Kiến trúc sư Giải pháp AWS** (AWS Solutions Architects - Vietnam)

### Nội dung chính (Highlights)

#### Tổng quan về AWS AI/ML Services (Amazon SageMaker)
- **Nền tảng toàn diện:** SageMaker cung cấp một giao diện thống nhất cho toàn bộ vòng đời ML, từ chuẩn bị và gán nhãn dữ liệu đến xây dựng, huấn luyện, tinh chỉnh và triển khai mô hình.
- **Tích hợp MLOps:** Nhấn mạnh tầm quan trọng của các tính năng MLOps tích hợp sẵn trong SageMaker giúp chuẩn hóa quy trình vận hành và đảm bảo tính tái lập của mô hình.
- **SageMaker Studio:** Demo trực tiếp cho thấy cách quản lý quy trình ML một cách trực quan, giúp cả Data Scientist và Developer đều dễ dàng tiếp cận.

#### Generative AI với Amazon Bedrock
- **Lựa chọn Foundation Models (FMs):** So sánh các mô hình khác nhau có sẵn trên Bedrock (Claude, Llama, Titan) và hướng dẫn chọn mô hình phù hợp cho từng trường hợp sử dụng (tốc độ, độ chính xác, chi phí).
- **Kỹ thuật Prompt Engineering:** Các phương pháp cải thiện đầu ra của mô hình, bao gồm tư duy chuỗi (Chain-of-Thought) và học từ vài mẫu (Few-shot learning).
- **RAG (Retrieval-Augmented Generation):** Giải thích kiến trúc kết nối FMs với cơ sở tri thức nội bộ để giảm thiểu ảo giác (hallucinations) và cung cấp câu trả lời chính xác theo ngữ cảnh doanh nghiệp.
- **Agents & Guardrails:** Cách sử dụng Agents cho các tác vụ đa bước và Guardrails để đảm bảo an toàn nội dung.

### Bài học rút ra (Key Takeaways)

#### Đơn giản hóa quy trình ML
- **SageMaker** giúp giảm đáng kể gánh nặng vận hành hạ tầng ML, cho phép team tập trung vào logic của mô hình thay vì việc bảo trì máy chủ.

#### Phổ cập hóa GenAI
- **Amazon Bedrock** mang lại trải nghiệm serverless để truy cập các mô hình Foundation hàng đầu chỉ qua một API, loại bỏ nhu cầu quản lý hạ tầng GPU phức tạp.
- **RAG là cốt lõi:** Đối với ứng dụng doanh nghiệp, RAG là mẫu thiết kế (pattern) quan trọng nhất để biến GenAI thành công cụ hữu ích và đáng tin cậy.

### Ứng dụng vào công việc

- **Khám phá SageMaker Canvas:** Thử nghiệm các tính năng low-code của SageMaker để tạo nhanh các mô hình dự đoán từ dữ liệu bảng.
- **Xây dựng Prototype RAG:** Sử dụng Amazon Bedrock để dựng một chatbot hỏi đáp đơn giản kết nối với tài liệu nội bộ (ví dụ: hướng dẫn thực tập hoặc tài liệu dự án).
- **Luyện tập Prompt Engineering:** Áp dụng kỹ thuật "Chain-of-Thought" để cải thiện chất lượng khi nhờ AI viết code hoặc tài liệu.

### Trải nghiệm sự kiện

Buổi workshop **"AI/ML/GenAI on AWS"** là một phiên làm việc cường độ cao và mang tính thực tiễn rất lớn.

#### Tập trung vào thực hành
Khác với các buổi hội thảo lý thuyết, workshop này tập trung nhiều vào **Live Demo**. Việc tận mắt thấy một GenAI chatbot được xây dựng từ con số 0 bằng Bedrock Agents giúp tôi hình dung rõ ràng cách các thành phần (FMs, Knowledge Bases, Action Groups) kết hợp với nhau.

#### Bộ công cụ toàn diện
Tôi nhận ra AWS có công cụ cho mọi giai đoạn của hành trình AI. Dù là ML truyền thống (SageMaker) hay GenAI tiên tiến (Bedrock), hệ sinh thái đều được tích hợp rất chặt chẽ.

#### Kết nối (Networking)
Phần "Ice-breaker" và giao lưu đầu giờ giúp tôi kết nối với các lập trình viên và sinh viên khác cùng quan tâm đến AI, mang lại góc nhìn rộng hơn về cách AI đang được áp dụng tại Việt Nam.

#### Một số hình ảnh tại sự kiện
*Thêm ảnh sự kiện của bạn vào đây*

> Tổng kết lại, buổi workshop đã giải mã những thuật ngữ phức tạp về GenAI và cung cấp một lộ trình kỹ thuật rõ ràng để xây dựng ứng dụng AI trên AWS.