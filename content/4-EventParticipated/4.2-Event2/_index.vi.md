---
title: "Event 2"
date: 2026-05-23
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---


# Bài thu hoạch "Chuỗi sự kiện chuyên sâu AI & Cloud"

### Mục Đích Của Sự Kiện

- **Thay đổi tư duy sử dụng AI**: Chuyển từ việc chỉ "viết prompt cơ bản" sang xây dựng "hệ thống ngữ cảnh và trí nhớ" để AI hoạt động hiệu quả; Nâng cao nhận thức về tính không xác định của các mô hình LLM.
- **Giới thiệu các giải pháp tiên tiến**: Chia sẻ về Agentic AI (Amazon Quick Suite), hệ thống Multi-Agent cấp doanh nghiệp và nền tảng cốt lõi Amazon CloudFront giúp tối ưu hiệu suất, bảo mật và chi phí cho doanh nghiệp.
- **Giao lưu và vượt qua giới hạn**: Tạo không gian học hỏi từ các chuyên gia AWS và các nhà phát triển (devs) xuất sắc thông qua các buổi chia sẻ và thử thách Hackathon quy mô lớn.

### Danh Sách Diễn Giả

- **Anh Tinh Truong** – Platform Engineer tại GoTymeX.
- **Phạm Ng Hải Anh** – AWS Community Builder (G-AsiaPacific Vietnam).
- **Nguyễn Tuấn Thịnh** – DevOps Engineer tại First Cloud AI Journey (FCAJ).
- **Anh Đức Đào** – Solution Architect tại Cloud Kinetics.
- **Bà Vy Lam** – Senior Business Systems Analyst tại VPBank.
- **Team VIB (Dự án UTMorpho)** – Đội ngũ thi đấu LotusHacks 2026.

### Nội Dung Nổi Bật

#### Tầm quan trọng của "ngữ cảnh" (Context)
- **Bản chất của lỗi**: AI đưa ra câu trả lời chung chung hoặc sai hướng thường do người dùng cung cấp ngữ cảnh yếu, không phải do mô hình AI kém.
- **3 sai lầm phổ biến khi dùng AI**:
  - **Internet Puller**: Nhồi nhét quá nhiều tài liệu không lọc, làm nhiễu AI.
  - **Nói lại điều hiển nhiên**: Cung cấp lại các thông tin mặc định mà AI đã biết.
  - **Thiếu mục tiêu và ràng buộc**: Đưa ra yêu cầu quá mơ hồ (Ví dụ: "Làm hộ tôi cái website").
- **Xu hướng tiến hóa**: Cách dùng AI đang dịch chuyển từ Prompt (Hỏi đáp đơn lẻ) → Context (Gắn với tài liệu) → Memory (Trí nhớ dài hạn/Second AI Brain).

#### Giải pháp Amazon Quick Suite (Agentic AI)
- **Phân tích nỗi đau doanh nghiệp**: Tốn thời gian thu thập dữ liệu đa nguồn và lặp lại các tác vụ thủ công.
- **Hệ sinh thái toàn diện**: Gồm BI (Dashboard), Automation (Flows) và Insights (Chat/Research) tích hợp mô hình Bedrock và hơn 40 cổng kết nối dữ liệu.
- **Demo thực tế**: Giải pháp Trợ lý PM (PM Assistant) tự động tạo biên bản họp (MoM), gửi email cho các bên liên quan và lên lịch họp tiếp theo.

#### Nền tảng Amazon CloudFront
- **Thách thức doanh nghiệp**: Rủi ro tài chính do phát sinh chi phí CDN ngoài kiểm soát (bill spike) vì traffic biến động hoặc bị tấn công DDoS.
- **Giải pháp Fixed-Price độc quyền**: Gói giá cố định tích hợp sẵn CDN, WAF, Anti-DDoS, Route 53 và S3 storage credits.
- **Phòng chống DDoS phân tán**: Cơ chế giảm thiểu tấn công diện rộng (volumetric attacks) ngay tại Edge thông qua AWS Shield, WAF và Origin Shield giúp giảm tải cho server gốc.
- **Tối ưu chi phí hạ tầng**: Giảm chi phí Load Balancer từ $8.13 xuống $2.95 (tiết kiệm chi phí Data Transfer Out nhờ CloudFront Free Tier lên tới 1TB).

#### Thử thách Hackathon LotusHacks 2026
- **Hành trình phát triển**: Đi từ "đầu óc trống rỗng" ở giờ đầu tiên cho đến bước ngoặt tìm ra ý tưởng từ chính công việc hàng ngày để khai sinh ra dự án UTMorpho.
- **Vượt khó kỹ thuật**: Đối mặt và xử lý thành công bài toán AI tạo thừa dữ liệu (AI Overgeneration) và Giới hạn dữ liệu đầu vào (Token Limits) trong 36 giờ.

#### Tính không xác định của các cấu hình LLM
- **Lý thuyết vs Thực tế**: Cấu hình Temperature = 0 (Greedy Decoding) lý thuyết sẽ đảm bảo kết quả đồng nhất 100%. Thực tế, trên 5 mô hình lớn (GPT-3.5, GPT-4o, Llama-3, Mixtral), độ chính xác có thể lệch tới 15% giữa các lần chạy giống hệt nhau.
- **Nguyên nhân kỹ thuật (GPU)**: Phép toán số dấu phẩy động trên GPU xử lý song song không có tính kết hợp: (a+b)+c != a+(b+c), dẫn đến sai số làm lật kết quả hàm chọn token (argmax).
- **Nguyên nhân thương mại (Batching)**: Việc gộp chung yêu cầu của nhiều người dùng (Inference Batching) làm thay đổi gián tiếp tiến trình tính toán của mô hình để tối ưu chi phí.

#### Ứng dụng hệ thống Multi-Agent
- **Sự bất đối xứng về dữ liệu**: Ngân hàng truyền thống thường từ chối Startup vì thiếu dữ liệu lịch sử tài chính (yêu cầu 3 năm vs thực tế 6-18 tháng).
- **Hạn chế Single Agent**: Dùng 1 AI Agent duy nhất dễ gây loãng chuyên môn, quá tải ngữ cảnh và thiếu cơ chế kiểm soát chéo.
- **Hội đồng tín dụng ảo**: Mô hình phối hợp nhiều Agent chuyên biệt (Phân tích tài chính, Đánh giá thị trường, Thẩm định đội ngũ, Đánh giá rủi ro, Kiểm tra tuân thủ) để ra quyết định chính xác, minh bạch, có thể kiểm toán.

### Những Gì Học Được

#### Xây dựng ngữ cảnh & Giao tiếp AI
- Hiểu được nguyên lý: Chất lượng ngữ cảnh quan trọng hơn số lượng.
- **Nắm vững Khung cấu trúc ngữ cảnh 4 yếu tố**:
  1. **Goal (Mục tiêu)**: Kết quả cuối cùng muốn đạt được.
  2. **Relevant info (Thông tin liên quan)**: Chỉ cung cấp dữ liệu thực sự cần thiết.
  3. **Constraints (Ràng buộc)**: Giới hạn về công nghệ, ngân sách, định dạng, phong cách.
  4. **Success criteria (Tiêu chí thành công)**: Thế nào là câu trả lời đạt yêu cầu.

#### Tư duy triển khai AI doanh nghiệp (Agentic & Multi-Agent)
- Tư duy áp dụng **Agentic AI** để tự động hóa chuỗi tác vụ phức tạp thay vì chỉ dùng chatbot thông thường.
- Tư duy thiết kế hệ thống **Multi-Agent** cho môi trường doanh nghiệp: Cách phân rã một bài toán phức tạp thành các nhiệm vụ chuyên biệt cho AI xử lý song song để tăng độ chính xác và tính chịu lỗi.

#### Kiến trúc Cloud & Bảo mật chiều sâu
- Hiểu sâu hơn về mô hình tính phí mới và cách hoạt động của mạng lưới Edge khu vực (Regional Edge Caches).
- Nắm vững nguyên lý bảo mật chiều sâu: Chặn lưu lượng xấu ngay từ điểm tiếp cận gần nguồn nhất thay vì để traffic đi sâu vào hệ thống.
- Biết cách tối ưu hóa kiến trúc phối hợp giữa EC2/ALB và CloudFront để tận dụng băng thông miễn phí.

#### Bản chất kỹ thuật của LLM & Kỹ năng làm việc nhóm
- **Xóa bỏ ảo tưởng**: Nhận ra ảo tưởng về tính an toàn và tính lặp lại tuyệt đối khi lập trình với LLM ở cấu hình mặc định. Hiểu sâu bản chất xác suất của AI từ tầng phần cứng.
- **Kỹ năng chuyên môn**: Kinh nghiệm thiết kế kiến trúc hệ thống tối ưu và kỹ thuật kiểm soát, xử lý lỗi của mô hình AI dưới áp lực lớn (under pressure).
- **Kỹ năng mềm**: Khả năng quản lý thời gian, phân phối sức lực, làm việc nhóm gắn kết và giữ bình tĩnh để tìm ra giải pháp khi khủng hoảng.

### Ứng Dụng Vào Công Việc

- **Ứng dụng khung 4 yếu tố**: Áp dụng ngay vào việc viết prompt hàng ngày để tối ưu thời gian sửa lỗi code, viết email, hoặc tóm tắt tài liệu.
- **Xây dựng Second AI Brain**: Lên kế hoạch tự xây dựng hệ thống quản lý kiến thức cá nhân tận dụng công nghệ lưu trữ đám mây và AI để hỗ trợ học tập lâu dài.
- **Triển khai tự động hóa**: Nghiên cứu tích hợp các luồng tự động (Automation Flows) và Agentic Workflow vào các tác vụ quản lý dự án, báo cáo hành chính, phân tích dữ liệu đa chiều.
- **Tối ưu hạ tầng**: Áp dụng CloudFront phân phối nội dung tĩnh/động nhằm giảm tải và hạ chi phí cho các bộ cân bằng tải (ALB); đề xuất triển khai AWS WAF và Rate Limiting để gia tăng cấu hình bảo mật.
- **Phát triển AI an toàn**: Áp dụng các kỹ thuật giảm thiểu rủi ro LLM như: Đầu ra có cấu trúc (JSON mode, function calling, regex grammars), Bầu chọn số đông (Majority Voting chạy $N$ lần), Tối ưu tham số (đưa Temperature về mức 0.1 và tăng nhẹ repeat penalty), Chấp nhận sự biến thiên trong xử lý logic.
- **Cải tiến quy trình làm việc**: Tìm kiếm cơ hội tự động hóa từ chính những tác vụ lặp đi lặp lại; áp dụng quy trình làm việc tăng tốc (agile/sprint dưới áp lực) vào các dự án thực tế của phòng ban để tối ưu tiến độ.

### Trải nghiệm trong event

#### Học hỏi thực tế và trực quan
- Sự kiện mang tính thực tiễn cao, các slide dẫn chứng số liệu trực quan (như bảng so sánh chi phí CloudFront), các ví dụ so sánh (Bad vs Good Prompt) rất dễ hiểu.
- Các phần demo (như Trợ lý PM) cực kỳ trực quan, nhận được nhiều sự tương tác và thảo luận sôi nổi từ người tham dự.

#### Trải nghiệm chuyên sâu và mở rộng góc nhìn
- Các buổi chia sẻ mở ra góc nhìn mang tính kỹ thuật nhưng rất gần gũi cho sinh viên và người mới bắt đầu làm quen với AI, đồng thời giúp dễ dàng tiếp cận các khái niệm DevOps phức tạp.
- Cung cấp case study thực tế từ chuyên gia tài chính-ngân hàng; mở rộng góc nhìn về cách biến các mô hình AI dạng thử nghiệm (PoC) thành hệ thống vận hành thực tế (Production).
- Giúp thay đổi tư duy khi thiết kế hệ thống kiểm thử (Regression testing/A-B testing) đối với AI.

#### Vượt qua giới hạn bản thân
- Một trải nghiệm kịch tính nhưng vô cùng thú vị ("have fun") tại LotusHacks. Đội ngũ đã trải qua cảm giác kiệt sức cận giờ Pitching (Burnout near pitch time) nhưng đã cùng nhau vượt qua ở những bước ngoặt quyết định để đưa sản phẩm về đích thành công.

#### Một số hình ảnh khi tham gia sự kiện
![Event 2](/images/4-EventParticipated/Event2.jpg)
> Tổng kết lại, sự kiện mang đến khối lượng kiến thức đồ sộ từ kỹ thuật chuyên sâu đến thực hành thực tiễn. Không chỉ bổ sung công cụ, chuỗi sự kiện còn giúp định hình lại tư duy thiết kế, làm việc nhóm và khai thác tối đa sức mạnh của AI/Cloud vào công việc thực tế.
