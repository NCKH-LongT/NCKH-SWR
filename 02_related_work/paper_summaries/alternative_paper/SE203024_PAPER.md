# Paper List - Danh sách bài báo liên quan

## Thông tin nhóm

- Lớp: SE2037
- Nhóm: 7
- Leader: Sĩ Hưng
- Người phụ trách phần này: Thanh
- Tuần: Week 2 (Tìm bài báo liên quan)

## Thông tin đề tài

**Chủ đề chính (English):** AI-Driven Personal Assistant for Mitigating Academic Procrastination and Enhancing Time Management among Students

**Chủ đề chính (Tiếng Việt):** Xây dựng ứng dụng trợ lý ảo cá nhân ứng dụng Trí tuệ nhân tạo nhằm giảm thiểu hành vi trì hoãn học tập và nâng cao năng lực quản lý thời gian cho học sinh, sinh viên.

**Lĩnh vực:** Software Requirements Engineering cho hệ thống AI-based personal assistant trong giáo dục đại học.

---

## Bài 1

**Tên bài báo:** How mature is requirements engineering for AI-based systems? A systematic mapping study on practices, challenges, and future research directions

**Tác giả:** Umm-e-Habiba, Markus Haug, Justus Bogner, Stefan Wagner

**Nguồn:** Requirements Engineering (Springer), Vol. 29, Issue 4, pp. 567-600, December 2024

**Link:** https://link.springer.com/article/10.1007/s00766-024-00432-3

**DOI:** 10.1007/s00766-024-00432-3

**Trạng thái:** Peer-reviewed, open access, 26 citations, 13k accesses

### Vấn đề thực tế trong bài

AI đang xâm nhập vào mọi lĩnh vực, kéo theo các thách thức mới cho Requirements Engineering (RE4AI): khó đặc tả và kiểm định yêu cầu cho hệ thống AI, các yêu cầu chất lượng mới phát sinh từ vấn đề đạo đức. Hiện chưa rõ liệu các phương pháp RE hiện có có đủ để xử lý những thách thức này không, hay cần phát triển phương pháp mới. Nhóm tác giả thực hiện systematic mapping study với 126 primary studies để tổng hợp toàn cảnh RE4AI.

### Vì sao vấn đề này quan trọng

Đây là bài tổng hợp lớn nhất hiện có về RE cho hệ thống AI. Cung cấp nền tảng lý thuyết bắt buộc cho mọi nhóm nghiên cứu liên quan đến RE cho AI assistant, bao gồm cả các đề tài về AI trong giáo dục.

### Gap (điểm thiếu sót)

1. Cấp độ trừu tượng cao, không đi sâu vào domain cụ thể (giáo dục, y tế, finance). Chỉ ra GAP chung của RE4AI nhưng không validate trong domain education.
2. Phương pháp là mapping và snowballing, không có primary user study với stakeholders thực.
3. Có thể bỏ sót nghiên cứu non-English hoặc grey literature từ Đông Nam Á.
4. Bài xác định "gap giữa ML engineers với end-users" là challenge phổ biến nhất nhưng không đề xuất phương pháp elicitation cụ thể để bridge gap đó trong hệ thống giáo dục.
5. Không bao quát các yêu cầu đặc thù của hệ thống chống trì hoãn như gamification, notification, behavioral nudging.

---

## Bài 2

**Tên bài báo:** AI-Based Personalized E-Learning Systems: Issues, Challenges, and Solutions

**Tác giả:** Mir Murtaza, Yamna Ahmed, Jawwad Ahmed Shamsi, Fahad Sherwani, Mariam Usman

**Nguồn:** IEEE Access, Vol. 10, pp. 81323-81342, xuất bản 26/07/2022

**Link:** https://ieeexplore.ieee.org/document/9840390

**DOI:** 10.1109/ACCESS.2022.3193938

**Trạng thái:** Peer-reviewed, open access, 131 citations

### Vấn đề thực tế trong bài

Hệ thống e-learning truyền thống cung cấp nội dung giống nhau cho mọi học viên, trong khi personalized e-learning cần xác định nội dung phù hợp dựa trên mức độ hiểu biết và phong cách học của từng người. Bài tổng hợp requirements và challenges của personalized e-learning với 4 research questions, đề xuất framework 5 module: Data Module, Adaptive Learning Module, Adaptable Learning Module, Recommender Module, Content and Assessment Delivery Module.

### Vì sao vấn đề này quan trọng

Là một trong những survey được trích dẫn nhiều nhất về personalized AI learning. Cung cấp framework chuẩn cho personalized e-learning AI, là nền tảng để nhóm so sánh khi đề xuất hệ thống assistant của mình.

### Gap (điểm thiếu sót)

1. Framework 5 module tập trung hoàn toàn vào "What to learn" (nội dung học), không có module nào xử lý "When to learn" hay "How to stop procrastinating".
2. Không có Reminder hoặc Notification Module, bỏ qua hoàn toàn behavioral nudging.
3. Là literature survey, không phải primary RE study. Requirements được tổng hợp từ literature thay vì phỏng vấn sinh viên thực tế.
4. Framework chưa được implement hay validate với stakeholders thực.
5. Không đề cập đến các khía cạnh tâm lý của procrastination (CBT, self-regulation theory).
6. Bối cảnh khảo sát chủ yếu phương Tây và Pakistan, thiếu Đông Nam Á và Việt Nam.

---

## Bài 3

**Tên bài báo:** How educational chatbots support self-regulated learning? A systematic review of the literature

**Tác giả:** Rui Guan, Mladen Raković, Guanliang Chen, Dragan Gašević

**Nguồn:** Education and Information Technologies (Springer), Vol. 30, Issue 4, pp. 4493-4518, March 2025 (xuất bản online 30/08/2024)

**Link:** https://link.springer.com/article/10.1007/s10639-024-12881-y

**DOI:** 10.1007/s10639-024-12881-y

**Trạng thái:** Peer-reviewed, open access, 76 citations, 19k accesses

### Vấn đề thực tế trong bài

Self-regulated learning (SRL) có thể cải thiện thành tích học tập và phát triển kỹ năng học suốt đời, nhưng nhiều sinh viên thấy SRL khó. Educational chatbots có tiềm năng scaffold hoặc externally regulate quá trình SRL bằng cách tương tác adaptively. Tuy nhiên đến nay chưa có nghiên cứu nào xác định rõ chatbots đã (1) promote learning processes liên quan SRL như thế nào và (2) cải thiện performance ra sao. Nhóm thực hiện systematic literature review theo PRISMA với 27 publications từ 2012 đến 2023.

### Vì sao vấn đề này quan trọng

Đây là bài SLR mới và nóng nhất về chatbot trong giáo dục từ góc độ SRL. Self-regulated learning chính là cơ chế lý thuyết mà AI assistant chống trì hoãn cần dựa vào (theo Zimmerman's SRL cycle: forethought, performance, self-reflection). Bài này trực tiếp định vị được khoảng trống mà nhóm có thể khai thác.

### Gap (điểm thiếu sót)

1. **Gap quan trọng nhất:** Chatbots cho đến nay chủ yếu hỗ trợ sinh viên identify learning resources, enact learning strategies, và metacognitively monitor việc học. Hỗ trợ rất hạn chế trong việc giúp sinh viên set learning goals, create learning plans, reflect on past studying, và adapt cho future studying. Đây chính là chỗ trống cho hệ thống lập kế hoạch và can thiệp procrastination.
2. Mẫu nghiên cứu chỉ 27 bài, đa số là chatbot rule-based, ít LLM-based.
3. Một số intervention chatbot cho kết quả không có ý nghĩa thống kê hoặc kết quả mixed.
4. Không bài nào trong corpus tập trung explicitly vào procrastination intervention.
5. Không bài nào nghiên cứu trong bối cảnh sinh viên đại học Việt Nam.

---

## Bài 4

**Tên bài báo:** Development of a Mobile Intervention for Procrastination Augmented With a Semigenerative Chatbot for University Students: Pilot Randomized Controlled Trial

**Tác giả:** Seonmi Lee, Jaehyun Jeong, Myungsung Kim, Sangil Lee, Sung-Phil Kim, Dooyoung Jung

**Nguồn:** JMIR mHealth and uHealth (Q1 journal), Vol. 13, Article e53133, xuất bản 10/04/2025

**Link:** https://mhealth.jmir.org/2025/1/e53133

**DOI:** 10.2196/53133

**Trạng thái:** Peer-reviewed, open access

### Vấn đề thực tế trong bài

Procrastination ảnh hưởng tiêu cực đến học tập và sức khỏe tâm thần của sinh viên đại học. Các app quản lý thời gian truyền thống thiếu chiến lược trị liệu như CBT (cognitive behavioral therapy) để xử lý khía cạnh tâm lý của procrastination. Nhóm phát triển và tích hợp một semigenerative chatbot tên Moa vào một to-do app. Pilot RCT với 85 sinh viên (37 nữ, 48 nam) tại một đại học Hàn Quốc. Moa hướng dẫn người dùng trong 30 ngày qua 3 giai đoạn: self-observation, strategy establishment, reflection. Kiến trúc gồm response-generating algorithm và procrastination factor detection algorithm.

### Vì sao vấn đề này quan trọng

Bài khớp 100% với chủ đề của nhóm: AI chatbot chống trì hoãn tích hợp vào ứng dụng quản lý thời gian. Đây là bài bắt buộc đọc kỹ. Kết quả pilot RCT cho thấy Time Management Behavior Scale và Perceived Stress Scale cải thiện có ý nghĩa thống kê (P<.001 và P=.009) trong nhóm treatment, Pure Procrastination Scale cải thiện đáng kể ở hầu hết clusters.

### Gap (điểm thiếu sót)

1. Pilot study, sample nhỏ (85 sinh viên), thời gian ngắn (30 ngày). Chưa biết hiệu quả dài hạn.
2. Chỉ thực hiện ở Hàn Quốc, không có bối cảnh Đông Nam Á hay Việt Nam.
3. Không có RE elicitation rõ ràng từ sinh viên. Chatbot được thiết kế dựa trên lý thuyết CBT có sẵn, không phỏng vấn sinh viên trước khi thiết kế xem họ thực sự cần gì.
4. Architecture semi-generative, chưa khai thác full LLM (như GPT-4, Claude) để personalize sâu hơn.
5. Chỉ tập trung khía cạnh tâm lý của procrastination (CBT), chưa kết hợp adaptive scheduling dựa trên workload và deadlines thực tế của sinh viên đa môn học.
6. Không có module dự đoán procrastination bằng ML để cảnh báo sớm.

---

## Bài 5

**Tên bài báo:** Predictive analysis of college students' academic procrastination behavior based on a decision tree model

**Tác giả:** Xiangmei Zhu

**Nguồn:** Humanities and Social Sciences Communications (Nature Palgrave), Vol. 11, Article 869, xuất bản 03/07/2024

**Link:** https://www.nature.com/articles/s41599-024-03300-1

**DOI:** 10.1057/s41599-024-03300-1

**Trạng thái:** Peer-reviewed, open access, journal thuộc Nature group

### Vấn đề thực tế trong bài

Dự đoán academic procrastination trong bối cảnh khủng hoảng có thể cung cấp hỗ trợ học tập thiết yếu và chiến lược ra quyết định cho các trường đại học để bảo vệ sức khỏe tâm lý sinh viên. Nghiên cứu tập trung vào dự đoán procrastination trong bối cảnh khủng hoảng toàn cầu vẫn còn rất hạn chế. Tác giả xây dựng predictive model dùng decision tree algorithm, dữ liệu từ 776 sinh viên tại tỉnh Quảng Tây, Trung Quốc. Mô hình đạt accuracy 85.78%.

### Vì sao vấn đề này quan trọng

Cung cấp cơ sở định lượng cho việc dự đoán procrastination. Nhóm có thể tham chiếu 8 yếu tố dự đoán (subjective well-being, nghiện smartphone, cảm xúc tiêu cực, lòng tự trọng, tự chủ cuộc sống, pro-environmental behavior, academic performance, sense of school belonging) để thiết kế module cảnh báo sớm trong AI assistant.

### Gap (điểm thiếu sót)

1. Chỉ là predictive model, không có intervention. Biết được ai sẽ procrastinate nhưng không có công cụ giúp họ thay đổi hành vi.
2. Dùng decision tree truyền thống, không phải deep learning hay LLM. Mô hình có thể bị outdated khi dữ liệu thay đổi.
3. Bối cảnh Trung Quốc (Quảng Tây), văn hóa học tập khác Việt Nam. Không có bài nào nghiên cứu sinh viên VN với các yếu tố đặc thù như hệ tín chỉ, deadline cụm cuối kỳ.
4. Không đề cập đến AI assistant hay chatbot, chỉ là phân tích thuần tâm lý xã hội.
5. Không kết nối với mobile app hay reminder system. Kết quả nghiên cứu chưa được "hành động hoá" thành công cụ thực tế.
6. Yếu tố dự đoán dựa trên self-report questionnaire, không dùng behavioral data thực tế (như log usage app, submission patterns).

---

## Gap chung của 5 bài báo

Sau khi phân tích, có 3 layer gap chồng lên nhau rất rõ ràng:

### Gap 1: Functional gap (chức năng)

Mỗi bài giải quyết một mảnh riêng, chưa ai làm tổng thể tích hợp:

- Bài 2 (Murtaza): có content personalization, không có chống trì hoãn
- Bài 3 (Guan): chatbot SRL nhưng chưa hỗ trợ goal-setting và planning
- Bài 4 (Lee/Moa): chatbot chống trì hoãn nhưng không có ML prediction
- Bài 5 (Zhu): có ML prediction nhưng không có intervention

**Kết luận:** Chưa có hệ thống nào tích hợp đầy đủ Planning + Reminder + Procrastination Prediction + Behavioral Intervention + LLM Personalization.

### Gap 2: Methodological gap (phương pháp)

Thiếu requirements elicitation từ chính sinh viên:

- Bài 1 (Habiba): RE4AI generic, không có domain education
- Bài 2 (Murtaza): literature survey, không phỏng vấn sinh viên
- Bài 4 (Lee/Moa): design dựa trên CBT có sẵn, không elicit từ sinh viên
- Bài 5 (Zhu): chỉ phân tích định lượng, không có RE
- Bài 3 (Guan): SLR, không có primary elicitation

**Kết luận:** Chưa có bài nào dùng kỹ thuật RE chuẩn (interview, survey, prototyping) để elicit requirements cho AI assistant chống trì hoãn từ chính sinh viên là stakeholder.

### Gap 3: Contextual gap (bối cảnh)

Bối cảnh Đông Nam Á và Việt Nam vắng bóng hoàn toàn:

- Bài 1: phương Tây
- Bài 2: Pakistan và phương Tây
- Bài 3: chủ yếu Trung Quốc và phương Tây
- Bài 4: Hàn Quốc
- Bài 5: Trung Quốc

**Kết luận:** Không có bài nào nghiên cứu sinh viên đại học Việt Nam hoặc Đông Nam Á, nơi văn hóa học tín chỉ, áp lực deadline cụm cuối kỳ, và tần suất sử dụng smartphone rất cao.

---

## Định vị đề tài dựa trên gap chung

Mặc dù đã có các nghiên cứu riêng lẻ về AI cho personalized e-learning (Murtaza et al., 2022), chatbot hỗ trợ self-regulated learning (Guan et al., 2024), mobile chatbot can thiệp procrastination ngắn hạn (Lee et al., 2025), và ML model dự đoán procrastination (Zhu, 2024), vẫn chưa có nghiên cứu nào thực hiện requirements elicitation có hệ thống từ chính sinh viên cho một AI personal assistant tích hợp đầy đủ các chức năng: quản lý thời gian, dự đoán procrastination bằng ML, và can thiệp hành vi dựa trên CBT và self-regulation theory. Khoảng trống này đặc biệt nghiêm trọng trong bối cảnh sinh viên đại học Việt Nam, nơi chưa có nghiên cứu nào về requirements engineering cho hệ thống AI assistant chống trì hoãn.

---

## Bảng tổng hợp nhanh

| # | Tác giả | Năm | Nguồn | Vai trò trong literature review |
|---|---|---|---|---|
| 1 | Habiba et al. | 2024 | Requirements Engineering (Springer) | Nền tảng RE4AI |
| 2 | Murtaza et al. | 2022 | IEEE Access | Framework personalized e-learning |
| 3 | Guan et al. | 2024 | Education and Information Technologies (Springer) | Chatbot cho SRL, gap rõ về goal-setting |
| 4 | Lee et al. | 2025 | JMIR mHealth and uHealth | Chatbot can thiệp procrastination (khớp 100%) |
| 5 | Zhu | 2024 | Humanities and Social Sciences Communications (Nature) | ML prediction procrastination |

---

## Literature Review Matrix

| Paper | Year | Venue | Topic / Domain | Research Method | Context | Key Findings | Limitation | Relevance |
|---|---|---|---|---|---|---|---|---|
| Paper 1 | 2024 | Requirements Engineering (Springer) | Requirements Engineering for AI-based systems | Systematic mapping study (126 primary studies) | Generic AI systems, đa quốc gia | Thách thức phổ biến nhất: requirements specification, explainability, gap giữa ML engineers và end-users; đề xuất 7 hướng nghiên cứu | Generic, không có domain education; không có primary user study | High |
| Paper 2 | 2022 | IEEE Access | Personalized AI e-learning systems | Literature survey | Tổng hợp literature, bối cảnh phương Tây và Pakistan | Đề xuất framework 5 module cho personalized e-learning (Data, Adaptive, Adaptable, Recommender, Delivery) | Không có module planning hay reminder; chỉ "What to learn" | Medium |
| Paper 3 | 2024 | Education and Information Technologies (Springer) | Educational chatbots cho self-regulated learning | Systematic literature review theo PRISMA | 27 publications từ 2012-2023, đa quốc gia | Chatbots hỗ trợ tốt identify resources và monitor; hạn chế ở goal-setting, planning, reflection | Mẫu nhỏ 27 bài; ít LLM-based; không có procrastination focus | High |
| Paper 4 | 2025 | JMIR mHealth and uHealth | Mobile chatbot intervention chống procrastination | Pilot Randomized Controlled Trial | 85 sinh viên đại học Hàn Quốc, 30 ngày | Moa chatbot cải thiện Time Management, Perceived Stress, Pure Procrastination Scale có ý nghĩa thống kê (P<.01) | Pilot, sample nhỏ; không có RE elicitation; không có ML prediction | Very High |
| Paper 5 | 2024 | Humanities and Social Sciences Communications (Nature) | ML prediction academic procrastination | Quantitative (decision tree algorithm) | 776 sinh viên Quảng Tây, Trung Quốc | Model accuracy 85.78%; 8 yếu tố dự đoán, subjective well-being quan trọng nhất | Chỉ prediction không intervention; bối cảnh TQ; không kết nối AI assistant | Medium |