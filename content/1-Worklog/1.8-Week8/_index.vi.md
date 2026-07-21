---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8:
* Tìm hiểu và triển khai cơ chế xử lý bất đồng bộ bằng Amazon SQS.
* Phát triển Backend Worker để xử lý các tác vụ nền.
* Tích hợp chức năng gửi email xác nhận đơn hàng.
* Cập nhật trạng thái đơn hàng theo thời gian thực thông qua Socket.io.

### Các công việc thực hiện trong tuần:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ 2 | Tạo và cấu hình Amazon SQS Queue để lưu trữ các yêu cầu xử lý đơn hàng. | 22/06/2026 | 22/06/2026 | Amazon SQS Documentation |
| Thứ 3 | Xây dựng Backend Worker sử dụng AWS SDK để nhận và xử lý các tin nhắn từ hàng đợi SQS. | 23/06/2026 | 23/06/2026 | AWS SDK for JavaScript |
| Thứ 4 | Phát triển chức năng cập nhật trạng thái đơn hàng và đồng bộ dữ liệu sau khi xử lý thành công. | 24/06/2026 | 24/06/2026 | Backend Service Documentation |
| Thứ 5 | Tích hợp Nodemailer để gửi email xác nhận giao dịch và thông báo đến khách hàng. | 25/06/2026 | 25/06/2026 | Nodemailer Documentation |
| Thứ 6 | Kết nối Socket.io để gửi thông báo theo thời gian thực đến giao diện quản trị khi có đơn hàng mới hoặc thay đổi trạng thái. | 26/06/2026 | 26/06/2026 | Socket.io Documentation |

### Kết quả đạt được tuần 8:
* Triển khai thành công Amazon SQS giúp tách biệt quá trình tiếp nhận và xử lý đơn hàng.
* Backend Worker hoạt động ổn định, tự động xử lý các tác vụ trong hàng đợi mà không ảnh hưởng đến hiệu năng của hệ thống.
* Hoàn thiện chức năng gửi email xác nhận đơn hàng tự động sau khi giao dịch thành công.
* Thiết lập thông báo thời gian thực bằng Socket.io giúp quản trị viên theo dõi trạng thái đơn hàng nhanh chóng.
* Hiểu rõ hơn về mô hình xử lý bất đồng bộ (Asynchronous Processing) trong các hệ thống thương mại điện tử trên nền tảng AWS.
