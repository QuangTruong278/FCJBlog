---
title: "Báo cáo sự kiện: AWS Security Pillar"
date: "2025-11-29"
weight: 5
chapter: false
pre: " <b> 4.5. </b> "
---
# Báo cáo tổng hợp: “AWS Well-Architected Security Pillar”

### Mục tiêu sự kiện

- Nắm vững các nguyên tắc cốt lõi của Trụ cột Bảo mật: Đặc quyền tối thiểu (Least Privilege), Zero Trust và Phòng thủ chiều sâu (Defense in Depth).
- Hiểu kiến trúc IAM hiện đại và cách loại bỏ việc sử dụng thông tin xác thực dài hạn (long-term credentials).
- Học cách triển khai các lớp phát hiện và giám sát liên tục (GuardDuty, Security Hub).
- Đi sâu vào bảo vệ Hạ tầng/Dữ liệu và Tự động hóa ứng phó sự cố (Incident Response).

### Diễn giả

- **Đội ngũ Kiến trúc sư Giải pháp AWS** (Chuyên gia Bảo mật)

### Nội dung chính (Highlights)

#### 1. Quản lý Định danh & Truy cập (IAM)
- **Định danh là bức tường lửa mới:** Phiên thảo luận nhấn mạnh việc chuyển dịch từ bảo mật dựa trên mạng sang bảo mật dựa trên định danh.
- **Best Practices:** Tránh dùng IAM User với key dài hạn. Thay vào đó, sử dụng **IAM Identity Center** cho SSO và các thông tin xác thực tạm thời qua Roles.
- **Kiểm soát truy cập:** Sử dụng SCPs (Service Control Policies) để quản trị đa tài khoản và Access Analyzer để kiểm tra chính sách.

#### 2. Phát hiện & Giám sát (Detection)
- **Tầm nhìn tập trung:** Tích hợp CloudTrail (kiểm toán API) và VPC Flow Logs với **AWS Security Hub** để có một giao diện quản lý an ninh duy nhất.
- **Detection-as-Code:** Coi các quy tắc bảo mật và cảnh báo như mã nguồn để đảm bảo tính nhất quán giữa các môi trường.

#### 3. Bảo vệ Hạ tầng & Dữ liệu
- **Phòng thủ chiều sâu (Defense in Depth):** Phân lớp các biện pháp kiểm soát:
    - **Mạng:** Phân đoạn VPC, WAF, Shield và Network Firewall.
    - **Dữ liệu:** Mã hóa khi lưu trữ (at-rest) và khi truyền tải (in-transit) sử dụng **AWS KMS**.
- **Quản lý Secrets:** Sử dụng AWS Secrets Manager để tự động xoay vòng (rotate) mật khẩu cơ sở dữ liệu thay vì hardcode trong ứng dụng.

#### 4. Ứng phó sự cố (Incident Response - IR)
- **Khái niệm "Playbook":** Định nghĩa các bước cụ thể cho các tình huống phổ biến như lộ IAM key hoặc lộ S3 bucket ra public.
- **Tự động hóa:** Sử dụng Lambda hoặc Step Functions để tự động cô lập EC2 bị nhiễm mã độc hoặc thu hồi quyền người dùng ngay khi phát hiện.

### Bài học rút ra (Key Takeaways)

#### Kiến trúc Zero Trust
- Không bao giờ tin tưởng, luôn luôn xác minh. Mọi yêu cầu, dù là nội bộ hay bên ngoài, đều phải được xác thực và cấp quyền.

#### Tự động hóa Bảo mật
- Tốc độ của con người không đủ để chống lại các mối đe dọa mạng. Các phản ứng bảo mật (như cô lập server) cần được tự động hóa bằng EventBridge và Lambda.

#### Mô hình Trách nhiệm chung
- Ôn lại mô hình: AWS bảo mật "của đám mây" (phần cứng, hạ tầng toàn cầu), trong khi khách hàng bảo mật "trong đám mây" (dữ liệu, cấu hình, bản vá).

### Ứng dụng vào công việc

- **Kiểm toán IAM Policies:** Sử dụng IAM Access Analyzer để kiểm tra các policy đang cấp quyền quá rộng trong dự án hiện tại.
- **Triển khai Secrets Manager:** Loại bỏ tất cả các API key bị hardcode trong code và thay thế bằng việc gọi tới AWS Secrets Manager.
- **Bật GuardDuty:** Kích hoạt Amazon GuardDuty trong tài khoản thực tập để phát hiện các mối đe dọa tiềm ẩn.

### Trải nghiệm sự kiện

Buổi workshop **"AWS Well-Architected Security Pillar"** đã cung cấp một khung tư duy mạch lạc về bảo mật.

#### Học tập có hệ thống
Việc chia nhỏ bảo mật thành **5 trụ cột rõ ràng** (IAM, Detection, Infra, Data, IR) giúp một chủ đề rộng lớn và phức tạp trở nên dễ quản lý và tiếp thu hơn.

#### Demo thực tế hữu ích
Phần demo trực tiếp về **Validate IAM Policy** và mô phỏng truy cập rất hữu ích. Nó chỉ ra cách xác minh quyền trước khi deploy, giúp tránh các lỗi "Access Denied" khi lên môi trường production.

#### Tính thực tiễn tại Việt Nam
Phần thảo luận về "Top các mối đe dọa trong môi trường cloud tại Việt Nam" và các sai lầm thường gặp giúp tôi có cái nhìn thực tế về bối cảnh an ninh mạng mà tôi sẽ đối mặt trong công việc.

#### Một số hình ảnh tại sự kiện
*Thêm ảnh sự kiện của bạn vào đây*

> Tổng kết lại, sự kiện này đã thay đổi tư duy của tôi từ "Bảo mật là rào cản" sang "Bảo mật là yếu tố then chốt" (enabler) cho việc phát triển ứng dụng hiện đại.