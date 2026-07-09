---
title: "Worklog Tuần 3"
date: 2026-05-04
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---


### Mục tiêu tuần 3:

* Nắm vững các dịch vụ lưu trữ cốt lõi trên AWS, tập trung vào Amazon S3 và Storage Gateway.
* Hiểu và triển khai các phương án bảo vệ dữ liệu tự động với AWS Backup.
* Triển khai thực tế website tĩnh và tối ưu hóa tốc độ truy cập toàn cầu bằng CloudFront.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Tìm hiểu & Thực hành AWS Backup: <br>&emsp; - Tìm hiểu: Cơ chế Data Protection và lập kế hoạch sao lưu tự động. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Tạo S3 Bucket làm nguồn và triển khai hạ tầng. <br>&emsp;&emsp; + Tạo Backup plan, thiết lập thông báo và kiểm tra hoạt động. | 04/05/2026 | 04/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 3 | - Tìm hiểu & Thực hành Amazon S3: <br>&emsp; - Tìm hiểu: Các đặc tính của Object Storage và Static Website Hosting. | 05/05/2026 | 05/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 4 | - Thực hành Amazon S3 & CloudFront: <br>&emsp;&emsp; + Tạo S3 bucket và tải dữ liệu website. <br>&emsp;&emsp; + Bật tính năng static website và cấu hình Public Access. <br>&emsp;&emsp; + Cấu hình chặn truy cập công cộng vào S3 để bảo mật. <br>&emsp;&emsp; + Tăng tốc website qua CloudFront và kiểm tra phân phối. <br>&emsp;&emsp; + Thực hành Bucket Versioning và sao chép Object sang region khác. | 06/05/2026 | 06/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 5 | - Tìm hiểu AWS Storage Gateway: <br>&emsp; - Tìm hiểu: Giải pháp Hybrid Storage kết nối On-premise và Cloud. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Khởi tạo dịch vụ Storage Gateway. <br>&emsp;&emsp; + Thiết lập cấu hình ban đầu cho Gateway. | 07/05/2026 | 07/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 6 | - Thực hành AWS Storage Gateway: <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Tạo các File Shares trên Cloud. <br>&emsp;&emsp; + Thực hiện kết nối File Shares tại máy On-premise (giả lập) để đồng bộ dữ liệu. | 08/05/2026 | 08/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |

### Kết quả đạt được tuần 3:

* **Về kiến thức:**
  * Hiểu rõ quy trình bảo vệ dữ liệu tập trung với AWS Backup giúp giảm thiểu rủi ro mất mát dữ liệu.
  * Nắm vững cách triển khai kiến trúc S3 + CloudFront để tối ưu chi phí và hiệu suất cho website tĩnh.
  * Phân biệt được các loại hình lưu trữ lai thông qua Storage Gateway.

* **Về thực hành:**
  * Đã xây dựng thành công hệ thống website tĩnh có tính bảo mật cao (chặn Public S3 và chỉ cho phép qua CloudFront).
  * Triển khai thành công việc sao lưu và đồng bộ hóa dữ liệu giữa môi trường tại chỗ và đám mây.
  * Hoàn thành tốt chuỗi các bài Lab thực hành về Storage trong lộ trình FCAJ.


