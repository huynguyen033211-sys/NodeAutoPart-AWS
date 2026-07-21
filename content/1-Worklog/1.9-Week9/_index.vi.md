---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---
### Mục tiêu tuần 9:
* Đóng gói ứng dụng Backend bằng Docker.
* Lưu trữ Docker Image trên Amazon Elastic Container Registry (ECR).
* Triển khai ứng dụng bằng Amazon ECS Fargate.
* Cấu hình cân bằng tải và tự động mở rộng cho hệ thống.

### Các công việc thực hiện trong tuần:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ 2 | Xây dựng Dockerfile cho ứng dụng Backend Node.js và tối ưu quá trình build container. | 29/06/2026 | 29/06/2026 | Docker Documentation |
| Thứ 3 | Tạo Amazon ECR Repository, build Docker Image và đẩy image lên Amazon ECR. | 30/06/2026 | 30/06/2026 | Amazon ECR Documentation |
| Thứ 4 | Tạo ECS Task Definition và cấu hình tài nguyên CPU, Memory, Environment Variables cho ứng dụng. | 01/07/2026 | 01/07/2026 | Amazon ECS Developer Guide |
| Thứ 5 | Triển khai Backend trên Amazon ECS Fargate, cấu hình Service và Application Load Balancer. | 02/07/2026 | 02/07/2026 | ECS Fargate Deployment Guide |
| Thứ 6 | Thiết lập Auto Scaling cho ECS Service và kiểm tra khả năng mở rộng khi tải hệ thống tăng cao. | 03/07/2026 | 03/07/2026 | ECS Auto Scaling Guide |
| Thứ 7 | Tham gia trực tiếp tại Văn phòng AWS tham dự sự kiện Swinburne Cloud Mastery 2026 để tìm hiểu về Điện toán Đám mây, hệ sinh thái AWS, cơ hội nghề nghiệp trong lĩnh vực Cloud Computing, tư duy đổi mới sáng tạo, đồng thời giao lưu với các Kiến trúc sư Giải pháp AWS, chuyên gia công nghệ và sinh viên. | 04/07/2026 | 04/07/2026 | AWS Office |

### Kết quả đạt được tuần 9:
* Đóng gói thành công ứng dụng Backend bằng Docker và quản lý phiên bản image trên Amazon ECR.
* Triển khai ứng dụng ổn định trên Amazon ECS Fargate mà không cần quản lý máy chủ.
* Hoàn thành cấu hình Application Load Balancer để phân phối lưu lượng truy cập đến các container.
* Thiết lập chính sách Auto Scaling giúp hệ thống tự động mở rộng khi nhu cầu sử dụng tăng.
* Hiểu rõ quy trình triển khai ứng dụng container hóa trên nền tảng AWS và các thành phần liên quan.
