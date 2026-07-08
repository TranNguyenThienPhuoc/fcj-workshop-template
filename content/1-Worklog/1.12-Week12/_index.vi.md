---
title: "Worklog Tuần 12"
date: 2024-01-01
weight: 12
chapter: false
pre: " <b> 1.12. </b> "
---

### Mục tiêu tuần 12:

* Hoàn thiện cấu hình Amazon ElastiCache (Redis) để tối ưu tốc độ hệ thống.
* Tích hợp thành công cổng thanh toán PayOS (VietQR) từ Backend đến Frontend.
* Cấu hình Email Production (Amazon SES) và bổ sung các thiếu sót trong CI/CD.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc                                                                                                                                                                                   | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                            |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ----------------------------------------- |
| 2   | - **Tối ưu Tốc độ (Redis) & Tích hợp PayOS (Backend)** <br> - Cấu hình Subnet, Security Group và tạo ElastiCache Redis Cluster. <br> - Lấy Key PayOS và cấu hình biến môi trường server. | 06/07/2026   | 06/07/2026      | <https://www.youtube.com/@javascriptmastery> <br> <https://bun.com/> <br> <https://www.youtube.com/@AWSEventsChannel> |
| 3   | - **PayOS (Frontend), SES Production & CI/CD** <br> - Tích hợp nút thanh toán PayOS trên Frontend. <br> - Gỡ SES Sandbox và cấu hình Secret CloudFront cho GitHub Actions.                 | 07/07/2026   | 07/07/2026      | <https://www.youtube.com/@javascriptmastery> <br> <https://bun.com/> <br> <https://www.youtube.com/@AWSEventsChannel> |
| 4   | - **Viết báo cáo tổng kết dự án** <br> - Bắt đầu soạn thảo tài liệu báo cáo quá trình thực tập.                                                             | 08/07/2026   | 08/07/2026      | 
| 5   | - **Viết báo cáo tổng kết dự án** <br> - Bắt đầu soạn thảo tài liệu báo cáo quá trình thực tập.                                                           | 09/07/2026   | 09/07/2026      | 



### Kết quả đạt được tuần 12:

* Hệ thống đã được tối ưu hóa tốc độ nhờ áp dụng Caching qua cụm ElastiCache (Redis).
* Chức năng thanh toán qua mã VietQR (PayOS) hoạt động mượt mà từ Frontend đến Backend.
* Hệ thống Email tự động đã sẵn sàng cho môi trường Production (thoát khỏi SES Sandbox).
* Luồng CI/CD được hoàn thiện 100%, tự động clear cache trên CloudFront mỗi lần cập nhật.
* Hoàn thành tài liệu báo cáo tổng kết dự án, sẵn sàng cho việc thuyết trình và bàn giao.
