---
title: "Worklog Tuần 6"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Mục tiêu tuần 6

* Nghiên cứu và xây dựng chức năng nhận diện linh kiện ô tô thông qua hình ảnh.
* Thiết kế API tiếp nhận ảnh từ người dùng.
* Xây dựng cơ chế phân tích thông tin ảnh và tìm kiếm phụ tùng thay thế phù hợp.
* Tích hợp Amazon S3 để lưu trữ hình ảnh phục vụ quá trình xử lý.
* Kiểm thử toàn bộ chức năng AI Scan Image.

### Các công việc thực hiện

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | --- | --- | --- |
| Thứ 2 | Thiết kế API `/api/upload/scan-image`, tiếp nhận hình ảnh từ người dùng và xử lý việc tải tệp lên hệ thống. | 08/06/2026 | 08/06/2026 | Express.js Documentation |
| Thứ 3 | Xây dựng chức năng phân tích tên tệp, metadata và thông tin ảnh nhằm xác định loại phụ tùng ô tô. | 09/06/2026 | 10/06/2026 | Image Processing Documentation |
| Thứ 4 | Thực hiện truy vấn Amazon DocumentDB để tìm kiếm các phụ tùng tương thích dựa trên kết quả phân tích. | 10/06/2026 | 11/06/2026 | Amazon DocumentDB Documentation |
| Thứ 5 | Tích hợp Amazon S3 để lưu trữ hình ảnh tải lên, đồng thời kiểm tra quyền truy cập và khả năng quản lý tệp. | 11/06/2026 | 12/06/2026 | Amazon S3 Developer Guide |
| Thứ 6 | Kiểm thử toàn bộ quy trình từ tải ảnh, phân tích dữ liệu, truy vấn cơ sở dữ liệu đến hiển thị kết quả gợi ý cho người dùng. | 12/06/2026 | 12/06/2026 | Integration Testing Guide |
| Thứ 7 | Tham gia trực tiếp tại Văn phòng AWS trong buổi Mini Meetup – First Cloud AI Journey để tìm hiểu về Điện toán Đám mây (Cloud Computing) và Trí tuệ Nhân tạo (AI). | 13/06/2026 | 13/06/2026 | AWS Office |

### Kết quả đạt được

* Hoàn thiện API tiếp nhận và xử lý hình ảnh cho chức năng AI Scan Image.
* Xây dựng thành công cơ chế phân tích thông tin ảnh để xác định nhóm phụ tùng phù hợp.
* Thực hiện truy vấn dữ liệu trên Amazon DocumentDB nhằm gợi ý các sản phẩm thay thế.
* Lưu trữ an toàn hình ảnh trên Amazon S3 phục vụ kiểm thử và quản lý dữ liệu.
* Hoàn thành kiểm thử chức năng, đảm bảo quy trình nhận diện và gợi ý phụ tùng hoạt động ổn định.