---
title: "Worklog Tuần 5"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---


### Mục tiêu tuần 5:

* Làm chủ kiến trúc Serverless Backend thông qua việc xây dựng ứng dụng xử lý ảnh và ghi dữ liệu tự động bằng Lambda, S3, và DynamoDB.
* Hiểu rõ cơ chế phân quyền bảo mật chuyên sâu cho ứng dụng Serverless bằng các chính sách định danh (IAM Policy).
* Tìm hiểu giải pháp tối ưu hóa hiệu năng ứng dụng bằng bộ nhớ đệm phân tán mã nguồn mở qua Amazon ElastiCache.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Tìm hiểu & Thực hành Serverless (Phần 1 - AWS Lambda & S3): <br>&emsp; - Tìm hiểu: Cơ chế kích hoạt theo sự kiện (Event-driven) khi có tệp tải lên S3. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Khởi tạo một hàm AWS Lambda đảm nhận vai trò xử lý ảnh (Image Resizing). <br>&emsp;&emsp; + Tạo cấu trúc lưu trữ dữ liệu bằng S3 Bucket. <br>&emsp;&emsp; + Thiết lập chính sách quyền truy cập chuyên sâu (IAM Policy) dành riêng cho hàm Lambda. <br>&emsp;&emsp; + Thực hiện chạy thử nghiệm và kiểm tra tính ổn định của hàm Lambda. | 18/05/2026 | 18/05/2026 | AWS Study Group |
| 3 | - Tìm hiểu & Thực hành Serverless (Phần 2 - Amazon DynamoDB): <br>&emsp; - Tìm hiểu: Mô hình lưu trữ dữ liệu dạng NoSQL và cách tương tác dữ liệu không máy chủ. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Thiết lập cấu hình và khởi tạo một bảng cơ sở dữ liệu (DynamoDB Table). <br>&emsp;&emsp; + Lập trình/Cấu hình để hàm Lambda tự động ghi nhận nhật ký hoặc siêu dữ liệu vào bảng DynamoDB khi có sự kiện xử lý. | 19/05/2026 | 19/05/2026 | AWS Study Group |
| 4 | - Nghiên cứu & Tối ưu ứng dụng: <br>&emsp; - Đọc tài liệu, rà soát lại toàn bộ luồng hoạt động tích hợp của Serverless Backend. <br>&emsp; - Kiểm tra lỗi thực thi (Debug), tối ưu thời gian phản hồi (Timeout) và lượng RAM phân phối cho hàm Lambda. | 20/05/2026 | 20/05/2026 | AWS Study Group |
| 5 | - Tìm hiểu Amazon ElastiCache (Phần 1): <br>&emsp; - Tìm hiểu: Khái niệm In-Memory Caching (Bộ nhớ đệm trong bộ nhớ RAM). <br>&emsp; - Tìm hiểu: Tổng quan về dịch vụ Amazon ElastiCache và hai engine phổ biến là Redis / Memcached. <br>&emsp; - Phân tích các chiến lược lưu bộ nhớ đệm (Caching Strategies) để tăng tốc truy vấn dữ liệu từ Database. | 21/05/2026 | 21/05/2026 | AWS Study Group |
| 6 | - Tìm hiểu nâng cao Amazon ElastiCache (Phần 2): <br>&emsp; - Tìm hiểu: Cách thiết lập Cluster, nhân bản dữ liệu (Replication) và đảm bảo tính sẵn sàng cao cho ElastiCache. <br>&emsp; - Nghiên cứu các mô hình kiến trúc thực tế kết hợp giữa Serverless Backend, Database truyền thống và lớp Caching. | 22/05/2026 | 22/05/2026 | AWS Study Group |

### Kết quả đạt được tuần 5:

* **Về kiến thức:**
  * Nắm trọn vẹn luồng đi của dữ liệu trong mô hình hướng sự kiện: S3 (Trigger) → Lambda (Process) → DynamoDB (Store).
  * Hiểu cách thắt chặt an toàn hệ thống bằng IAM Policy chi tiết đến từng hành động (Action) và tài nguyên (Resource).
  * Nắm vững lý thuyết về In-Memory Caching để giải quyết bài toán nghẽn cổ chai dữ liệu (Database Bottleneck).

* **Về thực hành:**
  * Tự tay xây dựng hoàn chỉnh hệ thống xử lý ảnh tự động quy mô nhỏ hoàn toàn trên môi trường Serverless.
  * Thực hiện thành thạo thao tác tạo bảng, thiết lập khóa và ghi log dữ liệu tự động vào DynamoDB.
  * Hoàn thành tốt tất cả các bài Lab thực hành chuyên sâu theo tiến độ đề ra của lộ trình FCAJ.


