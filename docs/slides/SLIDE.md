Hãy đóng vai một Frontend Developer & Presentation Designer. Tạo cho tôi một ứng dụng web trình chiếu dạng Slide Deck trong một file duy nhất (`slide_18-11.html`, sử dụng HTML5, Tailwind CSS qua CDN và Vanilla JS) bằng tiếng Việt để tôi dùng cho buổi họp nội bộ của đội thi **Hack4Biz Competition 2026** vào tối nay (18/11/2026).

---

### 1. BỐI CẢNH VÀ TINH THẦN
- Đội gồm 5 thành viên: `1 BA (NEU)` và `4 Developers`. Các thành viên chưa có nhiều kinh nghiệm làm việc cùng nhau, muốn tận dụng cuộc thi để cọ xát, học hỏi và thử sức với một bài toán thực tế.
- Đội có mục tiêu tham gia nghiêm túc, nhưng không phô trương tham vọng bằng các khẩu hiệu lớn.
- **Tinh thần xuyên suốt:** Thực tế, rõ ràng, tập trung vào công việc; chuyên nghiệp nhưng không cứng nhắc; ngôn ngữ tự nhiên như một thành viên trong đội trao đổi với những người còn lại. Mỗi slide phải giúp người nghe hiểu rõ một vấn đề hoặc thống nhất một quyết định cụ thể.
- Đây không phải pitch deck gọi vốn, không phải bài truyền cảm hứng và không phải tài liệu quảng bá cuộc thi.

---

### 2. NGUYÊN TẮC BIÊN TẬP NỘI DUNG
- **Tuyệt đối không** dùng các cụm từ mang tính khẩu hiệu, sáo rỗng hoặc cố tạo cảm giác hoành tráng (ví dụ: *Recode the DNA, Hành trình chinh phục Top 4, Kích hoạt chế độ try-hard, All in, Anh em chiến thôi...*). Không tự sáng tác slogan thay thế.
- **Tiêu đề & Câu chữ:** Tiêu đề ngắn gọn, nói thẳng nội dung chính. Câu văn trực tiếp, hạn chế tính từ, ưu tiên bullet point thay cho đoạn văn dài.
- **Thuật ngữ:** Không chèn tiếng Anh vào mọi tiêu đề. Chỉ dùng tiếng Anh cho thuật ngữ chuyên môn thực sự cần thiết như *Agile Scrum, MVP, Backlog, User Story, Acceptance Criteria, Definition of Done, RAG, Tool Calling, Guardrails, Change Request*.
- **Tính chính xác:** Giữ nguyên toàn bộ thông tin, mốc thời gian, yêu cầu và tiêu chuẩn nghiệm thu đã cung cấp. Không tự thêm giả định mới.

---

### 3. NGUYÊN TẮC THIẾT KẾ & KỸ THUẬT (MINIMALIST EDITORIAL / TECHNICAL)
- **Bảng màu & Kỷ luật 90/10:**
  - Background: `#090D16` | Surface: `#111827` | Text chính: `#F8FAFC` | Text phụ: `#94A3B8` (chiếm 90% diện tích).
  - Emerald (`#10B981`): chỉ dùng cho điểm chốt quan trọng nhất, trạng thái hoàn thành hoặc hành động chính.
  - Cyan (`#06B6D4`): chỉ dùng cho nhãn kỹ thuật, mốc thời gian hoặc luồng dữ liệu phụ. Không đặt hai màu này cạnh nhau gây rối mắt.
- **Tiết chế hiệu ứng:** Không lạm dụng gradient, neon glow, glassmorphism, đường line trang trí vô nghĩa, hay gắn icon/badge ở mọi thành phần. Không biến toàn bộ presentation thành một dashboard lặp lại cùng một kiểu card.
- **Typography & Cỡ chữ họp online:**
  - Dùng Google Fonts `Be Vietnam Pro` cho tiêu đề/nội dung và `JetBrains Mono` (`tabular-nums`) cho toàn bộ ngày tháng, thời lượng và số thứ tự.
  - Tiêu đề slide: `28px – 36px` (Bold), căn trái nhất quán. Nội dung chính tối thiểu `16px – 18px`, line-height `1.5 – 1.6`, giới hạn độ dài dòng khoảng `65 – 75 ký tự` để dễ đọc khi share màn hình.
- **Bố cục chuẩn 16:9 & Đa dạng layout:**
  - Mỗi slide gói gọn trong khung nhìn `100vh` (`overflow: hidden` ở khung chính), tuyệt đối không để tràn chữ hay xuất hiện thanh cuộn dọc.
  - Giữ tối thiểu 30% khoảng trắng để nội dung tự tách lớp mà không cần đóng khung card cho mọi khối. Thay đổi bố cục linh hoạt giữa các slide (chia cột, sơ đồ luồng, bảng biểu, danh sách).
- **Quy chuẩn Sơ đồ & Bảng biểu:**
  - Sơ đồ quy trình (Agile Scrum, lộ trình 4 chặng): dùng khối nền `#111827`, viền mảnh `1px solid #1F2937` và mũi tên nối đơn giản.
  - Bảng biểu: bỏ kẻ sọc zebra, chỉ dùng đường kẻ ngang mảnh `1px solid #1F2937` giữa các hàng, căn trái toàn bộ chữ.
- **Điều hướng & Tương tác trực tiếp (`localStorage`):**
  - Chuyển slide bằng phím `ArrowRight`, `ArrowLeft`, `Space`, hoặc nút bấm góc dưới. Thanh tiến trình mỏng ở cạnh trên, số trang (`01 / 13`) và nút phím tắt đặt nhỏ gọn, độ mờ thấp ở góc dưới để không tranh chấp thị giác.
  - Phím `F` bật/tắt Fullscreen; phím `G` hoặc nút lưới mở chế độ xem tổng quan 13 slide.
  - Tại **Slide 09** và **Slide 13**, thiết kế các ô `input` và `select` tối giản hòa nhập vào bảng (nền `#090D16`, viền mảnh `#334155`, đổi viền sang `#10B981` khi focus) để nhập và lưu trực tiếp ngay khi đang họp.

---

### 4. NỘI DUNG CHI TIẾT 13 SLIDES

**Slide 01: Trang bìa**
- **Tiêu đề chính:** Triển Khai Đội Thi Hack4Biz 2026
- **Thông tin phụ:** Ngày họp: 18/11/2026 • Team: 5 thành viên (1 BA + 4 Dev) • Hạn đăng ký: 22/11/2026

**Slide 02: Nội dung buổi họp**
- Trình bày 4 mục chính của buổi họp:
  1. **Mục 1:** Giới thiệu thành viên & Cách làm việc chung.
  2. **Mục 2:** Tổng quan cuộc thi, cấu trúc Agile Scrum & Chi tiết 5 Role.
  3. **Mục 3:** Chọn Role & Chia vai thi Vòng 1.
  4. **Mục 4:** Kế hoạch ôn tập & Phân việc tuần đầu (Vòng 1).

**Slide 03: Cách làm việc chung**
- **Bối cảnh:** 5 người lần đầu làm việc chung và cũng mới tiếp cận cuộc thi này, thống nhất 3 nguyên tắc cơ bản để dễ phối hợp:
  - **Phản hồi tin nhắn:** Cố gắng phản hồi nhóm trong vòng `2 tiếng` (khung `08:00 – 23:00`). Bận việc đột xuất thì nhắn báo trước một câu để cả nhóm chủ động.
  - **Thời gian:** Thu xếp khoảng `1.5 – 2 tiếng/ngày` từ nay đến 27/11 để xem tài liệu và làm phần việc được chia.
  - **Trao đổi:** Không rõ phần nào thì hỏi luôn để cả nhóm cùng gỡ, góp ý trực tiếp vào công việc trên tinh thần hỗ trợ nhau.

**Slide 04: Tổng quan Hack4Biz 2026 & Lộ trình 3 vòng**
- **Thông tin chung:** Mô phỏng quy trình làm sản phẩm theo **Agile Scrum**, ứng dụng **AI Agent** giải bài toán Ngân hàng của **VPBank** (BUV tổ chức).
- **3 Vòng thi:**
  - **Vòng 1 – Online Assessment (27/11/2026):** Thi trắc nghiệm kiến thức chuyên môn từng Role + Agile Scrum. Lấy **Top 20** cho **Vòng 2**.
  - **Vòng 2 – MVP Building (08/12 – 23/12/2026):** Nộp bộ tài liệu phân tích nghiệp vụ (BRD, sơ đồ luồng) + Code bản **MVP AI Agent** chạy được. Lấy **Top 4** cho **Vòng 3**.
  - **Vòng 3 – 32h Hackathon (09/01 – 10/01/2027):** Thi Offline tại BUV (Ecopark). Nhận **Change Request (CR)** từ BTC, code bổ sung trực tiếp trên source Vòng 2 và thuyết trình.

**Slide 05: Cấu trúc Agile Scrum – Khung cốt lõi (3-5-3)**
- Trình bày theo 3 cột chuẩn Scrum Guide:
  1. **3 Vai trò (Scrum Roles):**
     - **Product Owner (PO):** Tối đa hóa giá trị sản phẩm, quản lý và sắp xếp thứ tự ưu tiên *Product Backlog*.
     - **Scrum Master (gắn với PM):** Đảm bảo team hiểu và chạy đúng quy trình Scrum, gỡ bỏ trở ngại cho team.
     - **Developers (bao gồm BA, Dev, QA):** Tự tổ chức để biến các mục trong Backlog thành sản phẩm chạy được sau mỗi Sprint.
  2. **5 Sự kiện (Scrum Events):**
     - **Sprint:** Chu kỳ lặp cố định (1–4 tuần; ở Vòng 2 chia làm 2 Sprint, mỗi Sprint 7 ngày) để tạo ra bản tăng trưởng sản phẩm.
     - **Sprint Planning:** Họp đầu Sprint để chốt *Sprint Goal*, chọn task từ Product Backlog sang Sprint Backlog và chia việc.
     - **Daily Scrum:** Họp ngắn 15 phút mỗi ngày để đồng bộ tiến độ (Hôm qua làm gì – Hôm nay làm gì – Có vướng gì không).
     - **Sprint Review:** Cuối Sprint demo tính năng đã làm được cho Stakeholder/PO nghiệm thu và lấy phản hồi.
     - **Sprint Retrospective:** Họp nội bộ cuối Sprint để nhìn lại cách làm việc nhóm, rút kinh nghiệm cải tiến cho Sprint sau.
  3. **3 Tạo tác (Scrum Artifacts):**
     - **Product Backlog:** Danh sách toàn bộ tính năng, yêu cầu của sản phẩm được xếp theo độ ưu tiên (do PO quản lý).
     - **Sprint Backlog:** Tập hợp các task được chọn từ Product Backlog để làm trong Sprint hiện tại kèm kế hoạch thực hiện.
     - **Increment (Bản tăng trưởng):** Phần sản phẩm hoàn chỉnh, chạy được và đạt tiêu chuẩn *Definition of Done* sau mỗi Sprint.

**Slide 06: Cấu trúc Agile Scrum – Luồng vận hành & Khái niệm trọng tâm**
- **Sơ đồ luồng chạy 1 vòng Sprint:** `Product Backlog` -> `Sprint Planning` -> `Sprint Backlog` -> `Thực thi & Daily Scrum (15p/ngày)` -> `Increment` -> `Sprint Review (Demo)` -> `Sprint Retrospective`.
- **Các khái niệm & chỉ số thường gặp trong bài thi Vòng 1:**
  - **User Story & Acceptance Criteria (AC):** Mô tả tính năng dưới góc nhìn người dùng (*"Là [ai], tôi muốn [làm gì], để [đạt lợi ích gì]"*) kèm điều kiện nghiệm thu rõ ràng (thường viết theo chuẩn *Given - When - Then*).
  - **Story Points & Planning Poker:** Đơn vị ước lượng độ phức tạp/công sức của task (dùng dãy Fibonacci: 1, 2, 3, 5, 8, 13...) thay vì đoán giờ tuyệt đối.
  - **Velocity (Vận tốc):** Tổng số Story Points team hoàn thành trung bình trong 1 Sprint -> dùng để dự đoán khả năng nhận việc ở Sprint tiếp theo.
  - **Definition of Done (DoD) vs. Definition of Ready (DoR):** *DoR* là tiêu chuẩn để 1 task đủ điều kiện đưa vào Sprint; *DoD* là tiêu chuẩn bắt buộc (code xong, review, test pass, có tài liệu) để tính là hoàn thành.
  - **Burndown Chart:** Biểu đồ theo dõi lượng công việc (Story Points) còn lại theo từng ngày trong Sprint.

**Slide 07: Chi tiết công việc 5 Role – Khối Nghiệp vụ & Quản lý (BA, PO, PM)**
- Trình bày 3 cột nhiệm vụ cụ thể và kiến thức trọng tâm Vòng 1:
  1. **BA (Business Analyst – Phân tích nghiệp vụ):**
     - *Vai trò:* Cầu nối giữa bài toán kinh doanh của ngân hàng (VPBank) và đội ngũ kỹ thuật.
     - *Công việc cụ thể:* Khảo sát và làm rõ yêu cầu nghiệp vụ; viết tài liệu **BRD (Business Requirements Document)**, **SRS**; phân rã thành **User Stories** (chuẩn INVEST) và **Acceptance Criteria**; vẽ sơ đồ trực quan (**Business Flow / BPMN**, **Use Case Diagram**, **Sequence Diagram**, Wireframe cơ bản).
  2. **PO (Product Owner – Chủ sở hữu sản phẩm):**
     - *Vai trò:* Định hướng "Làm cái gì" và "Làm cái nào trước" để sản phẩm mang lại giá trị cao nhất.
     - *Công việc cụ thể:* Xây dựng tầm nhìn sản phẩm (Product Vision); quản lý **Product Backlog**; sắp xếp độ ưu tiên tính năng theo các khung **MoSCoW** (*Must-have, Should-have, Could-have, Won't-have*) hoặc **RICE / Value vs. Effort**; làm việc với Stakeholder và nghiệm thu sản phẩm ở Sprint Review.
  3. **PM (Project Manager – Quản lý dự án / Scrum Master):**
     - *Vai trò:* Giữ nhịp độ, điều phối nguồn lực và đảm bảo dự án về đích đúng hạn.
     - *Công việc cụ thể:* Lập kế hoạch tổng thể (Timeline/Milestone), phân bổ nhân sự, theo dõi tiến độ qua **Burndown/Burnup Chart**; quản trị rủi ro (Risk Register) và xử lý điểm nghẽn; tổ chức các buổi họp Scrum và đảm bảo team tuân thủ quy trình Agile.

**Slide 08: Chi tiết công việc 5 Role – Khối Kỹ thuật & Chất lượng (DEV, QA)**
- Trình bày 2 cột chi tiết DEV & QA + phần phối hợp chéo:
  1. **DEV (Developer – Kỹ sư phát triển):**
     - *Vai trò:* Hiện thực hóa giải pháp và tài liệu nghiệp vụ thành hệ thống AI Agent chạy thực tế.
     - *Công việc cụ thể:* Thiết kế kiến trúc hệ thống (System Architecture), thiết kế Database và **RESTful API**; lập trình luồng AI Agent (RAG, Tool Calling, Guardrails) và giao diện; quản lý mã nguồn qua **Git Flow**, CI/CD; tự ước lượng task (Story Points) và xử lý **Change Request** ở Vòng 3.
  2. **QA (Quality Assurance / Tester – Đảm bảo chất lượng):**
     - *Vai trò:* Kiểm soát chất lượng, phát hiện lỗi sớm và đảm bảo sản phẩm chạy đúng yêu cầu nghiệp vụ.
     - *Công việc cụ thể:* Dựa vào BRD và Acceptance Criteria để viết **Test Plan**, **Test Case** (gồm happy case và edge case); thực hiện các cấp độ kiểm thử (**Unit, Integration, System, UAT**); quản lý vòng đời lỗi (**Bug Life Cycle**); kiểm thử độ chính xác và khả năng chống bịa đặt (hallucination) của AI.
- **Luồng phối hợp 5 Role:** BA làm rõ bài toán & vẽ luồng -> PO chốt tính năng ưu tiên -> PM chia Sprint & giữ tiến độ -> DEV dựng kiến trúc & code AI Agent -> QA kiểm thử bám sát AC của BA. *(Ở Vòng 2 & 3, cả 4 thành viên Dev sẽ cùng tham gia code).*

**Slide 09: Chọn Role & Chia vai Vòng 1 (Interactive Slide)**
- **Quy tắc:** Ghế **BA** đã chốt cho thành viên NEU. 4 thành viên Dev chọn **tối đa 2 nguyện vọng** trong 4 vị trí: `PM`, `PO`, `DEV`, `QA`.
- **Bảng nhập liệu trực tiếp (5 dòng: BA + 4 Dev):** Gồm ô nhập `Tên thành viên`, dropdown `Nguyện vọng 1`, dropdown `Nguyện vọng 2`, và dropdown `Chốt Role Vòng 1` (có nút Reset bảng).
- **Ghi chú:** *"Role này dùng để đăng ký hồ sơ và làm bài test Vòng 1 (27/11). Sang Vòng 2 & 3, cả 4 thành viên Dev đều cùng tham gia thiết kế và code AI Agent."*

**Slide 10: Lộ trình 4 chặng xuyên suốt cuộc thi**
- Trình bày dạng sơ đồ/bảng 4 chặng rõ ràng:
  - **Chặng 1 (18/11 – 27/11 | 9 ngày):** *Ôn thi Vòng 1.* Tập trung ôn Agile Scrum và kiến thức từng Role cho bài test online ngày 27/11.
  - **Chặng 2 (28/11 – 07/12 | 10 ngày):** *Làm quen AI Agent & Dựng khung dự án.* 4 Dev thực hành Cursor/Claude Code theo hướng Spec-driven, dựng sẵn Boilerplate (FastAPI + LangGraph/OpenAI SDK + RAG). BA tìm hiểu trước hệ sinh thái sản phẩm VPBank.
  - **Chặng 3 (08/12 – 23/12 | 16 ngày):** *Vòng 2 – Build MVP.* Chia 2 Sprint (7 ngày/Sprint). Hoàn thiện BRD + Code MVP + Quay video demo.
  - **Chặng 4 (24/12 – 10/01/2027):** *Vòng 3 – 32h Hackathon.* Dọn gọn source code Vòng 2, viết file `ARCHITECTURE.md` để AI hỗ trợ sửa code nhanh khi nhận Change Request tại BUV.

**Slide 11: Lịch công việc & Ôn tập cụ thể Tuần 1 (19/11 – 26/11)**
- Bảng 4 cột (`Thời gian` | `Đầu việc` | `Phụ trách` | `Kết quả đầu ra`):
  - **19/11 (Mai):** Nộp đơn đăng ký sớm (hạn 22/11) & tạo Notion/GitHub/Discord | *PM + Cả đội* | Gửi ảnh xác nhận nộp form thành công vào nhóm.
  - **20/11 – 21/11:** Ôn kỹ khung Agile Scrum (3 Roles, 5 Events, 3 Artifacts, Story Points, DoD) | *Cả 5 người* | Ghi chú sơ đồ quy trình Scrum lên Notion.
  - **22/11 – 23/11:** Ôn chuyên sâu kiến thức theo từng Role đã chốt (BA, PO, PM, DEV, QA) | *Từng Role* | Nộp bản tóm tắt 1–2 trang A4 lên Notion để đọc chéo.
  - **24/11:** Mỗi người tự soạn 20 câu trắc nghiệm tình huống của vị trí mình | *Cả 5 người* | Tổng hợp đủ bộ 100 câu trên Quizizz / Forms.
  - **25/11 (Tối):** Làm thử bộ 100 câu & họp chữa chéo các câu sai | *Cả đội* | Nắm chắc mảng chính & hiểu góc nhìn các Role khác.
  - **26/11 (Tối):** Rà soát lại các phần còn hổng & test mic/mạng | *Cả đội* | Sẵn sàng trước giờ thi online ngày 27/11.

**Slide 12: Hướng tiếp cận AI Agent cho 4 Dev (Sau 27/11)**
- Cách triển khai để kiểm soát được mã nguồn khi chưa có nhiều kinh nghiệm vibecoding / agentic coding:
  - **Quy trình Spec-Driven:** Tự viết file `specs.md` (mô tả API, DB schema, luồng dữ liệu) -> Dùng Cursor/Windsurf/Claude Code sinh code từng module nhỏ -> Tự review code, test cục bộ và commit Git liên tục.
  - **Tech Stack gợi ý:**
    - *Backend & Agent:* Python (`FastAPI`), `LangGraph` hoặc `OpenAI Agents SDK`.
    - *Kỹ thuật chính:* `RAG` (tra cứu tài liệu), `Tool Calling` (gọi API nghiệp vụ), `Guardrails` (kiểm soát câu trả lời đúng phạm vi).
    - *Frontend:* `Next.js` hoặc `Chainlit / Streamlit` để dựng giao diện demo nhanh.

**Slide 13: Chốt thông tin & Việc cần làm ngay (Interactive Slide)**
- **Bảng điền nhanh thông tin đăng ký (5 dòng):** Tự động đồng bộ Role từ Slide 09, gồm các ô nhập `Họ tên`, `Ngày sinh`, `Trường / MSSV`, `SĐT`, `Email` + nút `Copy thông tin`.
- **Ô nhập khung giờ check-in tối (10–15p):** Mặc định `22:30` (cho phép chỉnh sửa trực tiếp).
- **3 việc chốt trước khi nghỉ:**
  1. Chốt danh sách Role chính thức của 5 thành viên.
  2. Điền đủ thông tin trên để ngày mai nộp đơn đăng ký.
  3. Tối mai bắt đầu check-in ngắn theo giờ đã chốt.