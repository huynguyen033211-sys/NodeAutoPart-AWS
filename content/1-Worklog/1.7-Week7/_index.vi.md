---
title: "Worklog Tuần 7"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---
### Mục tiêu tuần 7:
* Tích hợp các cổng thanh toán trực tuyến vào hệ thống J2Car AutoParts.
* Xây dựng API xử lý quy trình thanh toán và xác thực dữ liệu trả về.
* Triển khai AWS Lambda để tiếp nhận và xử lý các webhook từ cổng thanh toán.
* Kiểm thử quy trình thanh toán và cập nhật trạng thái đơn hàng.

### Các công việc thực hiện trong tuần:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ 2 | Tìm hiểu API của VNPay, MoMo và Stripe; xây dựng chức năng tạo URL thanh toán cho đơn hàng. | 15/06/2026 | 15/06/2026 | VNPay, MoMo & Stripe Documentation |
| Thứ 3 | Phát triển chức năng xác minh chữ ký (Checksum/Signature) để đảm bảo tính toàn vẹn của dữ liệu thanh toán. | 16/06/2026 | 16/06/2026 | Payment Security Guide |
| Thứ 4 | Xây dựng AWS Lambda bằng Node.js để tiếp nhận và xử lý Webhook/IPN từ các cổng thanh toán. | 17/06/2026 | 17/06/2026 | AWS Lambda Developer Guide |
| Thứ 5 | Kết nối Lambda với Backend để cập nhật trạng thái đơn hàng sau khi nhận kết quả thanh toán thành công hoặc thất bại. | 18/06/2026 | 18/06/2026 | AWS Integration Guide |
| Thứ 6 | Thực hiện kiểm thử toàn bộ quy trình thanh toán, mô phỏng các trường hợp giao dịch thành công và thất bại. | 19/06/2026 | 19/06/2026 | API Testing Documentation |

### Kết quả đạt được tuần 7:
* Hoàn thành tích hợp API thanh toán của VNPay, MoMo và Stripe.
* Xây dựng thành công cơ chế xác thực chữ ký giúp tăng cường bảo mật cho giao dịch.
* Triển khai AWS Lambda tiếp nhận Webhook/IPN và cập nhật trạng thái đơn hàng tự động.
* Kiểm thử thành công nhiều kịch bản thanh toán, đảm bảo hệ thống xử lý chính xác và ổn định.
* Nâng cao hiểu biết về kiến trúc xử lý thanh toán bất đồng bộ (Asynchronous Payment Processing) trên nền tảng AWS.
