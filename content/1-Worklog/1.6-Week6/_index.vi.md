---
title: "Worklog Tuần 6"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Mục tiêu tuần 6:

* Nắm vững quy trình đóng gói ứng dụng (Containerization) sử dụng Docker và Docker Compose.
* Hiểu và thực hành quản lý, điều phối container quy mô doanh nghiệp với Amazon ECS (Elastic Container Service).
* Triển khai thực tế các chiến lược Deployment nâng cao (Blue/Green Deployment, Rolling Update) kết hợp cân bằng tải (ALB).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --------- | ------------ | --------------- | -------------- |
| 2 | - Tìm hiểu & Thực hành Containerization với Docker (P1): <br>&emsp; - Tìm hiểu: Tổng quan về Docker, Dockerfile và các lệnh cơ bản. <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Cài đặt các thư viện phụ thuộc (Dependencies) và chạy ứng dụng ở môi trường Local. <br>&emsp;&emsp; + Tạo Docker Image cho ứng dụng, triển khai chạy thử và kiểm tra hoạt động (Test Application). | 25/05/2026 | 25/05/2026 | AWS Study Group |
| 3 | - Thực hành Docker Compose & Push Image (P2): <br>&emsp; - Thực hành nâng cao: <br>&emsp;&emsp; + Viết file docker-compose.yml để khởi chạy đồng thời nhiều container (Frontend, Backend, Database). <br>&emsp;&emsp; + Kiểm tra tính toàn vẹn và kết nối của ứng dụng đa container. <br>&emsp;&emsp; + Đăng nhập và đẩy (Push) sản phẩm Image lên hệ thống lưu trữ Amazon ECR và Docker Hub. | 26/05/2026 | 26/05/2026 | AWS Study Group |
| 4 | - Nghiên cứu kiến trúc & Chuẩn bị môi trường ECS: <br>&emsp; - Tìm hiểu: Centralized Container Management và kiến trúc Amazon ECS (Cluster, Task Definition, Service). <br>&emsp; - Thực hành: Chuẩn bị hạ tầng mạng cơ bản: <br>&emsp;&emsp; + Thiết lập cấu hình Infrastructure, tạo CodeDeploy Role. <br>&emsp;&emsp; + Cấu hình bổ sung Subnet, NAT Gateway, Route Table và Security Group. | 27/05/2026 | 27/05/2026 | AWS Study Group |
| 5 | - Triển khai Amazon ECS - Khởi tạo tài nguyên (P1): <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Đăng ký không gian tên định danh (Namespace) trong AWS Cloud Map. <br>&emsp;&emsp; + Khởi tạo cụm máy chủ container ECS Cluster. <br>&emsp;&emsp; + Định nghĩa các thông số vận hành qua ECS Task Definition (chia tách rõ ràng cho Backend task và Frontend task). | 28/05/2026 | 28/05/2026 | AWS Study Group |
| 6 | - Triển khai Amazon ECS - Cấu hình Load Balancer & Service (P2): <br>&emsp; - Thực hành: <br>&emsp;&emsp; + Cấu hình Application Load Balancer (ALB): Khởi tạo Target Group và ALB kiểm soát luồng traffic. <br>&emsp;&emsp; + Tạo ECS Service và áp dụng các chiến lược phát hành: <br>&emsp;&emsp;&emsp; * Backend: Blue/Green Deployment và cấu hình tự động co giãn (Service Scaling). <br>&emsp;&emsp;&emsp; * Frontend: Deploy theo cơ chế tịnh tiến cuốn chiếu (Rolling Update). <br>&emsp;&emsp; + Kiểm tra kết quả hệ thống (Test Result) và dọn dẹp tài nguyên (Clean Up Resources). | 29/05/2026 | 29/05/2026 | AWS Study Group |

### Kết quả đạt được tuần 6:

* **Về kiến thức:**
  * Hiểu sâu sắc tư duy đóng gói ứng dụng bằng Docker giúp giải quyết triệt để bài toán đồng nhất môi trường từ Local lên Cloud.
  * Nắm vững kiến trúc điều phối nâng cao của Amazon ECS, phân biệt rõ cách thức hoạt động của Task Definition và Service.
  * Hiểu rõ bản chất và kịch bản áp dụng của hai chiến lược deployment phổ biến: Blue/Green Deployment (giảm thiểu tối đa downtime) và Rolling Update.

* **Về thực hành:**
  * Tự tay viết Dockerfile, file Docker Compose và đóng gói thành công một ứng dụng đa lớp hoàn chỉnh.
  * Đẩy thành công mã nguồn đóng gói lên các Registry uy tín (ECR, Docker Hub).
  * Thiết lập hoàn chỉnh một hệ thống phân phối tự động trên ECS có gắn bộ cân bằng tải ALB, thực hiện cấu hình tự động co giãn tải (Scaling) linh hoạt cho tầng Backend và cập nhật cuốn chiếu an toàn cho tầng Frontend.


