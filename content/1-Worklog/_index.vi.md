---
title: "Nhật ký công việc"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

### Tổng quan dự án

Hệ thống NodeJ2Car được thiết kế theo mô hình Micro-services/Containerized chạy trên nền tảng điện toán đám mây Amazon Web Services (AWS), đảm bảo tính sẵn sàng cao (High Availability), bảo mật tuyệt đối và khả năng tự động mở rộng theo tải (Auto Scaling).

**Luồng xử lý chính:**
* **Truy cập phía người dùng (Frontend):** Ứng dụng Single Page Application (SPA) React được biên dịch và lưu trữ trên Amazon S3 Web Bucket, phân phối toàn cầu qua Amazon CloudFront và bảo vệ bởi AWS WAF.
* **Xử lý logic nghiệp vụ (Backend):** Các API REST và kết nối Socket.io được định tuyến thông qua Application Load Balancer (ALB) (hỗ trợ Sticky Sessions) đến các container ECS Backend Task (NodeJS + Express) chạy trên AWS Fargate nằm trong các Private Subnets bảo mật.
* **Thanh toán bất đồng bộ (Payment Integration):** Cổng thanh toán bên ngoài (Momo, VNPay, Stripe) gọi Webhook IPN đến AWS Lambda. Lambda tiếp nhận, kiểm tra tính hợp lệ và đẩy log hóa đơn sạch vào Amazon SQS (Payment Queue). Các Backend Tasks (ECS Fargate) đóng vai trò Worker rút tin nhắn từ hàng đợi SQS để xử lý chốt đơn và thông báo trạng thái thời gian thực thông qua Socket.io.
* **Lưu trữ dữ liệu:** Dữ liệu Document được lưu trữ tại Amazon DocumentDB (tương thích MongoDB) với cấu trúc Cluster gồm Primary Node (đọc/ghi) và Replica Node (chỉ đọc) tự động đồng bộ. Bộ nhớ đệm và quản lý phiên kết nối Socket.io sử dụng Amazon ElastiCache Redis (Primary/Replica).

---

### Nhật ký công việc (12 tuần)

Dưới đây là tiến độ công việc được thực hiện trong suốt thời gian thực tập.

**Tuần 1 (05/05/2026 - 10/05/2026):** [Làm quen môi trường thực tập, AWS Console, IAM và AWS Budgets](1.1-week1/)

**Tuần 2 (11/05/2026 - 17/05/2026):** [Tìm hiểu Amazon EC2, Amazon S3, Amazon RDS và kết nối cơ sở dữ liệu](1.2-week2/)

**Tuần 3 (18/05/2026 - 24/05/2026):** [Thực hành Amazon VPC, CloudWatch, DynamoDB và Redis](1.3-week3/)

**Tuần 4 (25/05/2026 - 31/05/2026):** [Nghiên cứu AWS Lambda, ECS, Elastic Load Balancer và Auto Scaling](1.4-week4/)

**Tuần 5 (01/06/2026 - 07/06/2026):** [Thực hành Amazon SQS, SNS, Cognito và quy trình phát triển hệ thống](1.5-week5/)

**Tuần 6 (08/06/2026 - 14/06/2026):** [Phân tích yêu cầu hệ thống, thiết kế cơ sở dữ liệu và xây dựng API cho J2Car AutoParts](1.6-week6/)

**Tuần 7 (15/06/2026 - 21/06/2026):** [Phát triển Backend, tích hợp JWT Authentication và nghiên cứu AI Scan Image](1.7-week7/)

**Tuần 8 (22/06/2026 - 28/06/2026):** [Xây dựng chức năng giỏ hàng, đặt hàng, thanh toán và xử lý hàng đợi Amazon SQS](1.8-week8/)

**Tuần 9 (29/06/2026 - 05/07/2026):** [Docker hóa ứng dụng Backend, tích hợp MongoDB và triển khai trên Amazon ECS](1.9-week9/)

**Tuần 10 (06/07/2026 - 12/07/2026):** [Hoàn thiện Frontend - Backend, kết nối API và triển khai hệ thống trên AWS](1.10-week10/)

**Tuần 11 (13/07/2026 - 19/07/2026):** [Kiểm thử chức năng, kiểm thử tích hợp, xử lý lỗi và tối ưu hiệu năng hệ thống](1.11-week11/)

**Tuần 12 (20/07/2026 - 27/07/2026):** [Hoàn thiện dự án, tối ưu cơ sở dữ liệu, tổng hợp tài liệu và kết quả thực tập](1.12-week12/)