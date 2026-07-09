---
title: "Event 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---


# Bài thu hoạch "FCAJ Community Day"

### Mục Đích Của Sự Kiện

- **Chia sẻ phương pháp học tập**: Hướng dẫn cách "hack" não bộ để tạo động lực và duy trì thói quen học tập công nghệ.
- **Hướng dẫn ứng dụng AI**: Chia sẻ kỹ thuật Prompt Engineering để tối ưu hóa giao tiếp với AI và giới thiệu phương pháp BMX (dùng các AI Agents) để hỗ trợ toàn diện vòng đời phát triển phần mềm (Software Development Lifecycle).
- **Định hướng nghề nghiệp & Mindset**: Nhấn mạnh tầm quan trọng của kiến thức nền tảng (Foundation), tư duy phản biện (hỏi "Tại sao?") và sự liêm chính trong công việc cho các bạn sinh viên/fresher.
- **Kết nối cộng đồng**: Tạo môi trường an toàn để các bạn trẻ rèn luyện kỹ năng thuyết trình, mạnh dạn chia sẻ kiến thức công nghệ (AWS, AI, kiến trúc phần mềm) với mọi người.

### Danh Sách Diễn Giả

- **Huỳnh Hoàng Long** – Bootcamp, First Cloud AI Journey
- **Nguyễn Tuan Thinh** – DevOps/Cloud Engineer, First Cloud AI Journey
- **Khang Nguyễn** – Solution Architect tại Cloud Kinetics
- **Nguyễn Phương Thảo** – Software Developer tại Ngân hàng Quốc tế VIB

### Nội Dung Nổi Bật

#### Hack não để "nghiện" học

- **Nguyên nhân lười học**: Việc học mang lại kết quả chậm và đòi hỏi sự tập trung cao, trái ngược với game hay mạng xã hội vốn cung cấp "phần thưởng nhanh" và liên tục kích thích sự tò mò.
- **Giải pháp (Cơ chế Dopamine)**: Dopamine không tiết ra khi nhận thưởng, mà tiết ra khi *mong chờ* phần thưởng. Bạn có thể hack não bằng cách:
  - **Tạo hộp phần thưởng ngẫu nhiên**: Ghi các phần thưởng nhỏ (hoặc "chúc may mắn lần sau") để bốc thăm sau mỗi 10 phút học, tạo sự tò mò.
  - **Tâm lý sợ mất mát (Streak)**: Điểm danh việc học mỗi ngày (giống chuỗi Duolingo/TikTok) để tạo tâm lý tiếc nuối nếu lỡ bỏ ngắt quãng.
  - **Chia nhỏ mục tiêu**: Đừng ép bản thân học 5 tiếng/ngày — hãy chia thành các chặng 10–30 phút để não không bị "ngợp" hay sợ hãi.
  - **Game hóa**: Tự tạo hệ thống cấp độ (rank) hoặc điểm XP để thấy rõ sự tiến bộ mỗi ngày.

#### Kỹ thuật Prompt Engineering

- **Công thức Prompt chuẩn (7 thành phần)**: Role (Vai trò), Context (Ngữ cảnh), Instruction (Hướng dẫn), Input (Đầu vào), Output format (Định dạng đầu ra), Examples (Ví dụ) và Constraints (Giới hạn).
- **Lưu ý khi viết Prompt**:
  - Dùng ngôn ngữ rành mạch, chia nhỏ input dài.
  - Tránh dùng từ phủ định (VD: "đừng làm thế này") — hãy chỉ định rõ điều AI nên làm để tránh ảo giác (hallucination).
- **Chi phí Token**: Dùng tiếng Việt cho AI thường tốn lượng token gấp đôi so với tiếng Anh.
- **Demo ứng dụng**: Tác giả trình bày dự án tiện ích mở rộng "Prompt Optimizer" sử dụng kiến trúc Serverless trên AWS (Cognito, S3, API Gateway, Lambda, Bedrock...).

#### Mindset & Định hướng nghề nghiệp

- **Đừng "outsource" tư duy cho AI**: AI sẽ không thay thế bạn — nó chỉ khuếch đại năng lực (làm tốt sẽ tốt hơn, làm tệ sẽ tệ đi). Nền tảng (Foundation) vững chắc mới là điều cốt lõi.
- **Tư duy "Tại sao?"**: Luôn chất vấn mọi giải pháp và tự kiểm tra lại công việc của mình. Trả lời được câu hỏi "Why" quan trọng hơn việc chỉ biết làm "What".
- **Sự liêm chính (Integrity)**: Làm việc chuẩn chỉnh đến cùng ngay cả ở những ngoại lệ nhỏ nhất hoặc khi không có ai giám sát — đây là chìa khóa xây dựng niềm tin đường dài.
- **Tiêu chí đánh giá Fresher**: Đối với nhà tuyển dụng, thứ tự ưu tiên là: **Thái độ > Học vấn > Kỹ năng > Kinh nghiệm**. Hãy nhìn dài hạn và ưu tiên những công việc mang lại nhiều trải nghiệm, kiến thức thay vì chỉ nhìn vào mức lương khởi điểm.

#### Phương pháp BMX phát triển phần mềm bằng AI

- **Vấn đề của cách dùng AI cũ**: Nếu ném toàn bộ ý tưởng vào một khung chat để AI sinh code, AI sẽ nhanh chóng quên bối cảnh (context) và tạo ra code lỗi, khó bảo trì.
- **Giải pháp BMX (B-Method)**: Chia nhỏ dự án và gán các vai trò (Role) cụ thể cho nhiều AI Agent khác nhau, quy trình vận hành như một team thật:
  - **PM Agent**: Phân tích ý tưởng và viết tài liệu yêu cầu (PRD).
  - **Architect Agent**: Dựa vào PRD để thiết kế kiến trúc công nghệ.
  - **Scrum Master Agent**: Cắt nhỏ PRD thành các tính năng (Epic/Story) nhỏ gọn.
  - **Dev & Tester Agent**: Chỉ nhận nhiệm vụ code và kiểm thử cho đúng một Story duy nhất.
- **Lợi ích**: Thu hẹp cửa sổ ngữ cảnh (context window) giúp AI code chính xác hơn, tránh chồng chéo tính năng và rất dễ quản lý/cập nhật hệ thống sau này.

### Những Gì Học Được

#### Phương pháp học tập & Tâm lý

- **Cơ chế Dopamine**: Hiểu rằng não bộ phản ứng với *kỳ vọng* phần thưởng, không phải bản thân phần thưởng — đây là chìa khóa để tự tạo động lực bền vững.
- **Game hóa việc học**: Áp dụng các yếu tố ngẫu nhiên (random reward), streak và XP vào lịch học hàng ngày để duy trì thói quen lâu dài.
- **Chia nhỏ mục tiêu**: Học theo chặng ngắn 10–30 phút thực sự hiệu quả hơn và ít tốn công sức tâm lý hơn là cố học "marathon" nhiều giờ liền.

#### Kỹ năng Prompt Engineering

- **Cấu trúc 7 thành phần** giúp viết Prompt rõ ràng, có hệ thống và giảm thiểu ảo giác (hallucination) từ AI.
- **Ngôn ngữ Prompt**: Ưu tiên dùng tiếng Anh khi làm việc với AI để tiết kiệm token và tăng độ chính xác của đầu ra.
- **Kiến trúc Serverless**: Hiểu cách xây dựng ứng dụng AI thực tế trên AWS thông qua demo Prompt Optimizer (Cognito, API Gateway, Lambda, Bedrock).

#### Tư duy nghề nghiệp

- **Foundation là tất cả**: AI chỉ là công cụ khuếch đại — người có nền tảng vững sẽ được khuếch đại tốt, người thiếu nền tảng sẽ bị khuếch đại sai hướng.
- **Tư duy "Why"**: Không chỉ học cách làm, mà phải hiểu lý do tại sao — đây là thứ tạo ra sự khác biệt thực sự trong công việc.
- **Integrity**: Sự liêm chính không phải là quy tắc mà là thói quen phải xây dựng từng ngày, kể cả khi không ai nhìn.
- **Ưu tiên trải nghiệm hơn lương**: Giai đoạn đầu sự nghiệp, môi trường học hỏi quan trọng hơn nhiều so với mức lương.

#### Phương pháp BMX

- **Context window là giới hạn thực tế**: Hiểu tại sao việc đưa quá nhiều context vào một cuộc hội thoại AI dẫn đến kết quả tệ.
- **AI as a team**: Mô hình nhiều Agent với vai trò rõ ràng (PM, Architect, Dev, Tester) giúp AI hoạt động hiệu quả hơn và dễ kiểm soát hơn.
- **Tư duy modular**: Chia nhỏ dự án thành các Story nhỏ không chỉ giúp AI code tốt hơn mà còn là best practice trong quản lý phần mềm.

### Ứng Dụng Vào Công Việc

- **Xây dựng thói quen học hàng ngày**: Thiết lập hệ thống streak + phần thưởng ngẫu nhiên cho lịch tự học AWS/AI hàng ngày, thay vì đặt mục tiêu học nhiều tiếng liền.
- **Viết Prompt có cấu trúc**: Áp dụng công thức 7 thành phần (Role, Context, Instruction, Input, Output, Examples, Constraints) vào mọi lần tương tác với AI trong công việc thực tế.
- **Ưu tiên tiếng Anh khi dùng AI**: Chuyển các Prompt quan trọng sang tiếng Anh để giảm chi phí token và tăng chất lượng đầu ra.
- **Thử nghiệm phương pháp BMX**: Áp dụng mô hình đa Agent cho dự án side-project tiếp theo — dùng AI Agent riêng biệt cho từng vai trò PM, Architect, Dev, Tester.
- **Luôn hỏi "Tại sao?"**: Trước khi áp dụng bất kỳ giải pháp nào (từ AI hay từ tài liệu), tự đặt câu hỏi "Why?" để hiểu sâu thay vì chỉ copy-paste.
- **Đặt nền tảng lên hàng đầu**: Dành thời gian ôn lại các kiến thức cơ bản (networking, OS, data structures) song song với việc học công nghệ mới.

### Trải nghiệm trong event

Tham gia **"FCAJ Community Day"** là một trải nghiệm thực sự khác biệt so với các workshop kỹ thuật thông thường. Điểm nổi bật nhất không phải là nội dung công nghệ mà là **cách tiếp cận con người** — từ tâm lý học tập, mindset nghề nghiệp đến cách tương tác với AI một cách thông minh.

#### Học hỏi từ những người đi trước thực chiến

- Các diễn giả không đến để "dạy lý thuyết" mà chia sẻ những bài học rút ra từ trải nghiệm thực tế của chính họ — từ DevOps, Solution Architect đến Software Developer tại các tổ chức lớn.
- Câu chuyện về **Integrity và tư duy "Why"** để lại ấn tượng sâu sắc, nhắc nhở rằng kỹ năng mềm và đạo đức nghề nghiệp quan trọng không kém kỹ thuật.

#### Trải nghiệm kỹ thuật thực tế

- Demo **Prompt Optimizer** trên kiến trúc Serverless AWS cho thấy cách biến một ý tưởng đơn giản thành sản phẩm thực sự với các dịch vụ cloud hiện đại.
- Phương pháp **BMX** mở ra cách nhìn mới về việc tổ chức công việc với AI — không phải "hỏi AI một câu", mà là "xây dựng một quy trình AI".

#### Kết nối cộng đồng

- Không khí sự kiện tạo ra một **không gian an toàn để chia sẻ** — các bạn trẻ mạnh dạn đặt câu hỏi, đưa ra góc nhìn cá nhân mà không sợ bị phán xét.
- Việc gặp gỡ những người có cùng đam mê công nghệ và chung hành trình học AWS/AI tiếp thêm rất nhiều động lực để tiếp tục cố gắng.

#### Bài học rút ra

- **Học tập bền vững** không đến từ ý chí mà đến từ việc thiết kế đúng môi trường và cơ chế khen thưởng cho bản thân.
- **AI là công cụ cộng hưởng**: Người giỏi dùng AI sẽ giỏi hơn — người yếu dùng AI sẽ yếu hơn vì sẽ phụ thuộc mà không hiểu bản chất.
- **Cộng đồng là tài sản**: Việc tham gia và đóng góp cho cộng đồng công nghệ sớm sẽ tạo ra lợi thế cạnh tranh lớn về lâu dài.


