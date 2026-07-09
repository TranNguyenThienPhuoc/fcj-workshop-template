---
title: "Worklog Tuần 4"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---


### Mục tiêu tuần 4:

* Nắm vững quy trình dịch chuyển hệ thống (Migration) giữa môi trường vật lý/on-premise và đám mây AWS.
* Thực hành thành thạo bộ công cụ AWS VM Import/Export để di chuyển các máy ảo qua lại.
* Tìm hiểu khái niệm và kiến trúc cơ bản của hệ thống Serverless trên AWS.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Tìm hiểu & Thực hành VM Import (Dịch chuyển lên AWS): <br>&emsp; - Tìm hiểu: Tổng quan về VM Migration và cấu trúc file cấu hình của AWS VM Import/Export. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Tạo và xuất máy ảo (Export) từ môi trường VMware Workstation tại On-premises. <br>&emsp;&emsp; + Tải file máy ảo lên AWS và thực hiện lệnh Import. <br>&emsp;&emsp; + Triển khai máy chủ ảo (Deploy Instance) thành công từ AMI vừa import. | 11/05/2026 | 11/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 3 | - Tìm hiểu & Thực hành VM Export (Dịch chuyển khỏi AWS): <br>&emsp; - Tìm hiểu: Quy trình và điều kiện để xuất một Instance trên Cloud ngược về on-premise. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Thiết lập phân quyền S3 bucket ACL để chứa file export. <br>&emsp;&emsp; + Thực hành lệnh xuất máy ảo trực tiếp từ EC2 Instance và từ AMI. | 12/05/2026 | 12/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 4 | - Nghiên cứu tài liệu: <br>&emsp; - Đọc thêm các tài liệu hướng dẫn nâng cao về tối ưu hóa dung lượng file và xử lý lỗi hệ điều hành thường gặp sau khi thực hiện VM Migration. | 13/05/2026 | 13/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 5 | - Tìm hiểu lý thuyết Serverless Backend: <br>&emsp; - Học lý thuyết cơ bản về kiến trúc Serverless. <br>&emsp; - Tìm hiểu vai trò và cách thức hoạt động độc lập của các dịch vụ: <br>&emsp;&emsp; + Điện toán: AWS Lambda <br>&emsp;&emsp; + Lưu trữ: Amazon S3 <br>&emsp;&emsp; + Cơ sở dữ liệu: Amazon DynamoDB | 14/05/2026 | 14/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 6 | - Tìm hiểu tích hợp hệ thống Serverless: <br>&emsp; - Tìm hiểu mô hình kết hợp Lambda + S3 + DynamoDB để xây dựng một ứng dụng Backend hoàn chỉnh không máy chủ (Serverless Backend). <br>&emsp; - Phân tích các luồng sự kiện (Event-driven) kích hoạt giữa các dịch vụ. | 15/05/2026 | 15/05/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |

### Kết quả đạt được tuần 4:

* **Về kiến thức:**
  * Hiểu rõ kiến trúc dịch chuyển hạ tầng máy ảo qua lại giữa On-premises và Cloud sử dụng dịch vụ VM Import/Export.
  * Nắm được tư duy thiết kế hệ thống theo kiến trúc Serverless và mô hình hướng sự kiện (Event-driven architecture).

* **Về thực hành:**
  * Thực hiện thành công việc đóng gói, upload và chuyển đổi cấu trúc máy ảo từ nền tảng VMware thành một AMI sẵn sàng chạy trên EC2.
  * Biết cách cấu hình S3 Bucket ACL phục vụ cho mục đích lưu trữ và trích xuất dữ liệu hệ thống an toàn.
  * Hoàn thành tốt các mục tiêu nghiên cứu và thực hành theo đúng tiến độ của tuần.


