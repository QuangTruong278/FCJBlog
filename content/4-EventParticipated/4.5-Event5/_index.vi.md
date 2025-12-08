---
title: "Báo cáo sự kiện: Agentic AI Journey"
date: "`r Sys.Date()`"
weight: 6
chapter: false
pre: " <b> 4.6. </b> "
---
# Báo cáo tổng hợp: “Agentic AI: Từ Kiến trúc đến Triển khai”

### Mục tiêu sự kiện

- Hiểu các khái niệm cốt lõi của Agentic AI (AI hành động) và AWS Bedrock Agents.
- Khám phá các trường hợp sử dụng thực tế (Use Cases) để xây dựng luồng công việc tự động (Agentic Workflow).
- Đi sâu vào kỹ thuật Điều phối Agent và Tối ưu hóa ngữ cảnh (mức độ chuyên sâu L300).
- Trải nghiệm thực hành: Xây dựng một Agent sử dụng CloudThinker và AWS Bedrock.

### Diễn giả

- **Nguyễn Gia Hưng** – Trưởng bộ phận Kiến trúc sư Giải pháp
- **Kiên Nguyễn** – Kiến trúc sư Giải pháp (AWS)
- **Việt Phạm** – Founder & CEO
- **Thắng Tôn** – Co-founder & COO (CloudThinker)
- **Henry Bùi** – Giám đốc Kỹ thuật (CloudThinker)
- **Kha Vân** – Technical Lead/Người hướng dẫn

### Nội dung chính (Highlights)

#### AWS Bedrock Agent Core
- **Khái niệm:** Chuyển dịch từ các "Chatbot" thụ động sang các "Agent" chủ động có khả năng thực thi các tác vụ đa bước.
- **Thành phần:** Giải phẫu cấu trúc của một Agent: Foundation Model (Bộ não) + Action Groups (Công cụ/API) + Knowledge Bases (RAG).
- **Cơ chế:** Cách Bedrock Agents chia nhỏ một yêu cầu phức tạp của người dùng thành chuỗi các bước logic (Chain-of-Thought) và thực thi chúng qua Lambda functions.

#### Ứng dụng thực tế & CloudThinker
- **Use Cases:** Tạo ra các quy trình nơi AI tự động xử lý công việc kinh doanh (đặt lịch, xử lý đơn hàng, phân tích dữ liệu) mà không cần con người can thiệp.
- **Điều phối (L300 Deep Dive):** Anh Henry Bùi chia sẻ các kỹ thuật nâng cao về quản lý tương tác phức tạp giữa các agent. Trọng tâm là **Tối ưu hóa ngữ cảnh (Context Optimization)**—đảm bảo AI giữ được thông tin quan trọng trong các hội thoại dài mà không bị tràn bộ nhớ (token limits) hoặc mất tập trung.
- **Nền tảng CloudThinker:** Giới thiệu framework chuyên dụng giúp đơn giản hóa việc điều phối các luồng agent phức tạp trên nền tảng AWS.

#### Workshop thực hành: CloudThinker Hack
- **Thực chiến:** Dưới sự hướng dẫn của anh Kha Vân, người tham dự đã thiết lập môi trường và triển khai một agent hoạt động thực tế.
- **Tích hợp:** Kết nối agent với các công cụ bên ngoài và quan sát cách nó suy luận để giải quyết vấn đề theo thời gian thực.

### Bài học rút ra (Key Takeaways)

#### Bước chuyển mình sang "Agency"
- Tương lai của AI không chỉ là tạo sinh văn bản, mà là hành động. "Agentic AI" là biên giới tiếp theo nơi các mô hình trở thành người ra quyết định.

#### Ngữ cảnh là Vua (Context is King)
- Trong các luồng công việc phức tạp, quản lý "Trạng thái" (State) và "Ngữ cảnh" là thách thức lớn nhất. Các kỹ thuật tối ưu hóa (như tóm tắt ngữ cảnh hoặc lưu giữ chọn lọc) là yếu tố sống còn cho các agent chạy production.

#### Sự phức tạp trong điều phối
- Xây dựng một agent thì dễ; làm cho nhiều agent phối hợp nhịp nhàng đòi hỏi một lớp điều phối mạnh mẽ (điều mà các công cụ như CloudThinker giải quyết).

### Ứng dụng vào công việc

- **Thử nghiệm Action Groups:** Tôi sẽ thử thêm một "Action Group" đơn giản vào dự án Bedrock của mình (ví dụ: Lambda function truy vấn database) để biến chatbot hiện tại thành một basic agent.
- **Nghiên cứu quản lý ngữ cảnh:** Tìm hiểu sâu hơn về cách tối ưu context cho các tác vụ dài hơi, dựa trên kiến thức từ phiên L300.
- **Kiểm thử hành vi Agent:** Áp dụng tư duy kiểm thử để đánh giá xem agent có thực hiện đúng hành động (action) hay không trước khi deploy.

### Trải nghiệm sự kiện

Sự kiện **"Agentic AI"** là sự kết hợp hoàn hảo giữa lý thuyết và thực hành.

#### Chiều sâu kỹ thuật (L300)
Tôi đặc biệt đánh giá cao phiên chia sẻ **L300** của anh Henry Bùi. Thông thường các sự kiện chỉ dừng ở mức tổng quan, nhưng phiên này đi sâu vào thách thức kỹ thuật của việc tối ưu hóa Context, mang lại kiến thức kiến trúc rất giá trị.

#### Phần "Hack" thực tế
Phiên thực hành cuối giờ rất năng lượng và hữu ích. Việc nhìn thấy agent do mình cấu hình thực sự thực thi một tác vụ (thay vì chỉ trả lời bằng chữ) là một khoảnh khắc "vỡ lẽ" về sức mạnh của hệ sinh thái Bedrock.

#### Networking
Thời gian ăn trưa và giao lưu giúp tôi có cơ hội thảo luận với đội ngũ CloudThinker về vấn đề độ trễ (latency) trong các luồng agent, thu được nhiều mẹo thực tế cho dự án cá nhân.

#### Một số hình ảnh tại sự kiện
*Thêm ảnh sự kiện của bạn vào đây*

> Tổng kết lại, sự kiện đã thu hẹp khoảng cách giữa "sự hào nhoáng" về AI Agents và "cách làm" thực tế để xây dựng chúng trên AWS.