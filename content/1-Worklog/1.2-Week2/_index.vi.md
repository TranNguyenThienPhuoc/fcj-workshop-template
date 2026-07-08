---
title: "Worklog Tuần 2"
date: 2026-04-27
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu tuần 2:

* Nắm vững các kỹ thuật quản lý và kết nối mạng nâng cao trên AWS.
* Hiểu cách triển khai hạ tầng tự động và tích hợp hệ thống Hybrid Cloud.
* Thực hành kết nối đa mạng thông qua Transit Gateway, VPC Peering và quản lý DNS tập trung.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Tìm hiểu & Thực hành Route 53: <br>&emsp; - Tìm hiểu: Hybrid DNS Management với Amazon Route 53. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Tạo Route 53 Outbound/Inbound Endpoint. <br>&emsp;&emsp; + Thiết lập Resolver Rules và Test kết quả. | 27/04/2026 | 27/04/2026 | AWS Study Group |
| 3 | - Tìm hiểu & Thực hành Transit Gateway (P1): <br>&emsp; - Tìm hiểu: Centralized Network Management với AWS Transit Gateway. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Tạo Key Pair và khởi tạo CloudFormation Template. <br>&emsp;&emsp; + Tạo Transit Gateway và Attachments. | 28/04/2026 | 28/04/2026 | AWS Study Group |
| 4 | - Thực hành Transit Gateway (P2): <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Thiết lập Transit Gateway Route Tables. <br>&emsp;&emsp; + Thêm Transit Gateway Routes vào VPC Route Tables. | 29/04/2026 | 29/04/2026 | AWS Study Group |
| 5 | - Tìm hiểu & Thực hành VPC Peering (P1): <br>&emsp; - Tìm hiểu: Network Integration với VPC Peering. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Khởi tạo CloudFormation, tạo Security Group và EC2. <br>&emsp;&emsp; + Cập nhật Network ACL. <br>&emsp;&emsp; + Thiết lập VPC và các thành phần phụ trợ. <br>&emsp;&emsp; + Kích hoạt ghi log lưu lượng mạng (VPC Flow Logs). | 30/04/2026 | 30/04/2026 | AWS Study Group |
| 6 | - Thực hành VPC Peering (P2): <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Tạo kết nối Peering giữa các VPC. <br>&emsp;&emsp; + Kích hoạt Cross-Peer DNS để phân giải tên miền. | 01/05/2026 | 01/05/2026 | AWS Study Group |

### Kết quả đạt được tuần 2:

* **Về kiến thức:**
  * Hiểu sâu về kiến trúc mạng quy mô lớn bằng cách sử dụng Transit Gateway để quản lý tập trung.
  * Nắm vững cách thức xử lý DNS trong môi trường lai (Hybrid) bằng Route 53 Resolver.
  * Biết cách sử dụng CloudFormation để tự động hóa việc triển khai hạ tầng thay vì thao tác tay.

* **Về thực hành:**
  * Xây dựng thành công hệ thống kết nối đa VPC thông qua cả hai phương thức: Peering và Transit Gateway.
  * Thiết lập được hệ thống DNS có khả năng phân giải tên miền từ Cloud về On-premise và ngược lại.
  * Thực hiện thành thạo các bước chuẩn bị hạ tầng (Key Pair, SG, EC2) thông qua các kịch bản mẫu có sẵn.


