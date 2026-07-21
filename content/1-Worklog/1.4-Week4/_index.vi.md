---
title: "Worklog Tuần 4"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4

* Tìm hiểu cơ chế cân bằng tải và tự động mở rộng tài nguyên trên AWS.
* Thực hành quản lý tên miền và hệ thống DNS bằng Amazon Route 53.
* Nghiên cứu phương thức truy cập Amazon S3 thông qua VPC Endpoint.
* Tăng cường bảo mật ứng dụng bằng AWS WAF.
* Quản lý thông tin nhạy cảm bằng AWS Secrets Manager.

### Các công việc thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ 2 | Thực hành tạo Application Load Balancer, cấu hình Target Group và triển khai Auto Scaling Group cho EC2 nhằm tự động mở rộng tài nguyên theo lưu lượng truy cập. | 25/05/2026 | 25/05/2026 | Amazon EC2 Auto Scaling Documentation |
| Thứ 3 | Tìm hiểu Amazon Route 53, tạo Hosted Zone và cấu hình các bản ghi DNS phục vụ truy cập ứng dụng. | 26/05/2026 | 26/05/2026 | Amazon Route 53 Developer Guide |
| Thứ 4 | Thực hành tạo Gateway VPC Endpoint cho Amazon S3 để cho phép truy cập dữ liệu trong mạng nội bộ mà không đi qua Internet. | 27/05/2026 | 27/05/2026 | Amazon VPC User Guide |
| Thứ 5 | Cấu hình AWS WAF, tạo Web ACL và áp dụng các Managed Rules nhằm bảo vệ ứng dụng trước các cuộc tấn công phổ biến. | 28/05/2026 | 28/05/2026 | AWS WAF Documentation |
| Thứ 6 | Tạo và quản lý thông tin bí mật bằng AWS Secrets Manager; lưu trữ chuỗi kết nối cơ sở dữ liệu và thử nghiệm truy xuất Secret từ ứng dụng. | 29/05/2026 | 29/05/2026 | AWS Secrets Manager User Guide |

### Kết quả đạt được

* Hiểu được nguyên lý hoạt động của Application Load Balancer và Auto Scaling Group trong việc đảm bảo khả năng mở rộng và tính sẵn sàng của hệ thống.
* Cấu hình thành công Amazon Route 53 để quản lý tên miền và định tuyến truy cập.
* Thiết lập VPC Endpoint giúp truy cập Amazon S3 an toàn, đồng thời giảm chi phí truyền dữ liệu qua NAT Gateway.
* Áp dụng AWS WAF để tăng cường bảo mật, ngăn chặn các truy cập và tấn công không mong muốn.
* Sử dụng AWS Secrets Manager để quản lý thông tin nhạy cảm, hạn chế việc lưu trữ trực tiếp thông tin xác thực trong mã nguồn.
