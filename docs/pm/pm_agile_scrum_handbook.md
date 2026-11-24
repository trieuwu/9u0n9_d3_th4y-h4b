# CẨM NANG CHUYÊN SÂU: PROJECT MANAGER & AGILE SCRUM TRONG PHÁT TRIỂN SẢN PHẨM AI / PHẦN MỀM

- **Bối cảnh áp dụng:** Cuộc thi **Hack4Biz Competition 2026** (Xây dựng MVP AI Agent giải quyết bài toán Ngân hàng cho **VPBank**)
- **Cấu trúc Đội nhóm (5 thành viên):** Project Manager (`PM` / kiêm `Scrum Master` trong mô hình Hybrid), Product Owner (`PO`), Business Analyst (`BA`), Developer (`DEV`), Quality Assurance (`QA`)
- **Phiên bản chuẩn hóa:** `v1.0` — Cập nhật theo **Scrum Guide 2020**, **PMI-ACP** & **ISTQB v4.0**
- **Mục tiêu tài liệu:**
  1. **Ôn luyện lý thuyết & tư duy xử lý tình huống chuyên sâu** cho Vòng 1 (Online Assessment — `27/11/2026`).
  2. **Cẩm nang vận hành thực chiến (Playbook)** cho Vòng 2 (`08/12 – 23/12/2026`: 16 ngày xây dựng MVP) và Vòng 3 (`09/01 – 10/01/2027`: 32 giờ Hackathon xử lý Change Request).

---

## MỤC LỤC TRA CỨU NHANH

1. [**PHẦN 1: Nền tảng & Cấu trúc chuẩn của Agile Scrum (Scrum Guide 2020)**](#phần-1-nền-tảng--cấu-trúc-chuẩn-của-agile-scrum-theo-scrum-guide-mới-nhất---2020)
   - [1.1. Bản chất Agile & Empiricism (Chủ nghĩa Thực nghiệm)](#11-bản-chất-agile--empiricism-chủ-nghĩa-thực-nghiệm)
   - [1.2. So sánh Phương pháp luận: Waterfall vs. Scrum vs. Kanban](#12-so-sánh-phương-pháp-luận-waterfall-vs-scrum-vs-kanban)
   - [1.3. 3 Vai trò trong Scrum (Scrum Accountabilities)](#13-3-vai-trò-trong-scrum-scrum-accountabilities)
   - [1.4. 5 Sự kiện trong Scrum (Scrum Events)](#14-5-sự-kiện-trong-scrum-scrum-events)
   - [1.5. 3 Tạo tác & Cam kết đi kèm (Scrum Artifacts & Commitments)](#15-3-tạo-tác--cam-kết-đi-kèm-scrum-artifacts--commitments)
2. [**PHẦN 2: Công cụ, Chỉ số & Kỹ thuật Quản lý trong Agile Scrum**](#phần-2-công-cụ-chỉ-số--kỹ-thuật-quản-lý-trong-agile-scrum)
   - [2.1. Ước lượng & Lập kế hoạch (Story Points, Planning Poker, Velocity, Capacity)](#21-ước-lượng--lập-kế-hoạch-estimation--planning)
   - [2.2. Biểu đồ Theo dõi Tiến độ & Phát hiện Điểm nghẽn (Burndown, Burnup, CFD)](#22-biểu-đồ-theo-dõi-tiến-độ--phát-hiện-điểm-nghẽn-bottlenecks)
   - [2.3. Tiêu chuẩn Chất lượng & Quản lý Backlog (DoR vs. DoD, INVEST, MoSCoW, RICE)](#23-tiêu-chuẩn-chất-lượng--quản-lý-backlog)
3. [**PHẦN 3: Vai trò & Nghiệp vụ Chuyên sâu của Project Manager (PM) trong Agile Hybrid**](#phần-3-vai-trò--nghiệp-vụ-chuyên-sâu-của-project-manager-pm-trong-môi-trường-agile-hybrid)
   - [3.1. Giải mã "Bẫy Đề Thi": PM Truyền thống vs. Scrum Master / PO & Ma trận RACI](#31-giải-mã-bẫy-đề-thi-sự-khác-biệt-giữa-pm-truyền-thống-vs-scrum-master--po--mô-hình-agile-hybrid)
   - [3.2. Các mảng Nghiệp vụ Cốt lõi của PM (Scope/CR, Critical Path, Risk 4T, Stakeholder)](#32-các-mảng-nghiệp-vụ-cốt-lõi-của-project-manager-pm)
4. [**PHẦN 4: Bộ 25 Câu hỏi Trắc nghiệm Tình huống Ôn thi Vòng 1 (Có giải thích chi tiết)**](#phần-4-bộ-25-câu-hỏi-trắc-nghiệm-tình-huống-ôn-thi-vòng-1-có-giải-thích-chi-tiết)
5. [**PHẦN 5: Bộ Template Thực chiến cho Team Hack4Biz (Vòng 2 & Vòng 3)**](#phần-5-bộ-template-thực-chiến-cho-team-hack4biz-vòng-2--vòng-3)
   - [5.1. Mẫu Kế hoạch 2 Sprint cho Vòng 2 (16 Ngày Build MVP AI Agent)](#51-mẫu-kế-hoạch-2-sprint-cho-vòng-2-16-ngày-build-mvp-ai-agent)
   - [5.2. Mẫu Risk Register Đặc thù cho Dự án AI Agent Ngân hàng (VPBank)](#52-mẫu-risk-register-đặc-thù-cho-dự-án-ai-agent-ngân-hàng-vpbank)
   - [5.3. Checklist & Quy trình 5 Bước Xử lý Change Request trong 32h Hackathon (Vòng 3)](#53-checklist--quy-trình-5-bước-xử-lý-change-request-cr-trong-32h-hackathon-vòng-3)

---

## PHẦN 1: NỀN TẢNG & CẤU TRÚC CHUẨN CỦA AGILE SCRUM (THEO SCRUM GUIDE MỚI NHẤT - 2020)

### 1.1. Bản chất Agile & Empiricism (Chủ nghĩa Thực nghiệm)

Scrum không phải là một quy trình cứng nhắc (prescriptive process) mà là một **khung làm việc nhẹ (lightweight framework)** giúp con người, đội nhóm và tổ chức tạo ra giá trị thông qua các giải pháp thích ứng cho các bài toán phức tạp (complex problems) — đặc biệt phù hợp với bài toán phát triển **AI Agent** vốn có độ bất định cao về chất lượng mô hình (LLM behavior), dữ liệu và trải nghiệm người dùng ngân hàng.

#### A. 4 Giá trị cốt lõi của Tuyên ngôn Agile (Agile Manifesto Values)

| Giá trị được ưu tiên hơn (Bên trái) | So với | Giá trị vẫn quan trọng nhưng ưu tiên thấp hơn (Bên phải) | Áp dụng thực tế trong dự án AI Agent (Hack4Biz) |
| :--- | :---: | :--- | :--- |
| **Individuals and interactions** (Cá nhân và sự tương tác) | **>** | *Processes and tools* (Quy trình và công cụ) | BA, DEV, QA ngồi trao đổi trực tiếp 5 phút để chốt luồng Prompt/API thay vì chờ phê duyệt tài liệu qua lại trên Jira. |
| **Working software** (Phần mềm chạy được) | **>** | *Comprehensive documentation* (Tài liệu đầy đủ) | Một bản Demo AI Agent trả lời đúng nghiệp vụ thẻ tín dụng VPBank có giá trị hơn bộ BRD 100 trang nhưng code chưa chạy. |
| **Customer collaboration** (Hợp tác với khách hàng) | **>** | *Contract negotiation* (Đàm phán hợp đồng) | PO liên tục lấy phản hồi từ Mentor/Giám khảo VPBank để tinh chỉnh tính năng thay vì bám cứng vào đề xuất ban đầu. |
| **Responding to change** (Phản hồi với sự thay đổi) | **>** | *Following a plan* (Bám sát kế hoạch) | Ở Vòng 3 (32h Hackathon), khi Ban Tổ chức tung Change Request (CR), team linh hoạt tái cấu trúc Backlog để thích ứng. |

> **Lưu ý bẫy đề thi:** Tuyên ngôn Agile khẳng định *"Mặc dù các mục ở bên phải vẫn có giá trị, chúng tôi đánh giá các mục ở bên trái cao hơn"*. Agile **KHÔNG** bỏ tài liệu, **KHÔNG** bỏ lập kế hoạch.

#### B. 3 Trụ cột của Chủ nghĩa Thực nghiệm (Three Pillars of Empiricism)

Scrum được xây dựng trên nền tảng **Empiricism** (kiến thức đến từ kinh nghiệm thực tế và việc ra quyết định dựa trên những gì đã quan sát được) kết hợp với **Lean Thinking** (giảm thiểu lãng phí, tập trung vào bản chất).

```text
                  +-----------------------------------+
                  |           EMPIRICISM              |
                  |     (Chủ nghĩa Thực nghiệm)       |
                  +-----------------------------------+
                    /               |               \
                   /                |                \
                  v                 v                 v
      +------------------+ +------------------+ +------------------+
      |  1. TRANSPARENCY | |  2. INSPECTION   | |  3. ADAPTATION   |
      |   (Minh bạch)    | |   (Thanh tra)    | |   (Thích ứng)    |
      +------------------+ +------------------+ +------------------+
      Hiển thị đúng thực   Kiểm tra Artifacts   Điều chỉnh ngay khi
      trạng công việc &    & tiến độ hướng tới  phát hiện sai lệch
      dùng chung chuẩn     Goal để tìm sai      vượt ngưỡng cho phép
      (VD: DoD rõ ràng).   lệch (Variances).    (tối ưu quy trình/SP).
```

1. **Transparency (Minh bạch):** Các khía cạnh quan trọng của quy trình và công việc phải hiển thị rõ ràng với cả người thực hiện lẫn người tiếp nhận kết quả. Công cụ đảm bảo minh bạch: Ngôn ngữ chung, bảng Task/Burndown cập nhật thực tế, và đặc biệt là **Definition of Done (DoD)**. *Không có Minh bạch thì Thanh tra chỉ là ảo tưởng.*
2. **Inspection (Thanh tra):** Các Scrum Artifacts và tiến độ hướng tới các Goal phải được thanh tra thường xuyên và cẩn trọng để phát hiện các sai lệch hoặc vấn đề không mong muốn. Việc thanh tra được thực hiện thông qua **5 sự kiện của Scrum**. *Không có Thanh tra thì không biết cần Thích ứng ở đâu.*
3. **Adaptation (Thích ứng):** Nếu bất kỳ khía cạnh nào của quy trình lệch khỏi giới hạn chấp nhận được hoặc sản phẩm không đạt yêu cầu, quy trình hoặc tài liệu đang xử lý phải được điều chỉnh **càng sớm càng tốt**. Việc thích ứng trở nên dễ dàng nhất khi Scrum Team được trao quyền (empowered) và tự quản lý (self-managing).

#### C. 5 Giá trị của Scrum (Five Scrum Values)

Thành công của Scrum phụ thuộc vào việc các thành viên sống và làm việc theo 5 giá trị:
* **Commitment (Cam kết):** Scrum Team cam kết đạt được mục tiêu chung (Product Goal, Sprint Goal) và hỗ trợ lẫn nhau, **không phải** cam kết cứng nhắc phải hoàn thành 100% số lượng task bằng mọi giá bất chấp chất lượng.
* **Focus (Tập trung):** Toàn bộ tâm lực tập trung vào công việc của Sprint hiện tại để tạo ra tiến bộ tốt nhất hướng tới Sprint Goal (tránh đa nhiệm - multitasking hoặc làm tính năng ngoài luồng).
* **Openness (Cởi mở):** Scrum Team và các Stakeholders cởi mở về công việc và các thách thức đang gặp phải (ví dụ: DEV thẳng thắn báo cáo mô hình LLM đang bị Hallucination thay vì giấu lỗi).
* **Respect (Tôn trọng):** Các thành viên tôn trọng năng lực, sự độc lập và góc nhìn chuyên môn của nhau (DEV không coi thường QA, PO không áp đặt thời gian ước lượng lên DEV).
* **Courage (Dũng cảm):** Có dũng khí để làm điều đúng đắn, giải quyết các bài toán khó, dám nói "Không" với các yêu cầu làm vỡ Sprint Goal hoặc vi phạm tiêu chuẩn bảo mật ngân hàng.

---

### 1.2. So sánh Phương pháp luận: Waterfall vs. Scrum vs. Kanban

| Tiêu chí đối chiếu | Waterfall (Thác nước) | Agile Scrum | Agile Kanban |
| :--- | :--- | :--- | :--- |
| **Triết lý cốt lõi** | **Predictive** (Dự đoán trước): Lập kế hoạch chi tiết từ đầu, thực thi tuần tự từng pha. | **Iterative & Incremental** (Lặp và Tăng trưởng) theo các khung thời gian cố định (Sprints). | **Continuous Flow** (Luồng liên tục): Tối ưu hóa dòng chảy công việc và giới hạn WIP. |
| **Khi nào nên áp dụng (Use Case)** | Yêu cầu đã rõ ràng 100%, ít thay đổi, công nghệ đã quen thuộc, quy định pháp lý bắt buộc chốt cứng thiết kế từ đầu. | Bài toán phức tạp (Complex), yêu cầu cần khám phá/thử nghiệm dần (như xây dựng sản phẩm AI mới, MVP). | Vận hành, bảo trì (Maintenance), xử lý ticket hỗ trợ, hoặc luồng việc đến liên tục không theo chu kỳ cố định. |
| **Cách xử lý thay đổi yêu cầu (Change)** | Hạn chế tối đa. Thay đổi ở pha sau rất tốn kém, phải qua quy trình Change Control Board (CCB) nặng nề. | Không nhận thay đổi làm nguy hại đến **Sprint Goal** đang chạy; đưa yêu cầu mới vào Product Backlog cho Sprint sau (hoặc PO thương lượng đổi item tương đương nếu chưa làm). | Rất linh hoạt. Có thể thêm hoặc đổi độ ưu tiên ở cột *To Do* bất cứ lúc nào miễn là cột thực thi còn trống **WIP Limit**. |
| **Nhịp độ bàn giao (Delivery Cadence)** | Bàn giao 1 lần duy nhất ở cuối dự án (Big Bang Release). | Bàn giao **Increment** khả dụng sau mỗi Sprint (tối đa 1 tháng hoặc ngắn hơn: 1–2 tuần). | Bàn giao liên tục (Continuous Delivery) ngay khi từng hạng mục hoàn tất. |
| **Đơn vị kiểm soát chính** | Phạm vi cố định (Fixed Scope), quản lý theo Gantt Chart & WBS. | **Timebox** (Khung thời gian cố định) và **Sprint Goal**. | **WIP Limit** (Giới hạn số việc đang làm cùng lúc trên mỗi cột trạng thái). |
| **Chỉ số đo lường chính** | Earned Value Management (CPI, SPI), Milestone variance. | **Velocity** (Story Points/Sprint), Sprint Burndown. | **Lead Time**, **Cycle Time**, Throughput, Cumulative Flow Diagram (CFD). |
| **Vai trò bắt buộc** | Project Manager, BA, Architect, Dev, Tester... | **Product Owner, Scrum Master, Developers** (3 vai trò chuẩn). | Không bắt buộc vai trò mới (giữ nguyên cấu trúc tổ chức hiện tại). |

---

### 1.3. 3 Vai trò trong Scrum (Scrum Accountabilities)

Trong **Scrum Guide 2020**, thuật ngữ *"Roles"* được đổi thành **"Accountabilities"** (Trách nhiệm giải trình). Một **Scrum Team** chuẩn (thường $\le 10$ người) là một đơn vị gắn kết gồm **1 Scrum Master**, **1 Product Owner** và **Developers**.
* **Đặc điểm cốt lõi:** Không có đội nhóm con (no sub-teams) và không có phân cấp sếp-nhân viên (no hierarchies).
* **Cross-functional (Liên chức năng):** Các thành viên có đủ mọi kỹ năng cần thiết để tạo ra giá trị sau mỗi Sprint.
* **Self-managing (Tự quản lý):** Tự quyết định ai làm gì, khi nào và làm như thế nào trong nội bộ.

> **Ánh xạ vào đội 5 người tại Hack4Biz:**
> * **Product Owner (PO):** 1 thành viên đóng vai trò PO.
> * **Scrum Master (SM):** Trong mô hình cuộc thi có vị trí PM, **PM sẽ kiêm nhiệm vai trò Scrum Master** ở tầng vận hành Scrum (đồng thời quản lý tổng thể Rủi ro/Stakeholder/Timeline cuộc thi).
> * **Developers:** Trong ngôn ngữ Scrum Guide, **BA, DEV (Coding/AI Engineer), và QA đều được gọi chung là "Developers"** vì tất cả đều trực tiếp tham gia tạo ra bản Increment có thể sử dụng được.

| Tiêu chí | Product Owner (PO) | Scrum Master (SM) | Developers (gồm DEV, BA, QA trong Team) |
| :--- | :--- | :--- | :--- |
| **Sứ mệnh tối cao** | **Tối đa hóa giá trị (Maximize Value)** của sản phẩm tạo ra từ công sức của Scrum Team. | Thiết lập Scrum theo đúng Scrum Guide và **đảm bảo hiệu quả (Effectiveness)** của Scrum Team. | Tạo ra bất kỳ khía cạnh nào của một **Usable Increment** (Phần tăng trưởng dùng được) trong mỗi Sprint. |
| **Quyền hạn & Trách nhiệm độc quyền** | - Quản lý **Product Backlog**: Xây dựng, truyền đạt rõ **Product Goal**, tạo và sắp xếp thứ tự các Product Backlog Items (PBIs).<br>- Là **1 cá nhân duy nhất** (không phải một hội đồng).<br>- **Duy nhất PO** có quyền hủy một Sprint (Cancel a Sprint) khi Sprint Goal trở nên lỗi thời. | - Là **True Leader who serves** (Lãnh đạo phục vụ) cho Scrum Team, PO và Tổ chức.<br>- Huấn luyện (Coach) team về tính tự quản và liên chức năng.<br>- Loại bỏ các **Impediments** (Trở ngại) vượt quá khả năng tự xử lý của Developers.<br>- Đảm bảo các sự kiện Scrum diễn ra tích cực, hiệu quả và đúng **Timebox**. | - Tạo kế hoạch cho Sprint (**Sprint Backlog**).<br>- Độc quyền ước lượng kích thước công việc (**Estimation** / Story Points) và chọn lượng việc đưa vào Sprint.<br>- Đảm bảo chất lượng bằng cách tuân thủ nghiêm ngặt **Definition of Done (DoD)**.<br>- Thích ứng kế hoạch mỗi ngày hướng tới **Sprint Goal**. |
| **Ranh giới KHÔNG được xâm phạm (Boundary Traps)** | - PO có thể ủy quyền cho BA viết User Story, nhưng **PO vẫn chịu trách nhiệm giải trình cuối cùng (Accountable)**.<br>- PO **KHÔNG** được ép Developers nhận nhiều Story Points hơn năng lực của họ.<br>- PO **KHÔNG** can thiệp vào giải pháp kỹ thuật chi tiết ("How"). | - SM **KHÔNG** phải là thư ký (chỉ ghi biên bản/đặt phòng họp).<br>- SM **KHÔNG** phải là sếp giao việc (Task Assigner) trong Daily Scrum.<br>- SM **KHÔNG** đánh giá KPI cá nhân hay ép tiến độ kiểu vi mô (Micromanagement). | - Không ai (kể cả PO, SM hay Giám đốc) được phép bắt Developers làm giảm chất lượng (bỏ qua DoD) để chạy theo số lượng.<br>- BA/DEV/QA trong nhóm Developers không đổ lỗi kiểu *"BA viết xong là hết việc"*, *"DEV code xong quăng cho QA"* — toàn bộ Developers cùng chịu trách nhiệm chung về Increment. |

---

### 1.4. 5 Sự kiện trong Scrum (Scrum Events)

Mọi sự kiện trong Scrum đều là cơ hội chính thức để thực hiện **Inspection (Thanh tra)** và **Adaptation (Thích ứng)**. Tất cả đều được gắn **Timebox** (thời lượng tối đa không được vượt quá).

```text
+===================================================================================+
|                           SPRINT (Container Event: <= 1 Tháng)                    |
|                                                                                   |
|  +-----------------+     +--------------------+     +--------------+   +-------+  |
|  | SPRINT PLANNING | --> |    DAILY SCRUM     | --> |SPRINT REVIEW |-->| SPRINT|  |
|  | (Why, What, How)|     | (Mỗi 24h - 15 phút)|     |(Inspect Product) | RETRO |  |
|  +-----------------+     +--------------------+     +--------------+   +-------+  |
|           |                        |                       ^               |      |
|           v                        v                       |               |      |
|    [Sprint Backlog] ----> [Development Work] ----> [Usable Increment]      |      |
|                                                                            |      |
|  <------------------ Cải tiến quy trình cho Sprint tiếp theo --------------+      |
+===================================================================================+
```

| Sự kiện (Event) | Thời lượng chuẩn (Timebox) | Người tham gia bắt buộc | Đầu vào (Input) | Đầu ra (Output) | Mục tiêu cốt lõi (Core Purpose) | Các lỗi sai thường gặp (Anti-patterns / Exam Traps) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **1. Sprint** | Cố định **$\le$ 1 tháng** (Ở Hack4Biz Vòng 2: **1 tuần / Sprint**; Vòng 3: **Mini-Sprint 8–16h**). | Toàn bộ **Scrum Team** (PO, SM, Developers) + tương tác với Stakeholders. | Product Backlog đã được tinh chỉnh (Refined). | Ít nhất một **Usable Increment** đạt chuẩn DoD. | Là sự kiện bao trùm (Container) chứa 4 sự kiện còn lại; biến ý tưởng thành giá trị thực tế theo nhịp độ ổn định. | - Kéo dài thêm vài ngày vì "chưa code xong" (Phá vỡ Timebox!).<br>- Có khoảng nghỉ ("Buffer/Hardening days") giữa 2 Sprint (Sai: Sprint mới bắt đầu ngay lập tức sau khi Sprint cũ kết thúc).<br>- Thay đổi phạm vi làm nguy hại đến **Sprint Goal**. |
| **2. Sprint Planning** | Tối đa **8 giờ** cho Sprint 1 tháng (Ngắn hơn theo tỷ lệ với Sprint ngắn: ~**2 giờ** cho Sprint 1 tuần). | Toàn bộ **Scrum Team** (Có thể mời chuyên gia bên ngoài vào tư vấn kỹ thuật/nghiệp vụ nếu cần). | - Product Backlog (các mục trên cùng đã đạt DoR).<br>- Bản Increment mới nhất.<br>- Velocity quá khứ & Năng lực hiện tại (Capacity) của Developers.<br>- Definition of Done. | **Sprint Backlog** bao gồm:<br>1. **Sprint Goal** (Tại sao Sprint này giá trị?).<br>2. Các **PBIs** được chọn (Làm cái gì?).<br>3. Kế hoạch bàn giao / Tasks (Làm thế nào?). | Khởi động Sprint bằng việc thống nhất 3 chủ đề: **Topic 1 (Why?)**, **Topic 2 (What?)**, **Topic 3 (How?)**. | - PO ép Developers nhận hết danh sách tính năng vượt quá Velocity.<br>- Bỏ qua việc đặt **Sprint Goal** mà chỉ nhặt một đống các User Story rời rạc không liên quan nhau.<br>- Phân rã 100% task chi tiết đến từng phút cho cả tháng ngay trong buổi Planning (chỉ cần phân rã đủ cho những ngày đầu). |
| **3. Daily Scrum** | Đúng **15 phút** mỗi ngày làm việc (cố định giờ và địa điểm để giảm phức tạp). | **Developers** của Scrum Team.<br>*(Lưu ý: Nếu PO hoặc SM đang trực tiếp làm các task trong Sprint Backlog, họ tham gia với tư cách là Developers).* | Sprint Backlog hiện tại, tiến độ thực tế hướng tới Sprint Goal. | Kế hoạch hành động cụ thể cho **24 giờ tiếp theo**; Sprint Backlog được cập nhật/điều chỉnh nếu cần. | **Thanh tra tiến độ hướng tới Sprint Goal** và điều chỉnh Sprint Backlog cho ngày làm việc sắp tới. | - Biến thành buổi **họp báo cáo trạng thái (Status Report)** cho Scrum Master, PM hoặc PO.<br>- Bắt buộc trả lời máy móc 3 câu hỏi truyền thống mà không nhìn vào Sprint Goal (Scrum Guide 2020 đã bỏ bắt buộc 3 câu hỏi, miễn là tập trung vào Sprint Goal).<br>- Sa đà thảo luận kỹ thuật sâu kéo dài 45 phút (Đúng ra phải tách sang buổi thảo luận riêng ngay sau Daily Scrum - gọi là *After-party / Parking Lot*). |
| **4. Sprint Review** | Tối đa **4 giờ** cho Sprint 1 tháng (~**1 giờ** cho Sprint 1 tuần). | Toàn bộ **Scrum Team** + **Key Stakeholders** được PO mời. | Bản **Increment(s)** đã hoàn thành đạt chuẩn DoD, Product Backlog hiện tại, bối cảnh thị trường/nghiệp vụ mới. | **Product Backlog đã được cập nhật** (thêm mới, sửa đổi hoặc sắp xếp lại thứ tự ưu tiên để đón cơ hội mới). | **Thanh tra kết quả của Sprint (Outcome / Increment)** cùng Stakeholders và xác định các điều chỉnh trong tương lai. | - Trình diễn các tính năng **chưa đạt DoD** (code dở dang, chưa test) hoặc chỉ chiếu slide PowerPoint.<br>- Biến thành buổi "nghiệm thu đóng dấu" (Sign-off Gate) một chiều thay vì một buổi **Working Session** (phiên làm việc tương tác hai chiều).<br>- Không có mặt bất kỳ Stakeholder nào (chỉ có Scrum Team tự xem với nhau). |
| **5. Sprint Retrospective** | Tối đa **3 giờ** cho Sprint 1 tháng (~**45–60 phút** cho Sprint 1 tuần). | **Chỉ nội bộ Scrum Team** (PO, SM, Developers). Không mời Stakeholders bên ngoài để đảm bảo an toàn tâm lý. | Dữ liệu và trải nghiệm của Sprint vừa qua (con người, mối quan hệ, quy trình, công cụ, DoD). | Các **Actionable Improvements** (Cải tiến khả thi) được xác định để thực hiện ngay trong Sprint tiếp theo (và có thể cập nhật mở rộng DoD). | Lên kế hoạch cho các cách thức nhằm **tăng cường chất lượng và hiệu quả làm việc (Quality & Effectiveness)** của đội nhóm. | - Biến thành buổi **"Đấu tố / Đổ lỗi" (Blame Game)** giữa DEV, BA và QA.<br>- Chỉ than phiền rồi để đó, không chốt được **Action Items** cụ thể gắn cho người phụ trách ở Sprint kế tiếp.<br>- Bỏ qua Retrospective vì "đang bận code cho kịp deadline". |

---

### 1.5. 3 Tạo tác & Cam kết đi kèm (Scrum Artifacts & Commitments)

Scrum Guide 2020 bổ sung khái niệm **Commitments (Cam kết)** gắn liền với từng **Artifact (Tạo tác)** nhằm đảm bảo tính minh bạch và mang lại tiêu điểm để đo lường tiến độ:

```text
+-------------------------+          Cam kết (Commitment)          +-----------------------------+
|  1. PRODUCT BACKLOG     | =====================================> |  PRODUCT GOAL               |
|  (Danh sách việc của SP)|   Mục tiêu dài hạn của sản phẩm        |  (Đích đến chiến lược)      |
+-------------------------+                                        +-----------------------------+
             |
             | (Lựa chọn trong Sprint Planning)
             v
+-------------------------+          Cam kết (Commitment)          +-----------------------------+
|  2. SPRINT BACKLOG      | =====================================> |  SPRINT GOAL                |
|  (Kế hoạch của Sprint)  |   Mục tiêu duy nhất của Sprint         |  (Giá trị cốt lõi của kỳ)   |
+-------------------------+                                        +-----------------------------+
             |
             | (Thực thi bởi Developers)
             v
+-------------------------+          Cam kết (Commitment)          +-----------------------------+
|  3. INCREMENT           | =====================================> |  DEFINITION OF DONE (DoD)   |
|  (Phần sản phẩm hoàn tất)|   Thước đo chất lượng bắt buộc        |  (Tiêu chuẩn Hoàn thành)    |
+-------------------------+                                        +-----------------------------+
```

1. **Product Backlog $\rightarrow$ Cam kết: Product Goal**
   * **Product Backlog** là một danh sách nổi (emergent), được sắp xếp theo thứ tự ưu tiên (ordered) gồm những gì cần thiết để cải thiện sản phẩm. Đây là **nguồn công việc duy nhất (single source of work)** mà Scrum Team thực hiện.
   * **Product Goal** mô tả trạng thái tương lai của sản phẩm, đóng vai trò là mục tiêu để Scrum Team lập kế hoạch. Tại một thời điểm, Scrum Team phải hoàn thành (hoặc từ bỏ) một Product Goal trước khi bắt tay vào Product Goal tiếp theo.
   * *Ví dụ tại Hack4Biz:* **Product Goal:** *"Xây dựng MVP AI Agent Tư vấn Tài chính & Xử lý Khiếu nại Thẻ tự động cho khách hàng VPBank với độ chính xác $\ge 90\%$ và thời gian phản hồi $< 3$ giây"*.

2. **Sprint Backlog $\rightarrow$ Cam kết: Sprint Goal**
   * **Sprint Backlog** được tạo bởi và thuộc quyền sở hữu của **Developers**. Công thức bất biến:
     $$\text{Sprint Backlog} = \text{Sprint Goal (Why)} + \text{Selected PBIs (What)} + \text{Actionable Plan (How)}$$
   * **Sprint Goal** là mục tiêu duy nhất của Sprint. Nó mang lại sự linh hoạt (flexibility) cho Developers về mặt phạm vi công việc chi tiết: nếu công việc thực tế khác với dự kiến, Developers thương lượng với PO về phạm vi của Sprint Backlog trong phạm vi không làm ảnh hưởng đến Sprint Goal.

3. **Increment $\rightarrow$ Cam kết: Definition of Done (DoD)**
   * **Increment** là bước tiến cụ thể hướng tới Product Goal. Mỗi Increment được cộng dồn (additive) vào tất cả các Increment trước đó và được xác minh kỹ lưỡng để đảm bảo mọi phần hoạt động trơn tru cùng nhau.
   * Một Increment được sinh ra **ngay tại thời điểm một Product Backlog Item đáp ứng được Definition of Done** (không nhất thiết phải đợi đến cuối Sprint mới có Increment, và có thể tạo ra nhiều Increment trong một Sprint, thậm chí release ngay trong Sprint).
   * Nếu một PBI **không đạt DoD** vào cuối Sprint:
     1. **KHÔNG** được đưa vào Increment.
     2. **KHÔNG** được trình diễn (show) trong buổi Sprint Review.
     3. Quay trở lại Product Backlog để PO xem xét ưu tiên lại cho tương lai (và được ước lượng lại phần việc còn dang dở).

---

## PHẦN 2: CÔNG CỤ, CHỈ SỐ & KỸ THUẬT QUẢN LÝ TRONG AGILE SCRUM

### 2.1. Ước lượng & Lập kế hoạch (Estimation & Planning)

#### A. Story Points (SP) vs. Giờ tuyệt đối (Man-hours)
* **Story Point** là đơn vị đo lường **tương đối (relative estimation)** phản ánh tổng hợp **3 yếu tố** để hoàn thành toàn diện một Product Backlog Item (đạt chuẩn DoD):
  $$\text{Story Points} = f(\text{Volume/Effort}, \text{Complexity}, \text{Risk/Uncertainty})$$
  * **Volume / Effort (Khối lượng công việc):** Nhiều màn hình hay ít màn hình, viết nhiều test case hay ít.
  * **Complexity (Độ phức tạp):** Thuật toán AI RAG kết nối đa nguồn dữ liệu phức tạp hơn form CRUD thông thường.
  * **Risk / Uncertainty (Rủi ro & Sự bất định):** Tích hợp API bên thứ 3 chưa rõ tài liệu, hoặc mô hình LLM chưa kiểm chứng độ ổn định.
* **Tại sao Agile ưu tiên Story Points thay vì Giờ tuyệt đối (Hours) ở cấp độ Backlog?**
  1. **Loại bỏ sai lệch do trình độ cá nhân:** Cùng 1 tính năng, Senior Dev code mất 4 giờ, Junior Dev mất 12 giờ. Nếu ước lượng theo giờ, hai người sẽ tranh cãi không hồi kết. Nhưng cả hai đều đồng ý tính năng này phức tạp gấp đôi tính năng chuẩn (Reference Story 2 SP $\rightarrow$ tính năng này là **5 SP**).
  2. **Não bộ con người giỏi so sánh tương đối hơn ước tính tuyệt đối:** Nhìn hai tòa nhà, ta dễ dàng nói tòa A cao gấp đôi tòa B, hơn là đoán chính xác tòa A cao bao nhiêu mét.
  3. **Tránh áp lực tâm lý (Padding / Parkinson's Law):** Khi bị ép cam kết theo giờ, con người có xu hướng khai khống thời gian (buffer quá mức) hoặc cắt giảm chất lượng khi sắp hết giờ.

#### B. Dãy số Fibonacci & Kỹ thuật Planning Poker
* **Dãy Fibonacci sửa đổi trong Agile:** `1, 2, 3, 5, 8, 13, 20, 40, 100` (hoặc `?`, `∞`).
* **Tại sao dùng Fibonacci?** Khoảng cách giữa các số ngày càng lớn phản ánh **độ bất định tăng dần khi kích thước công việc lớn lên**. Với một User Story lớn, việc tranh luận xem nó là `11` hay `12` là vô nghĩa; khoảng cách `8 - 13 - 20` buộc team phải nhận ra: nếu một Story rơi vào `13` hoặc `20`, nó quá lớn và **cần được tách nhỏ (Split)** trước khi đưa vào Sprint.
* **Quy trình Planning Poker chuẩn:**
  1. **Chọn Reference Story (Story mốc):** Team chọn 1 User Story nhỏ, ai cũng hiểu rõ làm mốc (ví dụ: `2 SP`).
  2. **PO/BA trình bày User Story** và giải đáp các câu hỏi về Acceptance Criteria.
  3. **Ước lượng độc lập (Chống hiệu ứng mỏ neo - Anchoring Bias):** Mỗi thành viên trong nhóm **Developers (cả DEV, BA, QA)** tự chọn lá bài Fibonacci và **lật bài cùng một lúc**. *(Lưu ý: PO và SM KHÔNG được giơ bài ước lượng).*
  4. **Thảo luận hai cực:** Nếu số điểm khác nhau (ví dụ: DEV giơ `3`, QA giơ `8`), người chọn **thấp nhất** và người chọn **cao nhất** giải thích lý do (thường QA nhìn ra góc khuất kiểm thử tự động hoặc edge cases mà DEV chưa tính tới).
  5. **Lật bài vòng 2:** Đạt được sự đồng thuận (Consensus) của cả nhóm Developers (không phải lấy trung bình cộng cơ học!).

#### C. Cách tính Velocity (Vận tốc) & Capacity Planning
* **Velocity (Vận tốc):** Tổng số Story Points của các Product Backlog Items đã **hoàn thành 100% đạt chuẩn DoD** trong một Sprint.
  * **Quy tắc Vàng (Golden Rule of Velocity):** **KHÔNG BAO GIỜ tính điểm phần trăm cho Story dở dang.** Một User Story `8 SP` đã code xong 100%, test xong 90% nhưng còn 1 lỗi chưa đạt DoD khi kết thúc Sprint thì Sprint đó ghi nhận **`0 SP`** cho Story này (8 SP sẽ được tính vào Sprint tiếp theo khi nó thực sự hoàn tất, hoặc ước lượng lại phần còn lại).
  * **Mục đích của Velocity:** Dùng để dự báo năng lực lập kế hoạch cho các Sprint tiếp theo và dự phóng ngày phát hành (Release Forecasting) thông qua trung bình trượt 3–5 Sprint gần nhất.
  * **Cảnh báo:** Tuyệt đối **KHÔNG** dùng Velocity để so sánh hiệu suất giữa Team A và Team B (vì mỗi team có Story mốc `1 SP` khác nhau, so sánh sẽ dẫn đến lạm phát điểm - *Point Inflation*).

* **Capacity Planning (Hoạch định công suất) cho Sprint mới:**
  Khi lập kế hoạch Sprint, cần kết hợp **Historical Velocity** (Vận tốc lịch sử) và **Available Capacity** (Công suất khả dụng thực tế của nhân sự trong Sprint tới):
  $$\text{Adjusted Sprint Capacity (SP)} = \text{Average Velocity} \times \left(\frac{\text{Available Person-Days trong Sprint tới}}{\text{Standard Person-Days của Sprint chuẩn}}\right)$$
  * *Ví dụ tính toán:* Team 3 Developers (BA, DEV, QA) trong một Sprint 5 ngày có tổng công suất chuẩn là $3 \times 5 = 15\text{ Person-Days}$, đạt Velocity trung bình là **$30\text{ SP}$**. Sang Sprint 2, DEV bận thi môn học ở trường mất 1.5 ngày, QA nghỉ ốm 0.5 ngày $\rightarrow$ Công suất thực tế còn $15 - 2 = 13\text{ Person-Days}$. Khi đó, lượng Story Points khuyến nghị đưa vào Sprint 2 là:
    $$30 \times \frac{13}{15} = 26\text{ SP}$$
  * Ngoài ra, nếu làm Capacity Planning theo giờ (Task Breakdown ở Topic 3 của Sprint Planning), chỉ nên lập kế hoạch ở mức **6–6.5 giờ productive work / ngày / người** (dành 1.5–2 giờ cho các sự kiện Scrum, trao đổi, xử lý sự cố phát sinh).

---

### 2.2. Biểu đồ Theo dõi Tiến độ & Phát hiện Điểm nghẽn (Bottlenecks)

#### A. Sprint Burndown Chart (Biểu đồ đốt cháy công việc trong Sprint)
Theo dõi **lượng công việc còn lại (Remaining Effort: Story Points hoặc Hours)** theo từng ngày của Sprint.
* **Trục tung (Y):** Lượng công việc còn lại (SP / Hours).
* **Trục hoành (X):** Thời gian (Ngày 1 $\rightarrow$ Ngày N của Sprint).
* **Đường lý tưởng (Ideal Line):** Đường thẳng nối từ tổng SP ban đầu ở Ngày 1 xuống `0` ở ngày cuối Sprint.
* **Đường thực tế (Actual Line):** Lượng việc còn lại thực tế mỗi ngày.

```text
Story Points (SP)
  30 |* (Bắt đầu Sprint)
     |  \          *---------*---------*   <-- (1) Đi ngang nhiều ngày (Flatline / Plateau)
  20 |    \      /                       \
     |      \  *                           \        *  <-- (2) Nhảy vọt lên (Spike / Scope Creep)
  10 |        \                              \    /   \
     |          \  (Đường lý tưởng - Ideal)    *       \
   0 +-----------\---------------------------------------*---> Ngày trong Sprint
     D1   D2   D3   D4   D5   D6   D7   D8
```

* **Cách đọc & chẩn đoán bệnh qua Sprint Burndown Chart:**
  1. **Đường thực tế nằm cao hơn đường lý tưởng (Above Ideal Line):** Team đang chậm tiến độ (Behind Schedule). Có thể do ước lượng quá lạc quan (Under-estimation) hoặc gặp Impediment chưa được gỡ bỏ.
  2. **Đường thực tế đi ngang nhiều ngày liên tục (Flatline / Plateau) rồi rơi thẳng đứng vào ngày cuối (Cliff Drop):**
     * *Nguyên nhân 1:* User Stories quá to (chưa tách nhỏ theo INVEST), làm mãi đến ngày cuối mới Done cùng lúc.
     * *Nguyên nhân 2:* **Bottleneck ở khâu QA / Code Review** (Mini-Waterfall trong Sprint: DEV code từ ngày 1 đến ngày 6 rồi dồn toàn bộ cho QA test vào ngày 7).
     * *Nguyên nhân 3:* Team quên không cập nhật bảng Jira/Kanban hàng ngày trước giờ Daily Scrum.
  3. **Đường thực tế nhảy vọt lên cao giữa chừng (Upward Spike):** Phạm vi công việc trong Sprint bị phình ra (**Scope Creep**) do thêm Story mới giữa Sprint hoặc phát hiện thêm nhiều task ẩn chưa lường trước.
  4. **Đường thực tế chạm mốc 0 quá sớm (Early Drop):** Team ước lượng quá dư dả (Over-estimation / Sandbagging). Hành động đúng: Developers phối hợp với PO kéo thêm PBI tiếp theo từ đỉnh Product Backlog vào Sprint.

#### B. Release Burnup Chart (Biểu đồ đốt lên cấp độ Phát hành)
Khác với Burndown (chỉ có 1 đường đi xuống nên khi đường đó đi ngang ta không phân biệt được là do *"Team không làm được việc"* hay do *"Team làm được rất nhiều nhưng PO cũng vừa nhét thêm từng ấy việc mới vào"*), **Burnup Chart tách bạch thành 2 đường độc lập**:
1. **Total Scope Line (Đường tổng phạm vi - phía trên):** Thể hiện tổng số Story Points của bản Release/MVP.
2. **Completed Work Line (Đường công việc đã hoàn thành - đi từ 0 lên):** Thể hiện tổng số SP tích lũy đã đạt DoD qua các Sprint.

```text
Story Points (SP)
 120 |                                      *-------*  <-- Total Scope Line (Tăng do thêm CR)
 100 |--------------*-------*-------*------/        .
  80 |                                    /       . (Dự phóng ngày hoàn thành)
  60 |                            *------*      .
  40 |                    *------/            .
  20 |            *------/  <-- Completed Work Line (Velocity tích lũy)
   0 +----*------/-----------------------------------------> Sprints
     S0   S1      S2      S3      S4      S5      S6
```
* **Ưu điểm vượt trội:** Giúp PM và PO minh bạch hóa với Stakeholders tác động của **Scope Creep**. Nếu đường *Completed Work* vẫn dốc lên đều đặn (Velocity của team rất tốt) nhưng hai đường mãi không cắt nhau vì đường *Total Scope* liên tục bị đẩy lên cao, PM có bằng chứng dữ liệu để yêu cầu đóng băng phạm vi hoặc cắt giảm tính năng phụ (De-scope).

#### C. Cumulative Flow Diagram - CFD (Biểu đồ Luồng Tích lũy)
CFD là công cụ mạnh nhất để phân tích độ ổn định của quy trình và phát hiện **Điểm nghẽn (Bottleneck)** thông qua các dải màu chồng lên nhau theo thời gian (từ trên xuống dưới: *To Do $\rightarrow$ In Analysis (BA) $\rightarrow$ In Development (DEV) $\rightarrow$ In Testing (QA) $\rightarrow$ Done*).

```text
Số lượng Items (PBIs)
  ^
  |          /------------- [ To Do ]
  |        /          /---- [ In Progress / DEV ]
  |      /          /
  |    /          /         <-- Khoảng cách dọc (WIP) phình to ở dải [In Testing / QA]!
  |  /          /               (Chứng tỏ tốc độ DEV đẩy sang nhanh hơn tốc độ QA xử lý)
  |           /            /--- [ In Testing / QA ] (BOTTLENECK!)
  |         /            /
  |       /            /    /-- [ Done ]
  +------------------------------> Thời gian (Ngày)
```

* **3 thông số đọc trực tiếp từ CFD (Theo Định luật Little - Little's Law: $\text{Cycle Time} = \frac{\text{WIP}}{\text{Throughput}}$):**
  1. **Khoảng cách theo chiều dọc (Vertical Distance) của một dải màu:** Chính là **WIP (Work In Progress)** — số lượng hạng mục đang nằm ở trạng thái đó tại một thời điểm.
  2. **Khoảng cách theo chiều ngang (Horizontal Distance) của một dải màu:** Chính là **Cycle Time / Lead Time** trung bình để một hạng mục đi qua trạng thái đó.
  3. **Độ dốc của đường ranh giới (Slope):** Chính là **Throughput** (Tốc độ đầu vào / đầu ra).
* **Cách bắt bệnh Bottleneck trên CFD:** Nếu một dải màu (ví dụ: *In Testing / QA*) **ngày càng phình to ra theo chiều dọc** (đường biên trên dốc lên nhanh nhưng đường biên dưới là *Done* lại lài lài đi ngang), nghĩa là công việc đang ứ đọng nghiêm trọng tại khâu QA.
* **Giải pháp của Scrum Master / PM:** Áp dụng **WIP Limit** (giới hạn số lượng ticket ở cột DEV/QA) và kích hoạt **Swarming** (DEV tạm dừng kéo ticket mới, nhảy vào viết Unit Test/Automation Test hoặc hỗ trợ chuẩn bị dữ liệu test để giải phóng nút thắt ở cột QA).

---

### 2.3. Tiêu chuẩn Chất lượng & Quản lý Backlog

#### A. Phân biệt Definition of Ready (DoR) vs. Definition of Done (DoD)

| Tiêu chí | Definition of Ready (DoR) | Definition of Done (DoD) |
| :--- | :--- | :--- |
| **Bản chất theo Scrum Guide** | **Thực hành bổ trợ tốt (Good Complementary Practice)** do team tự quy ước, **KHÔNG** phải là cam kết bắt buộc chính thức trong Scrum Guide. | **Cam kết bắt buộc chính thức (Formal Commitment)** gắn liền với **Increment** trong Scrum Guide 2020. |
| **Vị trí áp dụng** | **Cổng đầu vào (Input Gate)** trước buổi *Sprint Planning*. | **Cổng đầu ra (Output Gate)** trước khi công nhận một PBI trở thành *Increment* và đưa ra *Sprint Review*. |
| **Câu hỏi trả lời** | *"User Story này đã đủ rõ ràng, đủ nhỏ và khả thi để Developers tự tin kéo vào Sprint chưa?"* | *"Hạng mục này đã hoàn tất 100% với chất lượng sẵn sàng phát hành cho người dùng cuối chưa?"* |
| **Lưu ý tránh Anti-pattern** | Không biến DoR thành một "Hàng rào quan liêu (Stage-Gate)" cứng nhắc khiến team không dám đưa một Story vào Sprint chỉ vì thiếu 1 chi tiết nhỏ có thể trao đổi trong Sprint. | **Không bao giờ** được hạ thấp tiêu chuẩn DoD vào cuối Sprint chỉ để "làm đẹp báo cáo Velocity". Nếu tổ chức có sẵn chuẩn DoD, Scrum Team phải tuân thủ tối thiểu chuẩn đó; nếu chưa có, Scrum Team tự thiết lập. |
| **Checklist mẫu cho dự án AI Agent (Hack4Biz)** | 1. Đã viết đúng chuẩn User Story & thỏa tiêu chí INVEST.<br>2. Đã có đầy đủ Acceptance Criteria (Given-When-Then) cho cả luồng chính và luồng AI fallback.<br>3. Đã có tập dữ liệu mẫu (Sample Dataset / Prompt test cases) và xác nhận API Key khả dụng.<br>4. Đã được nhóm Developers ước lượng Story Points ($\le 8\text{ SP}$).<br>5. Đã có mockup UI cơ bản trên Figma (nếu là tính năng giao diện). | 1. Code hoàn tất, tuân thủ Coding Convention & đã qua Peer Code Review.<br>2. Đã cấu hình Guardrails chống Prompt Injection & che dữ liệu nhạy cảm (PII Masking).<br>3. Unit Test & API Integration Test đạt 100% pass.<br>4. QA đã chạy kiểm thử toàn bộ Acceptance Criteria + bộ câu hỏi đánh giá AI (Evaluation Dataset đạt ngưỡng Accuracy $\ge 85\%$, Latency $< 3\text{s}$).<br>5. Không còn Bug mức Critical/High tồn đọng.<br>6. Đã deploy lên môi trường Staging và cập nhật tài liệu API/HDSD. |

#### B. Kỹ thuật chia nhỏ User Story (INVEST) & Viết Acceptance Criteria (Given-When-Then)

1. **Cấu trúc chuẩn của User Story (Connextra Template):**
   > **As a** `<Vai trò người dùng cụ thể>`,  
   > **I want to** `<Hành động / Tính năng mong muốn>`,  
   > **So that** `<Giá trị / Lợi ích kinh doanh mang lại>`.
   * *Ví dụ dự án VPBank AI Agent:*
     > **As a** *Chủ thẻ tín dụng VPBank bị nuốt thẻ hoặc phát hiện giao dịch bất thường lúc nửa đêm*,  
     > **I want to** *yêu cầu AI Agent khóa thẻ tạm thời ngay trên khung chat sau khi xác thực OTP*,  
     > **So that** *tôi bảo vệ được tiền trong tài khoản ngay lập tức mà không phải chờ tổng đài viên trực điện thoại*.

2. **6 Tiêu chí đánh giá User Story chất lượng (Mô hình INVEST):**
   * **I — Independent (Độc lập):** Các User Story nên độc lập với nhau nhất có thể để PO dễ dàng thay đổi thứ tự ưu tiên mà không bị dây chuyền.
   * **N — Negotiable (Có thể thương lượng):** User Story không phải là bản hợp đồng đóng băng; chi tiết thực hiện sẽ được PO và Developers trao đổi, tinh chỉnh.
   * **V — Valuable (Có giá trị):** Phải mang lại giá trị cụ thể cho người dùng cuối hoặc khách hàng (VPBank). **Tránh chia Story theo tầng kỹ thuật (Horizontal Slicing)** kiểu *"Story 1: Thiết kế Database"*, *"Story 2: Viết Backend API"*, *"Story 3: Làm giao diện Frontend"* (vì hoàn thành Story 1 khách hàng không dùng được gì cả). Phải chia theo **Vertical Slicing (Lát cắt dọc)** xuyên qua cả UI + Backend + AI + DB cho từng kịch bản nghiệp vụ nhỏ.
   * **E — Estimable (Ước lượng được):** Đủ thông tin để Developers ước lượng được kích thước (nếu quá mơ hồ về mặt công nghệ AI, cần tạo một **Spike** — một hoạt động nghiên cứu/thử nghiệm có giới hạn thời gian cố định để lấy thông tin trước khi ước lượng Story chính).
   * **S — Small (Đủ nhỏ):** Đủ nhỏ để hoàn thành trọn vẹn (đạt DoD) trong vòng vài ngày của một Sprint (thường không quá `1/3` đến `1/2` độ dài Sprint).
   * **T — Testable (Kiểm thử được):** Có tiêu chí rõ ràng để QA và PO xác nhận là Đạt (Pass) hay Không đạt (Fail).

3. **Viết Acceptance Criteria (AC) theo chuẩn BDD (Given - When - Then):**
   Giúp xóa bỏ sự mơ hồ giữa BA, DEV và QA, đặc biệt trong các kịch bản AI Agent:
   * **Kịch bản 1 (Happy Path - Truy vấn chính sách thẻ bằng RAG):**
     * **Given (Giả sử):** Khách hàng đã đăng nhập ứng dụng VPBank NEO và hỏi về *"Phí thường niên thẻ VPBank StepUp"*, đồng thời thông tin này có trong Vector Database chính thức của ngân hàng.
     * **When (Khi):** Khách hàng gửi câu hỏi vào khung chat AI Agent.
     * **Then (Thì):** AI Agent trả về đúng biểu phí hiện hành trong thời gian $\le 3$ giây, kèm theo trích dẫn nguồn (Citation link) tới biểu phí chính thức của VPBank và **tuyệt đối không** suy diễn con số ngoài tài liệu.
   * **Kịch bản 2 (Edge Case / Guardrail chống AI Hallucination):**
     * **Given:** Khách hàng hỏi một thông tin nằm ngoài phạm vi tri thức ngân hàng hoặc yêu cầu AI tư vấn đầu tư cổ phiếu rủi ro cao.
     * **When:** Hệ thống RAG truy xuất có điểm tương đồng (Similarity Score) $< 0.75$ hoặc bộ lọc Guardrail phát hiện chủ đề bị cấm.
     * **Then:** AI Agent lịch sự từ chối trả lời theo mẫu chuẩn (*"Xin lỗi, tôi chưa có thông tin chính thức đã được xác thực từ VPBank về vấn đề này..."*) và hiển thị nút **"Kết nối Chuyên viên Tư vấn (Human Handover)"**.

#### C. Các phương pháp Ưu tiên hóa Product Backlog (Prioritization Techniques)

PO (với sự hỗ trợ phân tích từ BA và PM) sử dụng 3 phương pháp phổ biến sau để sắp xếp Product Backlog:

| Phương pháp | Cơ chế phân loại / Công thức | Cách áp dụng thực tế cho MVP AI Agent tại Hack4Biz |
| :--- | :--- | :--- |
| **1. MoSCoW** | Phân chia các hạng mục thành 4 nhóm:<br>- **M - Must have:** Bắt buộc phải có để MVP hoạt động được và hợp lệ.<br>- **S - Should have:** Quan trọng, mang lại giá trị cao nhưng nếu thiếu thì hệ thống vẫn chạy được qua giải pháp tạm.<br>- **C - Could have:** Tính năng "Nice-to-have" tăng trải nghiệm nếu còn dư thời gian.<br>- **W - Won't have (this time):** Chắc chắn loại bỏ khỏi phạm vi kỳ này để chống Scope Creep. | - **Must:** Luồng Chat RAG tra cứu sản phẩm ngân hàng chính xác + Guardrail chống bịa đặt & bảo mật PII.<br>- **Should:** Tự động điền form đăng ký mở thẻ / khiếu nại qua hội thoại (Agentic Tool Calling).<br>- **Could:** Nhận diện giọng nói (Voice-to-Text) và biểu đồ phân tích cảm xúc khách hàng.<br>- **Won't:** Tích hợp thanh toán quốc tế SWIFT trực tiếp trong bản MVP 16 ngày. |
| **2. RICE Scoring** | Định lượng điểm ưu tiên khách quan:<br>$$\text{RICE Score} = \frac{\text{Reach} \times \text{Impact} \times \text{Confidence}}{\text{Effort}}$$<br>- **Reach:** Số lượng khách hàng/giao dịch chạm tới trong 1 đơn vị thời gian.<br>- **Impact:** Mức độ tác động ($3$: Massive, $2$: High, $1$: Medium, $0.5$: Low, $0.25$: Minimal).<br>- **Confidence:** Độ tự tin về số liệu và tính khả thi ($100\%, 80\%, 50\%$).<br>- **Effort:** Công sức thực hiện (Person-Days / Story Points). | Rất hữu ích khi PO và Stakeholders tranh cãi giữa 2 tính năng AI hấp dẫn. Một tính năng có **Impact** rất cao ($3$), nhưng độ tự tin kỹ thuật **Confidence** thấp ($50\%$) và tốn **Effort** lớn ($10\text{ ngày}$) sẽ có điểm RICE thấp hơn tính năng cốt lõi dễ triển khai. |
| **3. Value vs. Effort Matrix (2x2)** | Ma trận 4 góc phần tư dựa trên trục **Business Value (Giá trị kinh doanh)** và **Implementation Effort (Nỗ lực triển khai)**:<br>1. **High Value – Low Effort (Quick Wins):** Làm ngay ở Sprint 1!<br>2. **High Value – High Effort (Major Projects / Big Bets):** Chia nhỏ và đưa vào lộ trình cốt lõi.<br>3. **Low Value – Low Effort (Fill-ins):** Làm khi rảnh hoặc cuối kỳ nếu dư Capacity.<br>4. **Low Value – High Effort (Time Sinks / Money Pits):** Loại bỏ ngay lập tức! | Trong cuộc thi 16 ngày (Vòng 2) và 32 giờ (Vòng 3), tiêu chí sống còn của PM & PO là săn tìm các **Quick Wins** (tính năng gây ấn tượng mạnh với Ban Giám khảo VPBank nhưng tận dụng được sẵn Function Calling / Prompt Engineering thay vì phải huấn luyện lại mô hình từ đầu). |

#### D. Quy trình Backlog Refinement (Trước đây gọi là Backlog Grooming)
* **Bản chất:** Là hành động chia nhỏ và định nghĩa chi tiết các Product Backlog Items thành các mục nhỏ hơn, chính xác hơn. Đây là một **hoạt động diễn ra liên tục (ongoing activity)** xuyên suốt Sprint, **KHÔNG phải là một Sự kiện chính thức (official Scrum Event)** trong số 5 sự kiện của Scrum.
* **Thời lượng:** Thường chiếm không quá **10% tổng thời gian/năng lực** của Scrum Team trong một Sprint.
* **Quy trình 4 bước thực hiện Refinement hiệu quả giữa PO, BA, DEV, QA:**
  1. **PO & BA trình bày các PBIs ưu tiên cho 1–2 Sprint tới:** Giải thích bài toán nghiệp vụ ngân hàng và mục tiêu người dùng.
  2. **Thảo luận & Làm rõ (Clarification & Edge Cases):** DEV hỏi về giới hạn API/cấu trúc dữ liệu, QA đặt câu hỏi phản biện về các trường hợp ngoại lệ (What-if scenarios) để cùng BA hoàn thiện **Acceptance Criteria**.
  3. **Chia nhỏ (Splitting):** Tách các Epic/Story lớn thành các User Story nhỏ thỏa mãn tiêu chí **INVEST**.
  4. **Ước lượng (Sizing):** Nhóm Developers dùng **Planning Poker** gán Story Points để đưa các PBIs đạt chuẩn **Definition of Ready (DoR)** trước khi bước vào buổi Sprint Planning của kỳ kế tiếp.

---

## PHẦN 3: VAI TRÒ & NGHIỆP VỤ CHUYÊN SÂU CỦA PROJECT MANAGER (PM) TRONG MÔI TRƯỜNG AGILE HYBRID

### 3.1. Giải mã "Bẫy Đề Thi": Sự khác biệt giữa PM Truyền thống vs. Scrum Master / PO & Mô hình Agile Hybrid

Trong lý thuyết **Thuần Scrum (Pure Scrum)** theo Scrum Guide:
* **KHÔNG tồn tại chức danh "Project Manager (PM)"**.
* Toàn bộ trách nhiệm của một PM truyền thống được **phân tách và tái phân bổ** cho 3 vai trò trong Scrum Team:
  * Quản lý Phạm vi, Giá trị kinh doanh, Lộ trình sản phẩm, Ngân sách tính năng $\rightarrow$ Thuộc về **Product Owner (PO)**.
  * Quản lý Quy trình, Hiệu suất làm việc nhóm, Gỡ bỏ rào cản (Impediments), Huấn luyện Agile $\rightarrow$ Thuộc về **Scrum Master (SM)**.
  * Quản lý Công việc chi tiết hàng ngày, Phân công tác vụ kỹ thuật, Ước lượng thời gian, Cam kết chất lượng kỹ thuật $\rightarrow$ Thuộc về **Developers** (tự quản lý - Self-managing).

Tuy nhiên, trong thực tế doanh nghiệp lớn (như các dự án chuyển đổi số Ngân hàng tại VPBank) hoặc trong cấu trúc đội thi **Hack4Biz (5 vị trí: PM, PO, BA, DEV, QA)**, mô hình **Agile Hybrid (Lai ghép)** được áp dụng:
* **Khi đề thi hỏi theo chuẩn Scrum Guide:** Tuyệt đối **KHÔNG** chọn đáp án có từ *"Project Manager giao việc / quyết định phạm vi / phê duyệt ước lượng"*. Phải quy về đúng 3 vai trò **PO, Scrum Master, Developers**.
* **Khi đề thi hoặc thực tế vận hành ở mô hình Dự án / Agile Hybrid (có vị trí PM):**
  * **PM (kiêm Scrum Master ở cấp độ Team)** đóng vai trò là **Servant Leader (Lãnh đạo phục vụ)** đồng thời quản trị **Bức tranh tổng thể của Dự án (Macro-level Governance)**: Quản lý Lộ trình tổng thể & Milestones cuộc thi, Quản trị Rủi ro dự án (Risk Register), Quản lý Phụ thuộc liên nhóm/bên thứ 3 (Dependencies), Quản trị Truyền thông với Ban Giám khảo/Stakeholders và Điều phối ngân sách/tài nguyên (API quota, hạ tầng Cloud).
  * **Cấm kỵ của PM trong Agile Hybrid:** PM **không** được cướp quyền sắp xếp thứ tự Product Backlog của PO, và **không** được áp đặt ước lượng hay chia task hộ Developers.

#### Bảng Phân định Trách nhiệm RACI Matrix (Cho Đội 5 người: PM/SM, PO, BA, DEV, QA)

*Chú giải RACI:*
* **R (Responsible):** Người trực tiếp bắt tay vào thực hiện công việc.
* **A (Accountable):** Người chịu trách nhiệm giải trình cuối cùng và có quyền phê duyệt (Quy tắc vàng: **Mỗi hàng công việc chỉ có DUY NHẤT một chữ A**).
* **C (Consulted):** Người được tham vấn ý kiến hai chiều trước khi ra quyết định.
* **I (Informed):** Người được thông báo kết quả một chiều sau khi đã có quyết định/hoàn thành.

| Giai đoạn / Hoạt động cốt lõi | PM (kiêm SM) | PO | BA (Developer) | DEV (Developer) | QA (Developer) | Ghi chú ranh giới & Bẫy đề thi |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| **1. Xác định Product Vision & Product Goal** | C | **A / R** | C | I | I | PO chịu trách nhiệm tối cao về định hướng giá trị sản phẩm. |
| **2. Lập Project Charter, Master Schedule (Milestones) & Quản lý Risk Register tổng thể** | **A / R** | C | C | C | C | Nghiệp vụ quản trị dự án vĩ mô của PM để đảm bảo khớp các mốc nộp bài Vòng 2, Vòng 3. |
| **3. Sắp xếp thứ tự ưu tiên (Ordering) cho Product Backlog** | C | **A / R** | C | C | C | DEV/BA/QA có thể tư vấn về phụ thuộc kỹ thuật, nhưng **PO là người duy nhất giữ chữ A**. |
| **4. Phân tích nghiệp vụ chi tiết, vẽ luồng quy trình (BPMN/Sequence) & viết đặc tả User Story + AC** | I | **A** | **R** | C | C | PO có thể ủy quyền cho BA viết Story/AC (**R**), nhưng PO vẫn chịu trách nhiệm giải trình (**A**). |
| **5. Ước lượng kích thước công việc (Story Points / Sizing)** | I (Facilitate) | C (Làm rõ) | **R** | **A / R** | **R** | Nhóm **Developers (BA, DEV, QA)** trực tiếp làm đều có quyền ước lượng. PM/SM chỉ điều phối quy trình Planning Poker, không bỏ phiếu. |
| **6. Quyết định lượng PBIs kéo vào Sprint & Lập kế hoạch kỹ thuật (Sprint Backlog)** | C | C | **R** | **A / R** | **R** | Không ai được ép Developers kéo thêm việc vượt quá khả năng họ tự xác định. |
| **7. Thiết kế kiến trúc AI (RAG, Prompt, Guardrails) & Viết code / Unit Test** | I | I | C | **A / R** | C | DEV chịu trách nhiệm chính; BA hỗ trợ làm rõ logic, QA góp ý các tình huống biên từ sớm (Shift-left testing). |
| **8. Thiết kế Test Plan, Test Cases, Evaluation Dataset cho AI & Thực thi kiểm thử** | I | C | C | R (Fix bug) | **A / R** | QA chủ trì thiết kế kịch bản test và bộ câu hỏi đánh giá độ chính xác của AI Agent. |
| **9. Đảm bảo tuân thủ quy trình Scrum, huấn luyện Agile & Gỡ bỏ Impediments ngoại cảnh** | **A / R** | C | I | I | I | Đây là trách nhiệm cốt lõi của Scrum Master (do PM đảm nhiệm). |
| **10. Chấp nhận / Từ chối (Accept/Reject) hạng mục theo tiêu chí nghiệp vụ & Quyết định Release** | I | **A / R** | C | I | C | QA xác nhận đạt DoD kỹ thuật, còn PO quyết định thời điểm phát hành (Release) ra thị trường. |

---

### 3.2. Các mảng Nghiệp vụ Cốt lõi của Project Manager (PM)

#### A. Scope & Change Management (Quản lý Phạm vi & Thay đổi)
1. **Kiểm soát Scope Creep (Phình phạm vi) và Gold Plating (Mạ vàng tính năng):**
   * **Scope Creep:** Yêu cầu mới từ bên ngoài (Stakeholders/Khách hàng) len lỏi vào dự án một cách không kiểm soát mà không điều chỉnh thời gian/nguồn lực hoặc cắt bớt việc cũ.
   * **Gold Plating:** Bản thân thành viên trong team (thường là DEV hoặc BA) tự ý thêm các tính năng "ngầu", hiệu ứng phức tạp hoặc tối ưu hóa quá đà mà PO không yêu cầu, gây trễ tiến độ các tính năng Must-have.
   * **Nguyên tắc chặn đứng của PM:** Mọi công việc Developers làm trong Sprint **bắt buộc phải gắn với một PBI trong Sprint Backlog** phục vụ trực tiếp cho **Sprint Goal**. Bất kỳ ý tưởng hay nào phát sinh phải được ghi nhận vào Product Backlog để PO đánh giá ưu tiên, tuyệt đối không làm chui.

2. **Quy trình xử lý Change Request (CR) chuẩn Agile mà không làm vỡ Sprint hiện tại:**

```text
                [Stakeholder / Ban Tổ chức đưa Change Request (CR)]
                                        |
                                        v
        +---------------------------------------------------------------+
        | Bước 1: CHẶN TRỰC TIẾP VÀO DEV (Gatekeeping)                  |
        | PM/SM bảo vệ Developers; chuyển toàn bộ CR qua một cửa là PO. |
        +---------------------------------------------------------------+
                                        |
                                        v
        +---------------------------------------------------------------+
        | Bước 2: PHÂN TÍCH TÁC ĐỘNG (Impact Analysis)                  |
        | PO + BA + DEV đại diện đánh giá nhanh: Giá trị kinh doanh (V) |
        | vs. Chi phí kỹ thuật, Rủi ro & Story Points (E).              |
        +---------------------------------------------------------------+
                                        |
                         +--------------+--------------+
                         |                             |
          (CR không khẩn cấp / Có thể đợi)   (CR khẩn cấp / Bắt buộc ngay trong Sprint)
                         |                             |
                         v                             v
        +-------------------------------+   +---------------------------------------+
        | Đưa vào PRODUCT BACKLOG,      |   | Kiểm tra: CR có làm SPRINT GOAL hiện  |
        | sắp xếp lại thứ tự ưu tiên    |   | tại trở nên vô nghĩa (obsolete) không?|
        | để làm ở Sprint tiếp theo.    |   +---------------------------------------+
        +-------------------------------+              |                       |
                                              (Không làm hỏng Goal)    (Làm hỏng hoàn toàn Goal)
                                                       |                       |
                                                       v                       v
                                            +---------------------+  +-----------------------+
                                            | TRADE-OFF (Hoán đổi)|  | PO HỦY SPRINT (Cancel)|
                                            | PO thương lượng với |  | & Họp Sprint Planning |
                                            | Developers: Đưa CR  |  | mới ngay lập tức      |
                                            | (X SP) vào thì phải |  | (Trường hợp cực hiếm).|
                                            | rút PBI chưa làm có |  +-----------------------+
                                            | kích thước tương    |
                                            | đương (X SP) ra!    |
                                            +---------------------+
```

#### B. Schedule & Dependency Management (Quản lý Tiến độ & Phụ thuộc)
1. **Lập lộ trình Milestone & Xác định Critical Path (Đường găng):**
   * Dù chạy Agile theo từng Sprint, dự án vẫn có các mốc **Hard Deadlines / Milestones** cố định (như ngày nộp MVP Vòng 2, giờ đóng cổng nộp code Vòng 3).
   * **Critical Path (Đường găng):** Là chuỗi các tác vụ phụ thuộc lẫn nhau dài nhất quyết định thời gian ngắn nhất có thể để hoàn thành dự án. Bất kỳ sự chậm trễ nào trên các tác vụ thuộc Đường găng (Float / Slack = 0) sẽ **lập tức làm trễ toàn bộ hạn chót của dự án**.
   * *Đường găng điển hình trong dự án AI Agent:*
     `Chốt kịch bản nghiệp vụ lõi & Dữ liệu mẫu (BA/PO)` $\rightarrow$ `Xây dựng Vector DB & Luồng RAG/Agent Core (DEV)` $\rightarrow$ `Tích hợp API Backend với UI Chat (DEV)` $\rightarrow$ `Kiểm thử End-to-End & Chỉnh sửa Hallucination (QA + DEV)` $\rightarrow$ `Đóng gói Staging & Quay Video Demo / Pitching Deck`.
     *(Trong khi đó, việc "Làm đẹp màu sắc CSS trang giới thiệu" có độ trôi Float cao, không nằm trên đường găng).*

2. **Giải quyết Phụ thuộc chéo (Cross-dependencies) giữa BA – DEV – QA để chống "Mini-Waterfall":**
   * **Căn bệnh phổ biến nhất:** Tuần đầu BA viết tài liệu, DEV ngồi chơi; giữa Sprint DEV cắm đầu code, QA ngồi chơi; ngày cuối Sprint DEV quăng cục code sang cho QA test không kịp $\rightarrow$ Vỡ Sprint!
   * **4 Kỹ thuật hóa giải của PM/SM:**
     1. **Phiên làm việc "Three Amigos" (Bộ ba BA – DEV – QA):** Trước khi bắt đầu code một tính năng, BA, DEV và QA ngồi lại 15–20 phút để thống nhất luồng dữ liệu, API contract và kịch bản test ngay từ đầu.
     2. **Thiết kế Contract-First & Mock Data:** Ngay ngày đầu tiên khi BA và DEV chốt xong cấu trúc JSON của API (API Contract / Swagger), Frontend có thể làm việc trên Mock API, và QA có thể viết sẵn kịch bản test Postman / bộ câu hỏi đánh giá AI (Evaluation Dataset) song song với lúc DEV đang code logic bên dưới.
     3. **Vertical Slicing & Micro-handovers:** Chia User Story đủ nhỏ (1–2 ngày xong 1 Story). Ngay khi Story 1 code xong ở Ngày 2 là chuyển sang QA test luôn, không đợi code xong cả 5 Stories mới đưa QA.
     4. **Shift-Left Testing:** QA tham gia kiểm thử ngay từ khâu đọc tài liệu của BA (kiểm tra tính logic của quy trình nghiệp vụ và Prompt System) trước cả khi dòng code đầu tiên được viết ra.

#### C. Risk Management (Quản trị Rủi ro Dự án)
* **Phân biệt Risk (Rủi ro) vs. Issue / Impediment (Vấn đề / Trở ngại):**
  * **Risk:** Sự kiện bất định **chưa xảy ra** (nằm ở tương lai), nếu xảy ra sẽ gây tác động tiêu cực (hoặc tích cực) đến mục tiêu dự án. *Ví dụ: "Có nguy cơ API OpenAI/Gemini bị giới hạn Rate Limit khi Ban Giám khảo chấm thi đồng loạt".*
  * **Issue / Impediment:** Sự kiện **đã hoặc đang xảy ra** ở hiện tại, đang cản trở tiến độ của team. *Ví dụ: "Tài khoản Cloud của team vừa bị khóa do hết hạn mức thẻ tín dụng".*
* **Đánh giá định lượng theo Ma trận Xác suất $\times$ Tác động (Probability $\times$ Impact Matrix):**
  $$\text{Risk Score (Severity)} = \text{Probability (1..5)} \times \text{Impact (1..5)}$$
  * **High Risk (Điểm $15 - 25$):** Bắt buộc phải có phương án chủ động xử lý ngay và theo dõi hàng ngày trong Daily Scrum.
  * **Medium Risk (Điểm $6 - 14$):** Lập kế hoạch dự phòng (Contingency Plan) và gắn chỉ báo cảnh báo sớm (Risk Trigger).
  * **Low Risk (Điểm $1 - 5$):** Đưa vào Watchlist (Danh sách theo dõi) hoặc chấp nhận.
* **4 Chiến lược ứng phó với Rủi ro tiêu cực (4 T's of Risk Response):**
  1. **Avoid (Né tránh / Terminate):** Thay đổi kế hoạch hoặc kiến trúc kỹ thuật để triệt tiêu hoàn toàn khả năng xảy ra rủi ro (Xác suất = 0). *Ví dụ: Để tránh rủi ro AI tự ý thực hiện giao dịch chuyển tiền sai gây thiệt hại tài chính, thiết kế hệ thống bắt buộc bước xác nhận cuối cùng (Human-in-the-loop Confirmation) bằng nút bấm cứng kết hợp OTP thay vì để LLM tự gọi hàm chuyển tiền.*
  2. **Mitigate (Giảm thiểu / Treat):** Hành động chủ động từ trước để giảm **Xác suất** xảy ra hoặc giảm **Mức độ thiệt hại** nếu nó xảy ra. *Ví dụ: Thiết lập cơ chế Semantic Caching và Fallback sang model dự phòng (như từ Gemini Pro sang Gemini Flash) để giảm rủi ro quá tải hoặc đứt kết nối API LLM.*
  3. **Transfer (Chuyển giao / Transfer):** Chuyển gánh nặng thiệt hại hoặc trách nhiệm xử lý rủi ro sang bên thứ ba (bảo hiểm, sử dụng dịch vụ Managed Cloud có cam kết SLA thay vì tự dựng server vật lý).
  4. **Accept (Chấp nhận / Tolerate):** Biết có rủi ro nhưng chi phí xử lý lớn hơn thiệt hại, nên chấp nhận sống chung. Chia làm *Active Acceptance* (chấp nhận nhưng trích sẵn quỹ dự phòng thời gian/ngân sách - Contingency Reserve) và *Passive Acceptance* (không làm gì, xảy ra mới tính).

#### D. Stakeholder & Communication Management (Quản lý Các bên liên quan & Giao tiếp)
1. **Phân loại Stakeholder theo Ma trận Power / Interest Grid:**
   * **High Power – High Interest (Manage Closely - Quản lý sát sao):** Ban Giám khảo VPBank, Mentor chuyên môn, Product Owner. $\rightarrow$ Tương tác thường xuyên, mời tham dự Sprint Review, lấy phản hồi sớm.
   * **High Power – Low Interest (Keep Satisfied - Giữ hài lòng):** Lãnh đạo cấp cao / Ban Tổ chức chung. $\rightarrow$ Báo cáo tóm tắt cấp điều hành (Executive Summary), không làm phiền bằng chi tiết kỹ thuật vụn vặt.
   * **Low Power – High Interest (Keep Informed - Thông báo đầy đủ):** Người dùng thử nghiệm (Pilot Users), các bộ phận nghiệp vụ liên quan. $\rightarrow$ Cập nhật bản tin tiến độ, hướng dẫn sử dụng.
   * **Low Power – Low Interest (Monitor - Theo dõi tối thiểu):** Các bên ít liên đới.
2. **Cách báo cáo tiến độ chuẩn của PM/SM:**
   * Sử dụng **Information Radiators (Bảng phát thông tin trực quan):** Kanban Board, Sprint Burndown, Release Burnup, Risk Heatmap được cập nhật theo thời gian thực để ai nhìn vào trong 30 giây cũng nắm được sức khỏe dự án.
   * Khi báo cáo cho cấp lãnh đạo/Stakeholders khi dự án gặp sự cố: Luôn tuân thủ cấu trúc **Sự thật minh bạch (Current Status) $\rightarrow$ Tác động đến mục tiêu (Impact on Goal) $\rightarrow$ Phương án đề xuất kèm đánh đổi (Options & Trade-offs)** thay vì giấu lỗi hoặc chỉ nêu vấn đề mà không có giải pháp.
3. **Điều phối xung đột nội bộ dưới áp lực thời gian cao (Hackathon / Nước rút):**
   * **Xung đột phổ biến 1: DEV vs. QA** (*"Máy tôi vẫn chạy được mà!", "Đây là tính năng chứ không phải bug!"*).
     * *Cách PM/SM giải quyết:* Đưa cuộc tranh luận quay về **tiêu chuẩn khách quan** là **Acceptance Criteria (AC)** và **Definition of Done (DoD)**, không tranh cãi cảm tính. Nếu AC chưa bao phủ trường hợp đó, gọi ngay **PO** vào quyết định xem hành vi đó có cần sửa ngay để đạt Sprint Goal hay tạo thành một PBI mới cho Sprint sau.
   * **Xung đột phổ biến 2: PO/BA muốn nhiều tính năng hoành tráng vs. DEV cảnh báo không kịp thời gian.**
     * *Cách PM/SM giải quyết:* Sử dụng **Tam giác Ràng buộc Agile (Agile Iron Triangle)**: Trong Agile, **Thời gian (Timebox)** và **Nguồn lực (5 người)** cùng **Chất lượng (DoD)** là **CỐ ĐỊNH**; biến số duy nhất được phép co giãn là **Phạm vi (Scope)**. PM điều phối để PO áp dụng **MoSCoW** cắt bỏ ngay các phần *Could-have*, giữ vững các phần *Must-have* chạy mượt mà 100%.

```text
          TAM GIÁC TRUYỀN THỐNG (WATERFALL)             TAM GIÁC AGILE (ĐẢO NGƯỢC)
                  [ Phạm vi (Scope) ]                 [ Thời gian ] --- [ Chi phí/Nhân sự ]
                     (CỐ ĐỊNH)                               (CỐ ĐỊNH)       (CỐ ĐỊNH)
                       /    \                                    \             /
                      /      \                                    \           /
                     /        \                                    \         /
                    /  Chất    \                                    \Chất lượng/
                   /   lượng    \                                    \ (DoD) /
                  /______________\                                    \     /
         [ Thời gian ]        [ Chi phí ]                              \   /
          (Biến đổi)          (Biến đổi)                          [ Phạm vi (Scope) ]
                                                                     (LINH HOẠT)
```

---

## PHẦN 4: BỘ 25 CÂU HỎI TRẮC NGHIỆM TÌNH HUỐNG ÔN THI VÒNG 1 (CÓ GIẢI THÍCH CHI TIẾT)

> **Hướng dẫn ôn luyện:** Các câu hỏi dưới đây được thiết kế ở mức độ **Trung bình – Khó (Situational & Trap Questions)** theo đúng chuẩn đề thi chứng chỉ quốc tế (PSM I / PSPO I / PMI-ACP) kết hợp bối cảnh dự án AI Agent ngân hàng tại Hack4Biz. Hãy chú ý phân tích kỹ **từ khóa bẫy (trap keywords)** trong từng phương án.

---

### Nhóm 1: Ranh giới Quyền hạn & Trách nhiệm (PM / Scrum Master / PO / Developers)

**Câu 1 [Bẫy can thiệp giữa Sprint]:** Đang ở Ngày thứ 4 của Sprint 1 (kéo dài 1 tuần), một Giám đốc Khối Nghiệp vụ Thẻ của ngân hàng (Key Stakeholder) nhắn tin trực tiếp cho DEV yêu cầu bổ sung gấp một nút *"Xuất báo cáo sao kê ra file PDF có chữ ký số"* vì cho rằng tính năng này chỉ mất khoảng 3 giờ code. Với vai trò là Scrum Master / PM của đội, hành động đúng đắn nhất bạn cần hướng dẫn cho DEV và thực hiện là gì?
* **A.** Bảo DEV cứ tranh thủ làm nhanh trong 3 giờ để làm hài lòng Stakeholder quan trọng, sau đó báo lại cho PO vào buổi Daily Scrum ngày mai.
* **B.** Yêu cầu DEV từ chối thẳng thừng và chặn tin nhắn của vị Giám đốc vì quy định của Scrum là không ai được nói chuyện với Developers trong Sprint.
* **C.** Hướng dẫn DEV lịch sự giải thích rằng mọi công việc trong Sprint phải phục vụ cho Sprint Goal đã cam kết, đề nghị Stakeholder trao đổi trực tiếp với Product Owner (PO) để PO đánh giá và sắp xếp vào Product Backlog; đồng thời SM gặp Stakeholder để giải thích cơ chế làm việc của Scrum.
* **D.** Với tư cách là PM, bạn trực tiếp phê duyệt yêu cầu này, tự tay thêm một ticket mới vào Sprint Backlog hiện tại và giao cho DEV làm ngay.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Trong Scrum, **Product Backlog là nguồn công việc duy nhất** và **PO là cổng tiếp nhận duy nhất** có quyền quyết định thứ tự ưu tiên. Developers không nhận việc trực tiếp từ Stakeholder bên ngoài để tránh **Scope Creep** và bảo vệ sự tập trung (**Focus**) vào **Sprint Goal**. Phương án A và D phá vỡ quyền của PO và tính tự quản của Developers; phương án B thiếu tinh thần hợp tác (Scrum không cấm giao tiếp, chỉ cấm tự ý thay đổi phạm vi Sprint Backlog không qua PO).

---

**Câu 2 [Bẫy quyền Hủy Sprint]:** Trong quá trình phát triển MVP AI Agent, Ngân hàng Nhà nước vừa ban hành thông tư mới cấm hoàn toàn việc sử dụng cơ chế xác thực qua SMS OTP không mã hóa cho phân khúc giao dịch đang xây dựng, khiến **Sprint Goal** của Sprint hiện tại hoàn toàn không còn giá trị sử dụng. Ai là người có thẩm quyền quyết định hủy bỏ (Cancel) Sprint này?
* **A.** Project Manager sau khi họp xin ý kiến Ban Giám khảo.
* **B.** Scrum Master vì Scrum Master là người quản lý các sự kiện và quy trình Scrum.
* **C.** Nhóm Developers biểu quyết theo đa số vì họ là người trực tiếp viết code.
* **D.** Duy nhất Product Owner (PO) mới có quyền hủy Sprint (dù có thể lắng nghe tư vấn từ Stakeholders, Developers hoặc Scrum Master).

> **Đáp án đúng:** **D**  
> **Giải thích nguyên lý:** Theo Scrum Guide 2020, **chỉ duy nhất Product Owner có thẩm quyền hủy một Sprint** khi Sprint Goal trở nên lỗi thời (obsolete). Không ai khác (kể cả PM, SM hay CEO) có quyền này trong khung Scrum.

---

**Câu 3 [Bẫy quyền Ước lượng & Chọn việc vào Sprint]:** Trong buổi Sprint Planning, Product Owner (PO) muốn đưa 10 User Stories (tổng cộng 45 Story Points) vào Sprint 2 để kịp ngày Demo. Tuy nhiên, dựa trên Velocity của Sprint 1 (chỉ đạt 28 Story Points) và việc 1 thành viên bận lịch cá nhân, nhóm Developers (BA, DEV, QA) khẳng định họ chỉ có thể nhận tối đa 25 Story Points. PO phản đối và cho rằng nhóm ước lượng "quá phóng đại" một số tính năng AI đơn giản. Ai là người có quyền quyết định cuối cùng về con số ước lượng và số lượng hạng mục đưa vào Sprint Backlog?
* **A.** Product Owner, vì PO chịu trách nhiệm tối đa hóa giá trị sản phẩm và cam kết với khách hàng.
* **B.** Project Manager / Scrum Master sẽ đứng ra lấy trung bình cộng là 35 Story Points để cả hai bên cùng vui vẻ.
* **C.** Nhóm Developers, vì những người trực tiếp thực hiện công việc là người duy nhất chịu trách nhiệm ước lượng kích thước công việc và quyết định lượng việc họ có thể kéo vào Sprint.
* **D.** Chỉ riêng thành viên Senior DEV có quyền chốt con số ước lượng, BA và QA không được tham gia.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Theo Scrum Guide, **Developers** sở hữu độc quyền việc ước lượng (Sizing) và tự quyết định số lượng Product Backlog Items kéo vào Sprint. PO chỉ quyết định **thứ tự ưu tiên** (cái nào quan trọng nhất đứng ở trên cùng để Developers kéo vào trước). Nếu PO thấy 25 SP là ít, PO có thể cùng Developers đàm phán thu hẹp phạm vi chi tiết hoặc chia nhỏ Story để lấy phần lõi có giá trị cao nhất, tuyệt đối không được ép nhận 45 SP.

---

**Câu 4 [Bẫy RACI & Ủy quyền của PO]:** Trong đội 5 người tại Hack4Biz, vì Product Owner (PO) bận nghiên cứu chiến lược kinh doanh và chuẩn bị bài Pitching nên đã giao cho Business Analyst (BA) trực tiếp viết các User Stories, vẽ luồng nghiệp vụ và sắp xếp lại một số hạng mục trên bảng Product Backlog. Phát biểu nào sau đây là ĐÚNG NHẤT theo chuẩn Scrum?
* **A.** Việc này vi phạm nghiêm trọng Scrum Guide vì không ai ngoài PO được phép chạm vào Product Backlog.
* **B.** BA lúc này chính thức trở thành đồng Product Owner (Co-Product Owner), trách nhiệm giải trình chia đều 50-50 cho PO và BA.
* **C.** Hoàn toàn hợp lệ: PO có thể ủy quyền (delegate) việc thực hiện các tác vụ quản lý Product Backlog cho người khác (BA/Developers), nhưng PO vẫn là người duy nhất chịu trách nhiệm giải trình cuối cùng (Accountable).
* **D.** Scrum Master phải lập tức thu hồi quyền truy cập Jira của BA và cảnh cáo PO.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Trong ma trận RACI và Scrum Guide: *"The Product Owner may do the above work or may delegate the responsibility to others. Regardless, the Product Owner remains accountable."* (PO có thể tự làm hoặc ủy quyền công việc cho BA/Developers thực hiện — tức BA giữ vai trò **R - Responsible**, nhưng PO luôn giữ duy nhất chữ **A - Accountable**).

---

**Câu 5 [Bẫy vai trò PM trong Agile Hybrid vs. Scrum Master]:** Điểm khác biệt cốt lõi nhất giữa một **Project Manager theo lối chỉ huy truyền thống (Command-and-Control PM)** và một **Scrum Master / Agile PM** khi điều hành đội dự án là gì?
* **A.** PM truyền thống không quan tâm đến tiến độ, còn Scrum Master ép tiến độ gắt gao hơn mỗi ngày.
* **B.** PM truyền thống trực tiếp phân chia task cho từng cá nhân và kiểm soát việc tuân thủ kế hoạch cố định; trong khi Scrum Master / Agile PM đóng vai trò Lãnh đạo phục vụ (Servant Leader), tạo môi trường cho đội tự quản lý (Self-managing), tháo gỡ trở ngại (Impediments) và tối ưu hóa dòng chảy giá trị thích ứng.
* **C.** Scrum Master là cấp trên trực tiếp có quyền duyệt tăng lương và đuổi việc các Developers, còn PM truyền thống thì không.
* **D.** Agile PM chỉ làm công việc hành chính như đặt lịch họp và ghi biên bản mà không cần hiểu về quản trị rủi ro hay các bên liên quan.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Chuyển dịch tư duy lớn nhất sang Agile là từ **Command-and-Control** (Chỉ huy & Kiểm soát vi mô) sang **Servant Leadership** (Lãnh đạo phục vụ) và trao quyền cho **Self-managing Team** (Đội tự quản). Phương án D là hiểu lầm tai hại (Anti-pattern biến SM thành thư ký).

---

### Nhóm 2: 5 Sự kiện Scrum (Scrum Events & Anti-patterns)

**Câu 6 [Bẫy Daily Scrum]:** Trong buổi họp Daily Scrum kéo dài 15 phút của đội Hack4Biz, Scrum Master / PM nhận thấy cả 3 thành viên (BA, DEV, QA) đều quay mặt về phía mình để lần lượt báo cáo: *"Hôm qua em đã làm đủ 8 tiếng, hôm nay em làm tiếp task X"*, đồng thời PO liên tục ngắt lời để chất vấn tại sao DEV code chậm và thảo luận sâu về thuật toán RAG khiến cuộc họp kéo dài sang phút thứ 35. Có bao nhiêu lỗi sai (Anti-patterns) trong tình huống này và cách khắc phục đúng là gì?
* **A.** Không có lỗi nào, miễn là PM và PO nắm được tình hình chi tiết của từng người là tốt.
* **B.** Có 3 lỗi: (1) Biến Daily Scrum thành buổi báo cáo cho cấp trên thay vì Developers tự đồng bộ kế hoạch với nhau hướng tới Sprint Goal; (2) PO can thiệp làm gián đoạn cuộc họp của Developers; (3) Thảo luận kỹ thuật chi tiết làm lố Timebox 15 phút. Cách khắc phục: SM huấn luyện lại mục đích Daily Scrum là của Developers và dành cho Developers, giữ đúng 15 phút, và tách phần thảo luận thuật toán sâu sang buổi họp riêng ngay sau đó (Parking Lot / After-party).
* **C.** Lỗi duy nhất là họp 35 phút hơi ngắn, SM nên tăng Timebox của Daily Scrum lên 60 phút mỗi ngày.
* **D.** SM nên cấm tuyệt đối PO không được có mặt trong phòng họp lúc diễn ra Daily Scrum và phạt tiền ai nói quá 3 phút.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Daily Scrum là sự kiện **15 phút dành cho Developers** để thanh tra tiến độ hướng tới **Sprint Goal** và lập kế hoạch cho 24 giờ tới. Nó không phải là buổi báo cáo trạng thái (Status Meeting) cho PM/SM/PO. Các thảo luận giải pháp kỹ thuật sâu phải được đưa vào *Parking Lot* để xử lý ngay sau khi kết thúc 15 phút Daily Scrum.

---

**Câu 7 [Bẫy cuối Sprint không kịp hoàn thành Backlog]:** Còn 1 ngày nữa là kết thúc Sprint 1 (Timebox 1 tuần). Nhóm Developers nhận ra rằng trong số 6 User Stories đã chọn vào Sprint Backlog, họ chắc chắn chỉ hoàn thành trọn vẹn (đạt DoD) được 4 Stories; còn 2 Stories (liên quan đến tính năng *Gợi ý sản phẩm thẻ phụ* và *Đổi giao diện Dark Mode*) mới chỉ code xong 70% và chưa qua QA kiểm thử. Tuy nhiên, **Sprint Goal** cốt lõi là *"Xây dựng thành công luồng AI Agent tư vấn mở thẻ tín dụng chính xác"* đã đạt được qua 4 Stories đầu. Nhóm nên xử lý như thế nào?
* **A.** Kéo dài Sprint 1 thêm 2 ngày nữa cho đến khi code và test xong toàn bộ 6 Stories rồi mới tổ chức Sprint Review.
* **B.** Bỏ qua bước QA kiểm thử của 2 Stories cuối, đánh dấu "Done" luôn cho cả 6 Stories để đạt 100% kế hoạch và đem tất cả ra trình diễn ở buổi Sprint Review.
* **C.** Kết thúc Sprint đúng hạn (giữ nguyên Timebox). Nhóm Developers minh bạch trao đổi ngay với PO, chỉ đưa 4 Stories đã đạt 100% DoD vào bản Increment để trình diễn tại Sprint Review; 2 Stories chưa hoàn thành được trả về Product Backlog để PO xem xét ưu tiên và ước lượng lại cho Sprint 2. Đồng thời đưa vấn đề ước lượng/quản lý khối lượng việc vào thảo luận tại buổi Sprint Retrospective.
* **D.** Tính điểm Velocity của Sprint 1 bằng tổng điểm của 4 Stories đầu cộng với 70% số điểm của 2 Stories dở dang.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Đây là câu hỏi kinh điển kiểm tra 3 nguyên tắc bất di bất dịch của Scrum:
> 1. **Timebox là cố định** (Không bao giờ kéo dài Sprint - loại A).
> 2. **Chất lượng (DoD) là không thỏa hiệp** (Không bao giờ hạ chuẩn DoD hay đem hàng chưa Done ra Sprint Review - loại B).
> 3. **Không tính điểm một phần (No partial credit)** cho Story chưa đạt DoD (loại D).

---

**Câu 8 [Bẫy Sprint Review]:** Phát biểu nào sau đây mô tả ĐÚNG NHẤT bản chất của sự kiện **Sprint Review** theo Scrum Guide?
* **A.** Là cổng phê duyệt chính thức (Formal Sign-off Gate) nơi Stakeholders ký biên bản nghiệm thu; nếu Stakeholders chưa ký thì Sprint chưa được phép kết thúc.
* **B.** Là buổi thuyết trình một chiều bằng slide PowerPoint do PM thực hiện để báo cáo tỷ lệ giải ngân và số giờ làm việc của từng thành viên.
* **C.** Là một phiên làm việc hợp tác (Working Session) giữa Scrum Team và các Stakeholders để cùng thanh tra bản Increment đạt chuẩn DoD, thảo luận về những gì đã làm được, bối cảnh thay đổi và cùng điều chỉnh Product Backlog nhằm tối đa hóa giá trị cho kỳ tiếp theo.
* **D.** Là buổi họp nội bộ chỉ gồm DEV, BA, QA để kiểm điểm xem ai gây ra nhiều bug nhất trong Sprint.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Scrum Guide nhấn mạnh: *"The Sprint Review is a working session and the Scrum Team should avoid limiting it to a presentation."* Nó không phải là một cổng phê duyệt chặn (Phase gate) hay buổi thuyết trình slide, mà là buổi làm việc hai chiều dựa trên **Working Software (Increment đạt DoD)** để cập nhật **Product Backlog**.

---

**Câu 9 [Bẫy Sprint Retrospective & DoD]:** Trong buổi **Sprint Retrospective** cuối Sprint 1, QA phản ánh rằng nhiều lỗi Prompt Injection cơ bản của AI Agent bị lọt sang môi trường Staging vì DEV không chạy bộ script kiểm tra bảo mật trước khi đẩy code. Để ngăn lỗi này lặp lại ở Sprint 2, giải pháp nào sau đây là chuẩn xác và bền vững nhất theo cơ chế Scrum?
* **A.** PM ra quy định phạt tiền DEV mỗi khi QA tìm thấy lỗi bảo mật.
* **B.** Cả Scrum Team thống nhất nâng cấp / mở rộng **Definition of Done (DoD)** bằng cách bổ sung tiêu chí: *"100% câu trả lời và cấu hình Prompt của AI phải vượt qua bộ Automated Security & Guardrail Check trước khi chuyển sang cột Ready for QA"*, và áp dụng ngay từ Sprint 2.
* **C.** Yêu cầu BA viết lại toàn bộ tài liệu BRD dài gấp đôi hiện tại.
* **D.** Bỏ qua vì Sprint Retrospective chỉ dùng để xả stress và khen ngợi nhau, không được thay đổi quy trình kỹ thuật.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Mục đích của **Sprint Retrospective** là lên kế hoạch cải tiến chất lượng và hiệu quả làm việc. Một trong những đầu ra quan trọng nhất được Scrum Guide khuyến nghị trong Retrospective là **điều chỉnh Definition of Done (DoD)** ngày càng chặt chẽ hơn khi năng lực của đội trưởng thành hơn.

---

**Câu 10 [Bẫy Backlog Refinement]:** Khi được hỏi về hoạt động **Product Backlog Refinement (Grooming)**, một ứng viên PM trả lời rằng: *"Backlog Refinement là sự kiện chính thức thứ 6 của Scrum, bắt buộc diễn ra vào chiều thứ Tư hàng tuần với Timebox cố định 4 giờ và chỉ có PO với BA tham gia"*. Câu trả lời này sai ở những điểm nào?
* **A.** Hoàn toàn đúng, không sai ở điểm nào.
* **B.** Sai ở chỗ Refinement chỉ do một mình Scrum Master thực hiện.
* **C.** Sai ở 3 điểm: (1) Refinement là hoạt động diễn ra liên tục (ongoing activity) chứ KHÔNG phải là sự kiện chính thức (Scrum chỉ có đúng 5 Events); (2) Không có Timebox cố định bắt buộc (thường chỉ chiếm $\le 10\%$ thời lượng của Sprint khi cần); (3) Cần sự tham gia của cả PO và nhóm Developers (DEV, BA, QA) để cùng làm rõ và ước lượng chứ không chỉ riêng PO và BA.
* **D.** Sai ở chỗ trong Agile không cần chuẩn bị trước Backlog, cứ vào buổi Sprint Planning mới bắt đầu nghĩ xem nên làm tính năng gì.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Đề thi rất hay gài bẫy rằng *"Scrum có 6 sự kiện bao gồm Backlog Refinement"*. Hãy nhớ: Scrum chỉ có **5 Events** (*Sprint, Sprint Planning, Daily Scrum, Sprint Review, Sprint Retrospective*). Refinement là một hoạt động thường xuyên cực kỳ quan trọng để chuẩn bị các PBIs đạt chuẩn **DoR** trước kỳ Planning.

---

### Nhóm 3: Biểu đồ, Chỉ số & Kỹ thuật Quản lý (Burndown, CFD, Velocity, Estimation, Backlog)

**Câu 11 [Bẫy phân tích Sprint Burndown Chart]:** Quan sát **Sprint Burndown Chart** của một Sprint kéo dài 8 ngày, bạn thấy từ Ngày 1 đến Ngày 6 đường thực tế (Actual Line) hầu như **đi ngang (Flatline)** ở mức 35 Story Points, sau đó vào Ngày 8 đường này đột ngột rơi thẳng đứng xuống mốc 5 Story Points. Nguyên nhân nào sau đây giải thích hợp lý nhất cho hiện tượng này?
* **A.** Đội dự án làm việc với tốc độ cực kỳ đều đặn và hoàn thành các User Story nhỏ mỗi ngày.
* **B.** Đội đang mắc bệnh **"Mini-Waterfall trong Sprint"** (ví dụ: DEV gom toàn bộ các Story lại code từ Ngày 1 đến Ngày 6 rồi mới chuyển đồng loạt sang cho QA test vào Ngày 7–8), hoặc các User Story có kích thước quá lớn (vi phạm tiêu chí **S - Small** trong INVEST) nên phải đến ngày cuối cùng mới hoàn tất đạt chuẩn DoD.
* **C.** Product Owner liên tục xóa bớt các User Story khỏi Sprint vào mỗi buổi sáng từ Ngày 1 đến Ngày 6.
* **D.** Đây là hình dáng lý tưởng nhất của một biểu đồ Sprint Burndown.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Burndown chỉ giảm xuống khi một PBI (hoặc Task) hoàn thành. Đường đi ngang suốt 6 ngày rồi rơi thẳng đứng ở ngày cuối (*Cliff Drop*) là dấu hiệu kinh điển của: (1) Story quá to chưa chia nhỏ; (2) Bàn giao theo lô lớn (*Batch handoff / Mini-Waterfall*) gây nghẽn ở QA vào cuối kỳ; hoặc (3) Team không cập nhật trạng thái công việc hàng ngày.

---

**Câu 12 [Bẫy phân tích Cumulative Flow Diagram - CFD]:** Khi theo dõi biểu đồ **Cumulative Flow Diagram (CFD)** của dự án trong 2 tuần qua, PM nhận thấy dải màu của trạng thái **"In Development (DEV)"** có độ dày chiều dọc không đổi, nhưng dải màu ngay bên dưới nó là **"In Testing (QA)"** lại ngày càng phình to ra theo chiều dọc, trong khi đường biên của trạng thái **"Done"** có độ dốc rất thấp. Dựa trên Định luật Little (Little's Law) và nguyên lý Kanban/Scrum, chẩn đoán và hành động nào sau đây là ĐÚNG?
* **A.** Khâu QA đang quá nhàn rỗi, cần giao thêm việc viết tài liệu cho QA.
* **B.** Hệ thống đang bị **Điểm nghẽn (Bottleneck) tại khâu Kiểm thử (QA)**: Tốc độ DEV đẩy ticket sang nhanh hơn tốc độ QA có thể kiểm thử, làm lượng WIP ở cột Testing tăng vọt và kéo dài Cycle Time tổng thể. Giải pháp: Đặt giới hạn **WIP Limit** và yêu cầu DEV ngừng kéo Story mới, thay vào đó cùng hỗ trợ (Swarming) giải quyết tồn đọng kiểm thử (viết automated test, fix bug tồn, chuẩn bị test data).
* **C.** Khâu BA đang bị nghẽn nên DEV không có việc để làm.
* **D.** Yêu cầu DEV code nhanh gấp đôi nữa để đẩy thêm nhiều ticket sang cột QA hơn.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Trên biểu đồ CFD, dải màu nào **phình rộng ra theo chiều dọc (WIP tăng)** thì công việc đang bị ứ đọng ngay tại công đoạn đó. Nếu DEV cứ tiếp tục đẩy thêm việc mới sang (Phương án D), nút thắt cổ chai ở QA càng trầm trọng hơn và cuối Sprint sẽ không có Story nào kịp sang cột *Done*. Giải pháp chuẩn Agile là *"Stop starting, start finishing"* (Ngừng mở việc mới, tập trung hoàn thành việc đang dở bằng **WIP Limit** và **Swarming**).

---

**Câu 13 [Bẫy tính Velocity & Lạm phát điểm]:** Đội A có Velocity trung bình là **40 Story Points/Sprint**. Đội B (cũng gồm 5 người làm một phân hệ khác) có Velocity trung bình là **80 Story Points/Sprint**. Giám đốc dự án kết luận rằng Đội B làm việc năng suất gấp đôi Đội A và yêu cầu Đội A trong Sprint tới phải nâng Velocity lên 80 Story Points nếu không sẽ bị trừ điểm thi đua. Nhận định nào sau đây của Agile Coach / PM là ĐÚNG?
* **A.** Quyết định của Giám đốc hoàn toàn chính xác vì Story Point là đơn vị đo lường chuẩn quốc tế giống như giờ đồng hồ.
* **B.** Kết luận của Giám đốc là **SAI hoàn toàn**. Story Point là đơn vị ước lượng tương đối và mang tính nội bộ của từng đội (dựa trên Story mốc riêng của đội đó). Việc so sánh Velocity giữa hai đội khác nhau hoặc dùng Velocity làm KPI thưởng/phạt sẽ dẫn đến hiện tượng **Lạm phát điểm (Point Inflation)** — Đội A sẽ chỉ cần nhân đôi số điểm ước lượng của mỗi Story từ `3 SP` lên `6 SP` để đạt 80 SP trên giấy tờ mà giá trị thực tế tạo ra không hề tăng, đồng thời làm hỏng tính minh bạch của dữ liệu dự báo.
* **C.** Đội A nên cắt bỏ bước kiểm thử của QA để tăng gấp đôi số Story Points hoàn thành theo yêu cầu của Giám đốc.
* **D.** Scrum Master của Đội A nên tự ý sửa số điểm trên phần mềm Jira sau khi Sprint kết thúc để báo cáo lên Giám đốc cho đẹp.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** *“Velocity is a measure of capacity, NOT a measure of productivity or performance comparison across teams.”* (Velocity là công cụ nội bộ giúp một đội tự dự báo khối lượng công việc cho các Sprint tiếp theo của chính đội đó, tuyệt đối không dùng để so sánh giữa các đội hay làm KPI ép chỉ tiêu).

---

**Câu 14 [Bẫy kỹ thuật Spike trong Agile]:** Trong buổi Backlog Refinement, PO đưa ra một hạng mục: *"Tích hợp mô hình nhận diện giọng nói tiếng Việt theo thời gian thực có khả năng lọc tiếng ồn quán cà phê cho AI Agent"*. Cả DEV, BA và QA đều chưa từng làm công nghệ này nên không biết phải dùng thư viện nào, độ trễ ra sao và hoàn toàn không thể ước lượng được Story Points cho hạng mục này. Cách xử lý đúng đắn nhất trong Agile Scrum là gì?
* **A.** Cứ nhắm mắt gán đại một con số thật to là `100 Story Points` rồi kéo luôn vào Sprint để vừa làm vừa mò.
* **B.** Từ chối vĩnh viễn không bao giờ làm tính năng này vì vi phạm tiêu chí Estimable.
* **C.** Tạo một **Spike** (một tác vụ nghiên cứu / thử nghiệm kỹ thuật hoặc làm Prototype nhỏ có giới hạn thời gian cố định — ví dụ Timebox tối đa 4 giờ hoặc 1 ngày trong Sprint) để tìm hiểu tính khả thi và kiến trúc kỹ thuật; kết quả đầu ra của Spike sẽ cung cấp đủ thông tin giúp đội chia nhỏ và ước lượng chính xác User Story chính.
* **D.** Bắt Scrum Master tự đi học lập trình AI rồi về ước lượng hộ cho DEV.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Khi một PBI có độ bất định quá cao khiến đội không thể ước lượng (chưa đạt chữ **E - Estimable** trong INVEST), Agile sử dụng kỹ thuật **Spike** (Technical Spike hoặc Functional Spike). Spike luôn được gắn một **Timebox nghiêm ngặt** nhằm mục đích mua thông tin / giảm thiểu rủi ro bất định trước khi ước lượng và cam kết xây dựng tính năng hoàn chỉnh.

---

**Câu 15 [Bẫy chia nhỏ User Story - Vertical vs. Horizontal Slicing]:** Một Epic lớn là *"Khách hàng tra cứu và khiếu nại giao dịch thẻ tín dụng qua AI Agent"* được ước lượng sơ bộ là `21 Story Points` (quá lớn cho 1 Sprint). BA đề xuất tách Epic này thành 3 User Stories nhỏ cho Sprint 1 như sau:
* *Story 1 (5 SP):* Thiết kế toàn bộ các bảng Database cho lịch sử giao dịch và phiếu khiếu nại.
* *Story 2 (8 SP):* Viết toàn bộ Backend API và cấu hình Prompt LLM.
* *Story 3 (8 SP):* Xây dựng toàn bộ giao diện màn hình Chat Frontend trên React.
Cách chia này mắc lỗi gì theo nguyên lý **INVEST** và nên sửa lại như thế nào?
* **A.** Cách chia này hoàn toàn chuẩn xác vì phân rõ việc của từng chuyên môn.
* **B.** Mắc lỗi **Horizontal Slicing (Chia cắt ngang theo tầng kỹ thuật)**, vi phạm tiêu chí **V (Valuable)** và **I (Independent)** trong INVEST — vì nếu cuối Sprint chỉ hoàn thành được Story 1 và Story 2 mà chưa xong Story 3 thì người dùng cuối / khách hàng hoàn toàn không thể sử dụng hay trải nghiệm được bất kỳ giá trị nào. Cần sửa lại theo hướng **Vertical Slicing (Chia lát cắt dọc theo kịch bản nghiệp vụ đầu-cuối)**: ví dụ *Story 1: Khách hàng chat tra cứu danh sách 5 giao dịch gần nhất (có đủ DB + Backend/AI + UI)*; *Story 2: Khách hàng chọn 1 giao dịch để gửi yêu cầu tra soát cơ bản*; *Story 3: Khách hàng đính kèm hình ảnh hóa đơn chứng từ vào phiếu tra soát*.
* **C.** Chỉ cần đổi tên "User Story" thành "Technical Task" là có thể đem đi trình diễn với khách hàng ở buổi Sprint Review.
* **D.** Nên gộp cả 3 Story lại thành 1 Story 21 SP như cũ để khỏi phải chia.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Một **User Story** đúng chuẩn phải mang lại giá trị có thể kiểm chứng từ góc nhìn người dùng (**Valuable**) và tạo ra một lát cắt tính năng chạy được xuyên qua các tầng kỹ thuật (**Vertical Slice**). Nếu chia theo tầng kỹ thuật (DB riêng, API riêng, UI riêng), từng mảnh rời rạc không tạo ra một **Usable Increment** độc lập.

---

**Câu 16 [Bẫy DoR vs. DoD]:** Nhận định nào sau đây phân biệt ĐÚNG giữa **Definition of Ready (DoR)** và **Definition of Done (DoD)**?
* **A.** DoR là tiêu chuẩn bắt buộc để kết thúc Sprint, còn DoD là tiêu chuẩn để bắt đầu Sprint Planning.
* **B.** Cả DoR và DoD đều là hai Cam kết chính thức (Formal Commitments) được quy định bắt buộc trong Scrum Guide 2020.
* **C.** **DoD** là Cam kết chính thức gắn với **Increment** trong Scrum Guide nhằm đảm bảo tính minh bạch về chất lượng của sản phẩm hoàn thành; trong khi **DoR** là một thực hành bổ trợ (Complementary Practice) giúp kiểm tra xem một PBI ở đầu Product Backlog đã đủ rõ ràng, đủ nhỏ và khả thi trước khi đưa vào **Sprint Planning** hay chưa.
* **D.** DoR chỉ áp dụng cho QA, còn DoD chỉ áp dụng cho DEV.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Trong Scrum Guide 2020 chỉ có đúng 3 Commitments chính thức: *Product Goal* (cho Product Backlog), *Sprint Goal* (cho Sprint Backlog) và *Definition of Done* (cho Increment). **DoR** không nằm trong Scrum Guide chính thức mà là một thực hành bổ trợ ở cổng đầu vào (Input) của Sprint Planning.

---

### Nhóm 4: Nghiệp vụ Quản trị Dự án của PM (Risk, Schedule, Change, Conflict, AI Specifics)

**Câu 17 [Bẫy phân biệt Risk vs. Issue/Impediment]:** Trong buổi họp rà soát dự án AI Agent vào sáng thứ Hai, đội ghi nhận hai thông tin sau:
* *(Thông tin 1):* "Nếu trong buổi chung kết trực tiếp, mạng Wifi của hội trường bị nghẽn băng thông thì hệ thống Voice AI Agent của chúng ta có thể bị trễ phản hồi quá 10 giây."
* *(Thông tin 2):* "Hiện tại tài khoản Google Cloud chứa Vector Database của nhóm vừa bị hệ thống khóa tự động từ 8h sáng nay do thẻ thanh toán hết hạn, khiến DEV và QA đang không thể truy cập môi trường Staging để làm việc."
Cách phân loại và hành động xử lý của PM đối với hai thông tin này là gì?
* **A.** Cả hai đều là Rủi ro (Risks), chỉ cần ghi vào sổ Risk Register và đợi đến cuối tuần sau mới xem xét.
* **B.** *(Thông tin 1)* là một **Risk (Rủi ro — sự kiện bất định trong tương lai)**: PM cần đưa vào **Risk Register**, đánh giá Xác suất $\times$ Tác động và lập kế hoạch **Mitigation / Contingency** (ví dụ: chuẩn bị sẵn cục phát 4G/5G riêng + cấu hình bản Local Fallback/Cache). *(Thông tin 2)* là một **Issue / Impediment (Vấn đề / Trở ngại đã xảy ra ở hiện tại)**: PM / Scrum Master phải lập tức hành động tháo gỡ ngay trong ngày (Escalate / đổi phương thức thanh toán hoặc kích hoạt tài khoản backup) để giải phóng cho DEV và QA làm việc.
* **C.** *(Thông tin 1)* là Issue, còn *(Thông tin 2)* là Risk.
* **D.** Cả hai đều không thuộc phạm vi quan tâm của PM vì nhóm Developers phải tự bỏ tiền túi ra mua server mới.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Phân biệt rõ: **Risk** = *Might happen* (Tương lai $\rightarrow$ Quản lý bằng Risk Register & Mitigation/Contingency Plan). **Issue / Impediment** = *Has happened / Is happening now* (Hiện tại $\rightarrow$ Quản lý bằng Issue Log & Immediate Resolution / Escalation).

---

**Câu 18 [Bẫy Chiến lược ứng phó Rủi ro trong dự án AI Ngân hàng]:** Khi xây dựng AI Agent cho VPBank, đội nhận diện một rủi ro cực kỳ nghiêm trọng (Impact = 5/5): *"Mô hình LLM có thể bị kẻ gian tấn công bằng kỹ thuật Prompt Injection để lừa AI tự động gọi API thực hiện lệnh chuyển tiền trái phép từ tài khoản khách hàng sang tài khoản kẻ gian"*. Đội quyết định thay đổi thiết kế kiến trúc: **Bỏ hoàn toàn quyền tự động gọi API chuyển tiền trực tiếp của LLM**; thay vào đó, AI Agent chỉ được phép tạo "Bản nháp giao dịch (Draft Transaction)" trên giao diện và bắt buộc khách hàng phải tự bấm nút xác nhận kết hợp nhập mã Smart OTP từ hệ thống Core Banking truyền thống. Chiến lược ứng phó rủi ro này thuộc loại nào?
* **A.** Risk Acceptance (Chấp nhận rủi ro).
* **B.** Risk Transfer (Chuyển giao rủi ro cho bên bảo hiểm).
* **C.** Risk Avoidance (Né tránh rủi ro — thay đổi kế hoạch/thiết kế để triệt tiêu hoàn toàn khả năng AI tự ý thực hiện giao dịch chuyển tiền trái phép).
* **D.** Passive Monitoring (Theo dõi thụ động).

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Khi ta thay đổi thiết kế hoặc cắt bỏ hoàn toàn cơ chế gây ra rủi ro sao cho xác suất xảy ra kịch bản đó giảm về **0%** (LLM không còn quyền gọi API thực thi chuyển tiền trực tiếp nữa), đó chính là chiến lược **Risk Avoidance (Né tránh rủi ro)**. Nếu vẫn cho LLM tự chuyển tiền nhưng chỉ thêm câu lệnh nhắc nhở trong System Prompt để giảm tỷ lệ bị lừa, đó mới là *Risk Mitigation (Giảm thiểu)*.

---

**Câu 19 [Bẫy Quản lý Thay đổi - Change Request trong Sprint]:** Ở giữa Sprint 2 (Vòng 2), sau khi xem bản thử nghiệm sớm, Mentor từ VPBank gợi ý một thay đổi rất hay: *"Thay vì chỉ hiển thị bảng so sánh thẻ dạng chữ, các em nên bổ sung tính năng AI tự động phân tích lịch sử chi tiêu 3 tháng gần nhất của khách hàng để tính toán số tiền hoàn (Cashback) dự kiến cho từng loại thẻ"* (ước lượng khoảng `5 Story Points`). Tính năng này rất phù hợp và giúp nâng tầm **Sprint Goal** hiện tại, nhưng công suất (Capacity) của Developers trong Sprint 2 đã kín 100%. Cách xử lý nào sau đây là chuẩn Agile nhất?
* **A.** Bắt Developers thức trắng đêm làm thêm giờ (Overtime) không lương để làm xong cả toàn bộ Sprint Backlog cũ lẫn tính năng 5 SP mới này.
* **B.** Từ chối thẳng thừng mọi góp ý của Mentor vì Sprint Backlog một khi đã lập trong buổi Sprint Planning thì tuyệt đối không được phép thay đổi bất kỳ chữ nào.
* **C.** Áp dụng nguyên tắc **Trade-off (Đánh đổi tương đương)**: Product Owner thương lượng với nhóm Developers để đưa hạng mục `5 SP` có giá trị cao này vào Sprint Backlog, đồng thời **rút ra khỏi Sprint Backlog** một hoặc hai hạng mục có độ ưu tiên thấp hơn (chưa bắt đầu làm, tổng kích thước tương đương ~`5 SP`) trả về Product Backlog để đảm bảo không vượt quá Capacity và vẫn bảo vệ được Sprint Goal.
* **D.** Lập tức hủy bỏ (Cancel) Sprint 2 để làm lại từ đầu.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Một hiểu lầm phổ biến là *"Sprint Backlog bị đóng băng 100% không được sửa đổi trong Sprint"*. Thực tế theo Scrum Guide: **Sprint Goal là cố định**, chất lượng (DoD) là cố định, còn **phạm vi chi tiết của Sprint Backlog có thể được thương lượng và điều chỉnh** giữa PO và Developers khi học hỏi được điều mới, miễn là tuân thủ nguyên tắc **Swap / Trade-off** (vào 5 SP thì phải rút ra 5 SP chưa làm) để tôn trọng Capacity của đội.

---

**Câu 20 [Bẫy Critical Path & Quản lý Phụ thuộc]:** Trong kế hoạch 16 ngày xây dựng MVP AI Agent của đội 5 người, bạn có hai nhánh công việc sau:
* **Nhánh 1 (Tổng thời gian 12 ngày nối tiếp nhau):** *BA chốt tài liệu & dữ liệu RAG (2 ngày) $\rightarrow$ DEV xây dựng Pipeline RAG + Agentic Workflow (6 ngày) $\rightarrow$ QA kiểm thử độ chính xác AI & DEV tinh chỉnh Hallucination (3 ngày) $\rightarrow$ Đóng gói môi trường Staging (1 ngày)*.
* **Nhánh 2 (Tổng thời gian 4 ngày):** *Thiết kế logo thương hiệu cho Bot, chỉnh hiệu ứng Animation màn hình chào mừng và viết trang Giới thiệu nhóm (About Us)*.
Hiện tại ở Ngày thứ 5, DEV đang gặp khó khăn khiến khâu xây dựng Pipeline RAG ở Nhánh 1 có nguy cơ trễ 2 ngày. Với vai trò là PM, quyết định điều phối nào sau đây dựa trên tư duy **Critical Path (Đường găng)** là ĐÚNG?
* **A.** Yêu cầu DEV tạm gác việc làm Pipeline RAG lại để chuyển sang làm xong trang Giới thiệu nhóm và hiệu ứng Animation ở Nhánh 2 trước cho có cái nhìn đẹp mắt.
* **B.** Nhận diện **Nhánh 1 chính là Critical Path (Đường găng, Float = 0)** quyết định sự sống còn và hạn chót của MVP. PM lập tức dồn nguồn lực bảo vệ Đường găng: cắt giảm hoặc hoãn toàn bộ phần hiệu ứng màu mè ở Nhánh 2 (có độ trôi Float lớn = 8 ngày), đồng thời huy động BA và QA hỗ trợ DEV làm sạch dữ liệu chunking, chuẩn bị sẵn bộ test prompt và gỡ nút thắt kỹ thuật ở Nhánh 1.
* **C.** Để mặc DEV tự xoay xở một mình, còn PM, PO, BA, QA đi chuẩn bị slide thuyết trình trước.
* **D.** Yêu cầu QA cắt giảm thời gian kiểm thử ở cuối Nhánh 1 từ 3 ngày xuống còn 0 ngày để bù lại 2 ngày DEV bị trễ.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Trong quản lý tiến độ dự án, **Critical Path (Đường găng)** là chuỗi tác vụ dài nhất có độ trôi tự do (**Total Float / Slack = 0**). Trễ 1 ngày trên đường găng là trễ 1 ngày của toàn dự án. PM giỏi phải biết áp dụng kỹ thuật **Fast-tracking** (gối đầu công việc giữa BA-DEV-QA) và điều chuyển nguồn lực từ các nhánh không găng (Non-critical paths có Float cao) sang hỗ trợ đường găng, tuyệt đối không cắt bỏ khâu kiểm thử chất lượng (loại D).

---

**Câu 21 [Bẫy Xung đột nội bộ DEV vs. QA]:** Trong giai đoạn nước rút 32 giờ Hackathon (Vòng 3), ở giờ thứ 20, QA phát hiện khi người dùng nhập câu hỏi có chứa ký tự emoji kèm tiếng lóng viết tắt (ví dụ: *"Thẻ tín dụng của tui bị lock rùi cứu với 😭"*), AI Agent trả về lỗi `500 Internal Server Error` do bộ tiền xử lý chuỗi (Regex Parser) của DEV không xử lý ký tự Unicode đặc biệt. DEV bực bội cãi lại: *"Ai đời khách hàng ngân hàng lại nhắn emoji, đây là lỗi của người dùng chứ không phải Bug của code! Tôi không sửa vì còn đang bận code tính năng phụ khác!"*. Với vai trò là PM / Scrum Master, bạn xử lý xung đột này như thế nào?
* **A.** Bênh vực DEV và yêu cầu QA xóa ngay bug đó đi để đội không bị mất đoàn kết.
* **B.** Mắng DEV trước mặt cả nhóm để lập uy của PM.
* **C.** Điều phối cuộc trao đổi dựa trên dữ liệu khách quan: Chiếu theo **Definition of Done (DoD)** và **Acceptance Criteria (AC)**, việc hệ thống bị sập (`HTTP 500 Crash`) trước bất kỳ đầu vào nào của người dùng trên khung chat là một lỗi nghiêm trọng (**High/Critical Severity Bug**) ảnh hưởng trực tiếp đến sự ổn định của bản Demo trước Ban Giám khảo. PM cùng PO xác nhận ưu tiên: DEV phải dừng ngay việc làm "tính năng phụ (Could-have)" để fix dứt điểm lỗi crash `HTTP 500` này của luồng chính (Must-have).
* **D.** Ghi vào biên bản rằng "Không ai có lỗi" rồi giữ nguyên lỗi `HTTP 500` đó đem đi thi thuyết trình.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Khi giải quyết xung đột kỹ thuật dưới áp lực cao, PM/SM luôn neo vào **3 điểm tựa khách quan**: (1) **DoD & Acceptance Criteria** (Không còn lỗi Critical/Crash 500); (2) **Thứ tự ưu tiên MoSCoW** (Sự ổn định của luồng *Must-have* luôn cao hơn việc code thêm tính năng *Could-have*); và (3) **Quyết định giá trị nghiệp vụ của PO**.

---

**Câu 22 [Bẫy Gold Plating - Mạ vàng sản phẩm]:** Trong khi thực hiện một User Story có yêu cầu đơn giản là *"Hiển thị biểu phí thẻ tín dụng dưới dạng bảng Markdown chuẩn trong khung chat"*, DEV tự ý dành thêm 2 ngày để tích hợp một thư viện đồ họa 3D xoay thẻ tín dụng 360 độ theo con trỏ chuột dù PO không hề yêu cầu trong Acceptance Criteria, dẫn đến việc DEV không còn thời gian làm User Story bảo mật dữ liệu khách hàng. Hiện tượng này trong Quản lý Dự án gọi là gì và cách phòng chống là gì?
* **A.** Gọi là **Kaizen (Cải tiến liên tục)**, cần tuyên dương DEV vì sự sáng tạo vượt mong đợi.
* **B.** Gọi là **Gold Plating (Mạ vàng tính năng)** — một dạng lãng phí và làm lệch phạm vi nội bộ rất nguy hiểm. Để phòng chống, PM/SM và PO phải quán triệt nguyên tắc: Developers chỉ xây dựng những gì phục vụ cho **Sprint Goal** và thỏa mãn **Acceptance Criteria** đã thống nhất; mọi ý tưởng sáng tạo thêm đều rất đáng quý nhưng phải được đề xuất với PO để đưa vào Product Backlog đánh giá ưu tiên, không tự ý làm khi chưa hoàn thành các hạng mục *Must-have*.
* **C.** Gọi là **Refactoring (Tái cấu trúc mã nguồn)**, hoàn toàn hợp lệ trong Agile.
* **D.** Gọi là **Technical Debt (Nợ kỹ thuật)**.

> **Đáp án đúng:** **B**  
> **Giải thích nguyên lý:** Phân biệt rõ: **Refactoring** là làm sạch cấu trúc code bên trong mà không làm thay đổi hành vi bên ngoài để dễ bảo trì (được khuyến khích). Ngược lại, **Gold Plating** là tự ý đắp thêm các tính năng/hiệu ứng ngoài yêu cầu của PO mà không qua đánh giá giá trị - chi phí, gây trễ các mục tiêu cốt lõi.

---

**Câu 23 [Bẫy Quản lý Nợ kỹ thuật - Technical Debt]:** Do áp lực thời gian, ở những ngày đầu đội đã viết cứng (hard-code) một số cấu hình Prompt và gộp chung toàn bộ logic xử lý vào một file code duy nhất dài 3.000 dòng, khiến việc sửa đổi hoặc thêm công cụ mới (Tools) cho AI Agent ở Sprint 2 ngày càng chậm và dễ phát sinh lỗi dây chuyền. Trong thuật ngữ Agile, tình trạng này gọi là gì và cách xử lý đúng là gì?
* **A.** Gọi là **Technical Debt (Nợ kỹ thuật)**. Nếu không trả nợ sớm, "lãi suất" (thời gian phải bỏ thêm cho mỗi tính năng mới) sẽ ngày càng tăng và làm giảm **Velocity** thực tế của đội. Cách xử lý đúng: Minh bạch hóa Technical Debt với PO, dành một phần dung lượng trong mỗi Sprint để **Refactor** dần các module đang cần mở rộng, và siết chặt tiêu chuẩn Code Review trong **Definition of Done (DoD)**.
* **B.** Gọi là **Sunk Cost (Chi phí chìm)**, không cần quan tâm vì code miễn chạy được là xong.
* **C.** Đội nên dừng toàn bộ việc phát triển tính năng nghiệp vụ trong 3 Sprint liên tiếp chỉ để ngồi viết lại code cho đẹp (Refactoring Sprint).
* **D.** Đổ lỗi toàn bộ cho BA vì viết tài liệu không rõ.

> **Đáp án đúng:** **A**  
> **Giải thích nguyên lý:** **Technical Debt** nếu tích tụ sẽ kéo tụt Velocity về lâu dài. Tuy nhiên, Agile **không khuyến khích** tạo ra một "Refactoring Sprint" (dừng hoàn toàn việc tạo giá trị nghiệp vụ trong cả Sprint chỉ để sửa code - loại C), vì mỗi Sprint đều phải tạo ra ít nhất một **Usable Increment** mang lại giá trị kinh doanh. Thay vào đó, việc trả nợ kỹ thuật và Refactoring phải được lồng ghép liên tục vào từng Sprint và vào chuẩn **DoD**.

---

**Câu 24 [Bẫy Ưu tiên hóa Backlog bằng RICE]:** Product Owner đang cân nhắc giữa hai tính năng AI cho Sprint tiếp theo và chỉ đủ nguồn lực chọn **1 tính năng**:
* **Tính năng X (AI Tư vấn Mở thẻ & So sánh ưu đãi tự động):** Tiếp cận (Reach) = `1.000` khách/ngày; Tác động (Impact) = `2` (High); Độ tự tin kỹ thuật (Confidence) = `90%` (`0.9`); Công sức thực hiện (Effort) = `3` Person-Days.
* **Tính năng Y (AI Dự báo biến động tỷ giá ngoại tệ bằng Deep Learning tự huấn luyện):** Tiếp cận (Reach) = `400` khách/ngày; Tác động (Impact) = `3` (Massive); Độ tự tin kỹ thuật (Confidence) = `50%` (`0.5`); Công sức thực hiện (Effort) = `6` Person-Days.
Dựa theo công thức **RICE Score**, điểm số của X và Y lần lượt là bao nhiêu và PO nên chọn tính năng nào?
* **A.** $\text{RICE}(X) = 600$; $\text{RICE}(Y) = 100$ $\rightarrow$ Chọn **Tính năng X**.
* **B.** $\text{RICE}(X) = 100$; $\text{RICE}(Y) = 600$ $\rightarrow$ Chọn **Tính năng Y**.
* **C.** $\text{RICE}(X) = 1.800$; $\text{RICE}(Y) = 1.200$ $\rightarrow$ Chọn **Tính năng Y** vì có Impact bằng 3.
* **D.** Hai tính năng có điểm RICE bằng nhau là `300`.

> **Đáp án đúng:** **A**  
> **Giải thích nguyên lý:** Áp dụng công thức $\text{RICE} = \frac{\text{Reach} \times \text{Impact} \times \text{Confidence}}{\text{Effort}}$:
> * $\text{RICE}(X) = \frac{1000 \times 2 \times 0.9}{3} = \frac{1800}{3} = \mathbf{600}$.
> * $\text{RICE}(Y) = \frac{400 \times 3 \times 0.5}{6} = \frac{600}{6} = \mathbf{100}$.
> **Tính năng X** có điểm RICE cao gấp 6 lần Tính năng Y (một **Quick Win** điển hình: tệp người dùng lớn, độ tự tin kỹ thuật cao, tốn ít thời gian triển khai), do đó PO chắc chắn phải ưu tiên chọn **Tính năng X**.

---

**Câu 25 [Bẫy Đặc thù Quản lý Chất lượng Dự án AI Agent / LLM]:** Khác với phần mềm truyền thống (Deterministic Software — nơi `1 + 1` luôn bằng `2`), hệ thống **AI Agent sử dụng LLM** có tính chất xác suất (Probabilistic / Non-deterministic — cùng một câu hỏi nhưng mỗi lần gọi có thể sinh ra câu chữ hơi khác nhau hoặc tiềm ẩn nguy cơ bịa đặt thông tin **Hallucination**). Với vai trò là PM và QA trong một dự án Agile xây dựng AI Agent cho ngân hàng, phương pháp quản lý chất lượng nào sau đây là PHÙ HỢP NHẤT để đưa vào **Definition of Done (DoD)**?
* **A.** Chỉ cần DEV test thử bằng tay 2 câu hỏi trên máy cá nhân thấy AI trả lời trôi chảy là được phép đánh dấu "Done".
* **B.** Bắt buộc AI phải trả lời giống hệt từng dấu chấm, dấu phẩy (Exact String Match 100%) như câu mẫu cố định, nếu lệch 1 từ cũng đánh Fail.
* **C.** Xây dựng một **Golden Evaluation Dataset** (Bộ dữ liệu kiểm thử chuẩn gồm ví dụ 50–100 kịch bản câu hỏi thực tế của khách hàng VPBank: câu hỏi thường gặp, câu hỏi bẫy ngoài phạm vi, câu hỏi chứa thông tin nhạy cảm/tấn công Prompt Injection) và đánh giá tự động/bán tự động theo bộ chỉ số ngưỡng chất lượng (Quality Thresholds): **Groundedness / Faithfulness** (Độ trung thực dựa trên tài liệu ngân hàng, $0\%$ Hallucination về con số lãi suất/biểu phí), **Answer Relevance** ($\ge 85\%$), **Guardrail Pass Rate** ($100\%$ chặn được câu hỏi độc hại/rò rỉ PII) và **Latency** (Thời gian phản hồi $< 3\text{s}$).
* **D.** Vì AI có tính xác suất nên QA không cần kiểm thử nữa, giao thẳng cho khách hàng tự dùng và tự chịu trách nhiệm.

> **Đáp án đúng:** **C**  
> **Giải thích nguyên lý:** Trong quản lý dự án AI (AI Product Management & GenAI QA), ta không thể kiểm thử bằng cách so khớp chuỗi tuyệt đối 100% (*Exact String Match* - loại B) và càng không thể chỉ test mò vài câu (*Vibe check* - loại A). Chuẩn mực hiện đại là **Eval-Driven Development (Phát triển hướng đánh giá)**: BA và QA phối hợp thiết lập bộ **Golden Evaluation Dataset** kèm các ngưỡng đo lường (**Faithfulness/No Hallucination, Relevance, Safety Guardrails, Latency**) ngay trong **Definition of Done (DoD)**.

---

## PHẦN 5: BỘ TEMPLATE THỰC CHIẾN CHO TEAM HACK4BIZ (VÒNG 2 & VÒNG 3)

> Các bảng biểu dưới đây được thiết kế chuẩn hóa cho đội hình **5 thành viên (PM, PO, BA, DEV, QA)** để bạn có thể copy trực tiếp sang Notion / Confluence / Jira / Markdown của nhóm khi bước vào Vòng 2 và Vòng 3.

---

### 5.1. Mẫu Kế hoạch 2 Sprint cho Vòng 2 (16 Ngày Build MVP AI Agent)

**Cấu trúc Chu kỳ (Cadence):**
* **Ngày 1 (Day 1):** *Sprint 0 / Inception & Architecture Foundation* (Khởi tạo dự án, chốt Product Goal, kiến trúc RAG/Agent, DoR, DoD và Product Backlog).
* **Ngày 2 – Ngày 8 (7 ngày):** **SPRINT 1 — "Core Engine & Happy Path MVP"** (Mục tiêu: AI Agent chạy thông suốt luồng nghiệp vụ cốt lõi số 1 với dữ liệu thật của VPBank trên môi trường Staging).
* **Ngày 9 – Ngày 15 (7 ngày):** **SPRINT 2 — "Agentic Actions, Guardrails & UX Polish"** (Mục tiêu: Hoàn thiện tính năng tự động thực thi tác vụ/Tool Calling, lớp bảo mật chống Hallucination/PII, tối ưu độ trễ và hoàn tất bộ hồ sơ thuyết trình/Video Demo).
* **Ngày 16 (Day 16):** *Final Hardening, Rehearsal & Submission* (Đóng băng code, tổng duyệt Pitching và nộp bài trước hạn chót ít nhất 3 giờ).

```text
LỘ TRÌNH 16 NGÀY VÒNG 2 (MASTER TIMELINE & CRITICAL MILESTONES)
[D1: Sprint 0] ==> [D2 ........ D8: SPRINT 1 (7 Ngày)] ==> [D9 ........ D15: SPRINT 2 (7 Ngày)] ==> [D16: Submit]
  ^                  ^               ^        ^              ^                ^        ^              ^
  Chốt Charter,      Planning S1     Code     Review &       Planning S2      Code     Review S2      Pitching
  DoR/DoD, Backlog   (Sáng D2)       Freeze   Retro S1       (Sáng D9)        Freeze   & Quay Demo    Rehearsal
                                     (Tối D7) (Chiều D8)                      (Tối D14)(Chiều D15)    & Nộp bài
```

#### Bảng Phân bổ Mục tiêu & Đầu ra Từng Ngày cho 5 Vị trí (16-Day Actionable Matrix)

| Giai đoạn / Ngày | Mục tiêu Trọng tâm (Daily Milestone) | PM (kiêm Scrum Master) | Product Owner (PO) | Business Analyst (BA) | Developer (DEV - AI & Fullstack) | Quality Assurance (QA) |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **Ngày 1**<br>*(Sprint 0 - Khởi tạo)* | **Chốt Product Vision, Kiến trúc & Product Backlog** | Lập Project Charter, bảng Kanban/Jira, Risk Register, thống nhất DoR & DoD với cả đội. | Xác định **Product Goal**, chân dung khách hàng VPBank, ưu tiên hóa Backlog theo **MoSCoW**. | Phân tích đề bài, vẽ sơ đồ luồng nghiệp vụ tổng thể (BPMN), viết chi tiết 5–6 User Stories đầu tiên đạt **DoR**. | Khảo sát Tech Stack (LLM API, Vector DB, Backend/UI), dựng Git Repo, CI/CD & chạy thử "Hello World" LLM. | Thiết lập Test Strategy, quy trình log Bug và khung **Golden Evaluation Dataset** để chấm điểm AI. |
| **Ngày 2**<br>*(Sprint 1 - Ngày 1)* | **Sprint 1 Planning & Chốt API Contract / Dữ liệu lõi** | Điều phối **Sprint 1 Planning** (Timebox 1.5h) và phiên **Planning Poker**; chốt **Sprint 1 Goal**. | Trình bày Sprint 1 Goal & các PBIs ưu tiên cao nhất (Must-have); giải đáp thắc mắc giá trị nghiệp vụ. | Thu thập & làm sạch bộ tài liệu tri thức VPBank (biểu phí, chính sách thẻ/vay), bàn giao API Contract cùng DEV. | Thiết kế kiến trúc dữ liệu, dựng Pipeline Ingestion (Chunking & Embedding vào Vector DB), dựng khung UI Chat cơ bản. | Viết Test Cases (Given-When-Then) cho các Stories của Sprint 1; tạo 30 câu hỏi kiểm thử RAG đầu tiên. |
| **Ngày 3 – 4**<br>*(Sprint 1 - Ngày 2, 3)* | **Xây dựng Luồng RAG & Hội thoại Nghiệp vụ số 1** | Chủ trì **Daily Scrum** (15p/ngày), cập nhật Burndown Chart, kiểm soát WIP, gỡ bỏ rào cản tài nguyên/API. | Kiểm tra sớm (Early feedback) các câu trả lời mẫu của AI; chuẩn bị định hướng cho buổi gặp Mentor. | Đặc tả chi tiết System Prompt, cấu trúc đầu ra JSON của AI; bắt đầu chuẩn bị User Stories cho Sprint 2. | Code hoàn chỉnh luồng **RAG Retrieval + Prompt Engineering** cho tính năng cốt lõi số 1; kết nối Backend API với giao diện Chat. | Thực hiện **Shift-left Testing**: review Prompt và test ngay API RAG trên Postman khi DEV vừa code xong từng phần. |
| **Ngày 5 – 6**<br>*(Sprint 1 - Ngày 4, 5)* | **Tích hợp End-to-End Luồng 1 & Backlog Refinement** | Theo dõi CFD để chống nghẽn cổ chai ở cuối Sprint; điều phối buổi **Backlog Refinement** (1h) cho Sprint 2. | Chủ trì buổi Refinement cùng đội cho các Stories của Sprint 2; rà soát giá trị kinh doanh đạt được. | Tinh chỉnh luồng xử lý ngoại lệ (Fallback khi AI không biết câu trả lời); hoàn tất đặc tả các Stories Sprint 2 đạt DoR. | Hoàn thiện tích hợp UI + Backend + AI của Sprint 1; viết Unit Test và sửa ngay các lỗi do QA phát hiện. | Chạy kiểm thử tích hợp (Integration Test) và chấm điểm độ chính xác của AI trên bộ 30 câu hỏi chuẩn. |
| **Ngày 7**<br>*(Sprint 1 - Ngày 6)* | **Code Freeze Sprint 1 & Kiểm thử Hồi quy** | Giám sát mốc **Code Freeze Sprint 1** lúc 18h00; đảm bảo 100% các Stories đạt chuẩn **DoD**. | Nghiệm thu sớm (UAT) từng Story đã được QA đánh dấu Pass trên môi trường Staging. | Rà soát tính nhất quán giữa tài liệu đặc tả (BRD/SRS) và hành vi thực tế của sản phẩm trên Staging. | Fix dứt điểm toàn bộ Bug mức Critical/High của Sprint 1; deploy bản ổn định lên Staging. | Chạy Regression Test và xác nhận các Stories đạt 100% **Definition of Done (DoD)**. |
| **Ngày 8**<br>*(Sprint 1 - Ngày 7)* | **Sprint 1 Review (với Mentor) & Retrospective** | Điều phối **Sprint 1 Review** (1h) và **Sprint 1 Retrospective** (45p); chốt Action Items cải tiến cho Sprint 2. | Trình diễn **Usable Increment 1** với Mentor/Stakeholders, thu thập phản hồi để cập nhật Product Backlog. | Ghi nhận các góp ý nghiệp vụ từ Mentor để cập nhật vào Acceptance Criteria của các Stories Sprint 2. | Tham gia Demo kỹ thuật tại Sprint Review; đề xuất cải tiến kỹ thuật/tối ưu tốc độ phản hồi trong buổi Retro. | Báo cáo chỉ số chất lượng Sprint 1 (Tỷ lệ AI trả lời đúng, Latency trung bình, số Bug đã đóng) trong buổi Review & Retro. |
| **Ngày 9**<br>*(Sprint 2 - Ngày 1)* | **Sprint 2 Planning & Khởi động Agentic Tool Calling** | Điều phối **Sprint 2 Planning** dựa trên Velocity thực tế của Sprint 1; cập nhật Risk Register. | Chốt **Sprint 2 Goal** (tập trung vào tính năng tạo sự khác biệt — Differentiators & Bảo mật ngân hàng). | Đặc tả luồng **Agentic Tool Calling / Function Calling** (ví dụ: AI tự động tra cứu trạng thái giao dịch / tạo phiếu yêu cầu). | Bắt đầu code các **Tools / Functions** cho AI Agent và cơ chế quản lý trạng thái hội thoại nhiều bước (Multi-turn Memory). | Mở rộng bộ **Golden Evaluation Dataset** lên 60–80 kịch bản (bổ sung kịch bản tấn công Prompt Injection & PII). |
| **Ngày 10 – 12**<br>*(Sprint 2 - Ngày 2, 3, 4)* | **Hoàn thiện Agentic Workflow, Guardrails & Giao diện** | Giữ nhịp Daily Scrum, kiểm soát chặt **Scope Creep / Gold Plating**; nhắc mốc đường găng (Critical Path). | Bắt đầu xây dựng cốt truyện kinh doanh (Business Storytelling), tính toán chỉ số ROI / Cost Saving cho VPBank. | Đồng bộ hóa toàn bộ tài liệu thiết kế hệ thống (Architecture, Erd, Sequence Diagrams, Prompt Catalog) để đưa vào hồ sơ nộp. | Tích hợp **Guardrails** (chống Hallucination, che thông tin thẻ/CCCD - PII Masking), tối ưu Latency ($< 3\text{s}$), hoàn thiện UX/UI. | Kiểm thử liên tục (Continuous Testing) các tính năng Agentic, thực hiện **Red-Teaming** (đóng vai hacker thử bẻ khóa Prompt của AI). |
| **Ngày 13 – 14**<br>*(Sprint 2 - Ngày 5, 6)* | **Ổn định toàn hệ thống & Chuẩn bị Kịch bản Demo** | Đóng băng phạm vi tính năng (**Feature Freeze**); điều phối luồng khớp nối giữa bản Demo sống và Slide thuyết trình. | Hoàn thiện **Pitching Deck** (Bài toán $\rightarrow$ Giải pháp AI $\rightarrow$ Giá trị kinh doanh $\rightarrow$ Lộ trình triển khai thực tế tại VPBank). | Viết **Kịch bản Demo trực tiếp (Live Demo Script)** từng bước khớp với dữ liệu mẫu "đẹp" và sát thực tế ngân hàng nhất. | Tối ưu hiệu năng, cấu hình **Semantic Cache / Fallback Model** cho các kịch bản Demo trọng tâm; fix toàn bộ Bug tồn đọng. | Chạy **Full System & Performance Test**; xác nhận toàn bộ MVP đạt 100% DoD; chuẩn bị sẵn dữ liệu sạch cho buổi quay Demo. |
| **Ngày 15**<br>*(Sprint 2 - Ngày 7)* | **Sprint 2 Review, Retrospective & Quay Video Demo dự phòng** | Chủ trì **Sprint 2 Review & Retro**; kiểm tra chéo toàn bộ danh mục hồ sơ nộp theo đúng quy chế Ban Tổ chức. | Duyệt lần cuối toàn bộ sản phẩm MVP, Slide Pitching và Video Demo. | Hoàn tất đóng gói bộ tài liệu Nghiệp vụ & Kỹ thuật (BRD/System Design) dạng PDF chuyên nghiệp. | Đóng băng code (**Hard Code Freeze**), giữ nguyên trạng thái Server Staging ổn định, hỗ trợ quay **Backup Demo Video**. | Kiểm tra lần cuối đường link Staging trên nhiều trình duyệt/thiết bị khác nhau; xác nhận Video Demo rõ nét, không lỗi. |
| **Ngày 16**<br>*(Ngày Nộp bài)* | **Tổng duyệt Pitching (Dry-run) & Nộp bài chính thức** | Bấm giờ cho 2 lượt **Dry-run Pitching & Q&A**; trực tiếp nộp bài lên hệ thống **trước Deadline tối thiểu 3 giờ** (phòng nghẽn mạng). | Luyện tập thuyết trình và phản biện các câu hỏi hóc búa về bài toán kinh doanh & ROI của ngân hàng. | Chuẩn bị bộ câu trả lời Q&A chi tiết về quy trình nghiệp vụ và tính tuân thủ pháp lý ngân hàng. | Trực kỹ thuật đảm bảo Server Staging & API Key còn dư hạn mức (Quota) để Ban Giám khảo vào chấm thử bất cứ lúc nào. | Chuẩn bị bộ số liệu thực nghiệm (Accuracy %, Latency, Security Test Report) để chứng minh chất lượng sản phẩm khi Giám khảo hỏi. |

---

### 5.2. Mẫu Risk Register Đặc thù cho Dự án AI Agent Ngân hàng (VPBank)

Bảng quản trị rủi ro này đã được thiết lập sẵn **8 rủi ro sống còn** trong các cuộc thi phát triển AI Agent ngành Tài chính – Ngân hàng, đánh giá theo thang điểm $1 - 5$ ($\text{Severity} = P \times I$):

| Mã RR | Tên Rủi ro & Mô tả Kịch bản (Risk Description) | Nhóm | Xác suất ($P$: 1-5) | Tác động ($I$: 1-5) | Điểm ($P \times I$) | Chiến lược | Dấu hiệu Cảnh báo sớm (Risk Trigger) | Phương án Phòng ngừa chủ động (Mitigation Plan) | Kế hoạch Dự phòng khi sự cố xảy ra (Contingency Plan) | Người phụ trách (Owner) |
| :---: | :--- | :---: | :---: | :---: | :---: | :---: | :--- | :--- | :--- | :---: |
| **RR-01** | **AI Hallucination (Bịa đặt thông tin tài chính):** AI tự suy diễn sai lãi suất, biểu phí hoặc điều kiện mở thẻ của VPBank, gây rủi ro pháp lý và mất điểm nghiêm trọng trước Giám khảo. | AI / Nghiệp vụ | 4 | 5 | **20 (High)** | **Mitigate** | Kết quả test bộ Golden Dataset có tỷ lệ câu trả lời sai lệch tài liệu gốc $> 5\%$. | 1. Hạ `temperature = 0.0 - 0.2`.<br>2. Áp dụng **Strict RAG Prompting**: Bắt buộc AI chỉ trả lời dựa trên Context truy xuất được và phải đính kèm trích dẫn nguồn (**Citation**).<br>3. Nếu điểm tương đồng (Similarity Score) $< 0.75$, bắt buộc kích hoạt câu trả lời từ chối an toàn. | Kích hoạt bộ lọc hậu kiểm (Post-processing Regex/Rule check) đối với các con số lãi suất/biểu phí quan trọng trước khi hiển thị lên màn hình khách hàng. | **DEV + QA** |
| **RR-02** | **Rò rỉ Dữ liệu Nhạy cảm (PII Leakage) & Prompt Injection:** Người dùng dùng câu lệnh bẻ khóa (Jailbreak) hoặc AI vô tình gửi số thẻ đầy đủ, CCCD, số dư thật lên LLM bên thứ 3. | Bảo mật Ngân hàng | 3 | 5 | **15 (High)** | **Avoid & Mitigate** | QA vượt qua được hàng rào System Prompt trong phiên Red-Teaming. | 1. Xây dựng lớp **PII Masking Middleware** ẩn danh hóa số thẻ (`4553-****-****-1234`), CCCD, SĐT trước khi gửi dữ liệu lên LLM API.<br>2. Thiết lập **Input/Output Guardrails** chặn các mẫu câu Prompt Injection / Jailbreak. | Ngắt luồng hội thoại AI ngay lập tức khi phát hiện truy vấn xâm nhập trái phép, ghi log cảnh báo bảo mật và chuyển hướng khách hàng về kênh xác thực truyền thống hoặc tổng đài viên. | **DEV + BA** |
| **RR-03** | **Độ trễ phản hồi cao (High Latency) hoặc Đứt kết nối / Hết Quota API LLM lúc Demo:** LLM phản hồi $> 10\text{s}$ hoặc báo lỗi `429 Rate Limit` ngay khi Giám khảo đang chấm trực tiếp. | Kỹ thuật / Hạ tầng | 4 | 4 | **16 (High)** | **Mitigate** | Thời gian phản hồi trung bình lúc test $> 4\text{s}$ hoặc lượng token tiêu thụ đạt $70\%$ hạn mức. | 1. Sử dụng cơ chế **Streaming Response (SSE)** để chữ hiện ra tức thì sau $< 1\text{s}$.<br>2. Chuẩn bị ít nhất **3 API Keys** từ các tài khoản/nhà cung cấp khác nhau.<br>3. Cài đặt **Semantic Caching** cho các kịch bản Demo cốt lõi. | Hệ thống tự động **Auto-Fallback** chuyển sang API Key dự phòng hoặc model nhẹ hơn trong vòng $2\text{ giây}$; đồng thời luôn mở sẵn tab **Video Demo chất lượng cao** đã quay sẵn. | **DEV + PM** |
| **RR-04** | **AI tự ý thực thi hành động nhạy cảm sai lệch (Uncontrolled Agentic Action):** AI hiểu nhầm ý khách hàng và tự gọi hàm khóa thẻ vĩnh viễn hoặc tạo giao dịch sai. | Nghiệp vụ / Kiến trúc | 3 | 5 | **15 (High)** | **Avoid** | AI tự động gọi Tool/API có tính chất ghi/thay đổi dữ liệu (Write/Mutate) mà không hỏi lại. | Áp dụng thiết kế **Human-in-the-Loop (HITL)**: Đối với mọi tác vụ thay đổi trạng thái (Khóa thẻ, Đăng ký vay, Khiếu nại), AI chỉ tạo **Confirmation Card (Thẻ xác nhận)** trên UI, bắt buộc người dùng bấm nút xác nhận + nhập OTP. | Thu hồi quyền gọi trực tiếp các API ghi dữ liệu từ tầng LLM, chuyển toàn bộ quyền kích hoạt cuối cùng về sự kiện click nút cứng trên giao diện Frontend. | **PO + DEV** |
| **RR-05** | **Lệch pha giữa Tài liệu Nghiệp vụ (BRD/Deck) và Code thực tế (Doc-Code Drift):** Lúc thuyết trình Slide nói một đằng nhưng khi mở web Demo thì giao diện và luồng chạy một nẻo. | Quy trình / Giao tiếp | 4 | 3 | **12 (Med)** | **Mitigate** | DEV tự ý sửa luồng trên code mà không báo BA, hoặc BA sửa tài liệu không báo DEV. | 1. Đưa tiêu chí *"Cập nhật đồng bộ tài liệu API/Luồng nghiệp vụ"* vào **Definition of Done (DoD)**.<br>2. Áp dụng phiên **Three Amigos (BA-DEV-QA)** ngắn mỗi khi có điều chỉnh luồng. | Dành 4 giờ chiều Ngày 14 để BA, PO và DEV ngồi khớp từng màn hình trên Staging với từng trang trên Slide Pitching. | **BA + PM** |
| **RR-06** | **Scope Creep & Gold Plating làm vỡ tiến độ (Bệnh "Ôm đồm tính năng"):** Đội cố nhồi nhét 10 tính năng AI phức tạp nhưng không có tính năng nào chạy ổn định trọn vẹn. | Quản trị Dự án | 4 | 4 | **16 (High)** | **Avoid & Mitigate** | Đường Sprint Burndown đi ngang đến Ngày thứ 5 của Sprint mà chưa có Story nào đạt DoD. | 1. PM và PO kiên quyết áp dụng **MoSCoW**: Tập trung hoàn thành $100\%$ nhóm **Must-have** ở Sprint 1.<br>2. Mọi tính năng mới phát sinh phải qua quy trình Trade-off. | Kích hoạt phương án **De-scoping (Cắt giảm phạm vi)** ngay ở Ngày 12: Cắt bỏ hoàn toàn các tính năng *Could-have*, ẩn các nút chưa hoàn thiện trên UI để bản MVP gọn và mượt tuyệt đối. | **PM + PO** |
| **RR-07** | **Nghẽn cổ chai ở khâu Kiểm thử phút chót (QA Bottleneck):** DEV dồn code đến sát ngày nộp bài mới đẩy sang khiến QA không kịp test, sản phẩm đầy lỗi vặt khi trình diễn. | Quy trình Scrum | 3 | 4 | **12 (Med)** | **Mitigate** | Trên biểu đồ CFD, số lượng ticket ở cột *In Progress* vượt quá 3 nhưng cột *In Testing* bằng 0 trong 3 ngày đầu. | 1. Chia nhỏ User Story (tối đa $1 - 2$ ngày/Story).<br>2. Đặt **WIP Limit = 2** cho cột DEV.<br>3. Áp dụng **Code Freeze** trước thời điểm kết thúc Sprint ít nhất $18 - 24$ giờ. | Kích hoạt **Team Swarming**: Toàn bộ PM, PO, BA cùng nhảy vào thực hiện Exploratory Testing theo checklist của QA, trong khi DEV chỉ tập trung fix bug Critical. | **PM + QA** |
| **RR-08** | **Kiệt sức & Xung đột nội bộ trong 32h Hackathon (Team Burnout & Conflict):** Các thành viên thiếu ngủ dẫn đến cáu gắt, code nhầm nhánh Git hoặc xóa nhầm dữ liệu sát giờ G. | Nhân sự / Vận hành | 3 | 4 | **12 (Med)** | **Mitigate** | Thành viên thức trắng quá 20 giờ liên tục, bắt đầu xuất hiện tranh cãi gay gắt hoặc commit code lỗi liên tiếp. | 1. PM lập lịch **luân phiên nghỉ ngơi (Rotating Power Naps 2-3h)** giữa các thành viên.<br>2. Bắt buộc bảo vệ nhánh `main` trên Git (chỉ merge qua Pull Request đã test). | PM can thiệp hạ nhiệt ngay lập tức, cho thành viên đang quá tải nghỉ 90 phút; sử dụng bản Git Tag ổn định gần nhất nếu nhánh hiện tại bị lỗi nặng trước giờ nộp 2 tiếng. | **PM** |

---

### 5.3. Checklist & Quy trình 5 Bước Xử lý Change Request (CR) trong 32h Hackathon (Vòng 3)

Trong Vòng 3 (32 giờ Hackathon liên tục), Ban Tổ chức / Giám khảo VPBank sẽ tung ra các **Change Requests (CR)** bất ngờ nhằm kiểm tra khả năng **Thích ứng (Adaptation)**, tư duy ưu tiên hóa của PO/PM và độ linh hoạt trong kiến trúc phần mềm của đội.

```text
QUY TRÌNH 5 BƯỚC XỬ LÝ CHANGE REQUEST TRONG 32H HACKATHON (TIMEBOXED PIPELINE)

 [BƯỚC 1: TIẾP NHẬN & GIẢI MÃ CR]  (T+0h -> T+1h: Timebox 60 phút)
   PO + BA + PM bóc tách đề bài CR, phân loại mức độ bắt buộc & tiêu chí chấm điểm
                                  |
                                  v
 [BƯỚC 2: ĐÁNH GIÁ TÁC ĐỘNG KỸ THUẬT & NGHIỆP VỤ] (T+1h -> T+2.5h: Timebox 90 phút)
   Three Amigos (BA + DEV + QA) đánh giá kiến trúc, DB, API, Prompt & ước lượng SP
                                  |
                                  v
 [BƯỚC 3: TÁI CẤU TRÚC & CHỐT SPRINT BACKLOG] (T+2.5h -> T+3.5h: Timebox 60 phút)
   PO + PM áp dụng MoSCoW / Trade-off, cắt bỏ việc phụ, khóa Mini-Sprint Goal mới
                                  |
                                  v
 [BƯỚC 4: THỰC THI TỐC ĐỘ CAO & KIỂM THỬ SONG SONG] (T+3.5h -> T+26h: ~22.5 giờ)
   Chia 2 Mini-Sprints (11h/kỳ), Standup mỗi 4h, DEV code + QA Shift-left Test liên tục
                                  |
                                  v
 [BƯỚC 5: CODE FREEZE, ĐÓNG GÓI & TỔNG DUYỆT PITCHING] (T+26h -> T+32h: 6 giờ cuối)
   T+26h Soft Freeze -> T+28h Hard Code Freeze -> Cập nhật Slide/Video -> Nộp bài T+30.5h
```

#### Checklist Hành động Chi tiết theo 5 Bước (Copy để tick trực tiếp trong 32h Vòng 3)

##### BƯỚC 1: Tiếp nhận & Giải mã Đề bài Change Request (T+00:00 $\rightarrow$ T+01:00 | Timebox: 60 phút)
* [ ] **[PM]:** Giữ bình tĩnh cho toàn đội; yêu cầu DEV **không** vội vàng nhảy vào sửa code ngay khi chưa hiểu hết bức tranh tổng thể của CR.
* [ ] **[PO + BA]:** Đọc kỹ văn bản CR từ Ban Tổ chức, gạch chân các từ khóa yêu cầu và xác định chính xác: **Đâu là yêu cầu cốt lõi bắt buộc (Core Requirement)** chiếm nhiều điểm chấm nhất?
* [ ] **[PO + BA]:** Chuẩn bị danh sách câu hỏi làm rõ (Clarification Questions) để hỏi ngay Mentor / Ban Tổ chức trong khung giờ Q&A đầu tiên (tránh hiểu sai đề dẫn đến làm lạc hướng).
* [ ] **[BA]:** Tóm tắt CR thành 1 trang **CR Brief** gồm: *Bối cảnh thay đổi $\rightarrow$ Danh sách các tính năng mới/sửa đổi $\rightarrow$ Tiêu chí nghiệm thu (Acceptance Criteria) kỳ vọng của Ban Giám khảo*.

##### BƯỚC 2: Đánh giá Tác động Kỹ thuật & Nghiệp vụ - Impact Analysis (T+01:00 $\rightarrow$ T+02:30 | Timebox: 90 phút)
* [ ] **[BA + DEV + QA (Three Amigos)]:** Rà soát xem CR tác động vào tầng nào của hệ thống MVP hiện tại:
  * [ ] *Tầng Giao diện (UI/UX):* Có cần thêm màn hình mới hay chỉ cần thêm Component/Card ngay trên khung Chat hiện có? *(Ưu tiên tận dụng khung Chat/Adaptive Card để tiết kiệm thời gian code UI!).*
  * [ ] *Tầng AI / Prompt / RAG:* Có thể giải quyết bằng cách cập nhật System Prompt, nạp thêm tài liệu mới vào Vector DB và thêm 1–2 Function Calling (Tools) hay không?
  * [ ] *Tầng Backend / Database:* Có làm thay đổi Schema hiện tại hay gây lỗi dây chuyền (Breaking Changes) cho các tính năng cũ đang chạy tốt ở Vòng 2 không?
* [ ] **[DEV + BA + QA]:** Tách CR thành các User Stories nhỏ (mỗi Story chỉ nên tốn từ **2 đến 4 giờ** làm việc) và ước lượng nhanh điểm nỗ lực (**Story Points / Ideal Hours**).
* [ ] **[QA]:** Cảnh báo ngay các rủi ro hồi quy (Regression Risks) có thể làm hỏng luồng Demo cũ của Vòng 2.

##### BƯỚC 3: Tái cấu trúc & Chốt lại Sprint Backlog (T+02:30 $\rightarrow$ T+03:30 | Timebox: 60 phút)
* [ ] **[PO + PM]:** Tính toán ngân sách thời gian thực tế: Trong 32 giờ, trừ đi 3.5 giờ phân tích đầu kỳ, 6 giờ cuối cho Code Freeze/Pitching và 3.5 giờ nghỉ ngơi/ăn uống, nhóm chỉ còn đúng **~19 giờ lập trình thực tế (Net Coding Hours)**.
* [ ] **[PO]:** Áp dụng **MoSCoW** và ma trận **Value vs. Effort** cho các Stories của CR:
  * Chọn **100% mục Must-have** (Giải quyết trực diện đề bài CR với kiến trúc gọn nhất).
  * Chọn có chọn lọc mục **Should-have** (Tạo điểm nhấn thông minh của AI Agent).
  * Kiên quyết đưa các ý tưởng phức tạp tốn thời gian vào cột **Won't-have** hoặc dùng giải pháp **Mock / Wizard-of-Oz hợp lệ** cho các hệ thống tích hợp bên ngoài ngân hàng không nằm trong trọng tâm chấm điểm.
* [ ] **[PM]:** Thiết lập bảng Kanban 32h và khóa **Mini-Sprint Backlog** cùng với **Sprint Goal của Vòng 3**.

##### BƯỚC 4: Thực thi Tốc độ cao & Kiểm thử Song song (T+03:30 $\rightarrow$ T+26:00 | Thời lượng: 22.5 giờ)
* [ ] **[PM]:** Chia 22.5 giờ này thành **2 Mini-Sprints** (Mini-Sprint 3.1 từ `T+3.5h -> T+15h`; Mini-Sprint 3.2 từ `T+15h -> T+26h`) và tổ chức **Micro-Standup (5–10 phút) mỗi 4–6 giờ** để đồng bộ tiến độ.
* [ ] **[DEV]:** Tạo nhánh Git riêng cho CR (`feature/v3-change-request`), tuyệt đối **không** sửa trực tiếp trên nhánh `main` đang chứa bản MVP ổn định của Vòng 2 (để luôn có đường lui an toàn).
* [ ] **[BA + DEV]:** Ngay ở giờ thứ 4, chốt xong **Mock JSON / API Contract** của tính năng CR để Frontend, Backend/AI và QA chạy song song 3 luồng không chờ đợi nhau.
* [ ] **[QA]:** Thực hiện **Continuous Testing** — DEV vừa đẩy xong Story nào lên nhánh Staging sau mỗi 3–4 giờ là QA test ngay lập tức và báo bug tại chỗ (không viết ticket rườm rà, ngồi cạnh DEV chỉ trực tiếp để fix trong 15 phút).
* [ ] **[PO + BA]:** Song song với lúc DEV/QA hoàn thiện code từ giờ thứ 16 trở đi, bắt đầu cập nhật **Slide Pitching Vòng 3** (bổ sung phần: *"Cách đội ngũ tiếp nhận Change Request theo quy trình Agile Scrum và Kiến trúc mở rộng đáp ứng CR"* — Giám khảo cực kỳ đánh giá cao tư duy này!).
* [ ] **[PM]:** Điều phối lịch chợp mắt luân phiên (90–120 phút/người trong khung giờ từ 02:00 sáng đến 06:00 sáng) để giữ sự tỉnh táo cho ngày thuyết trình chung kết.

##### BƯỚC 5: Đóng băng Code (Code Freeze), Đóng gói & Tổng duyệt (T+26:00 $\rightarrow$ T+32:00 | 6 giờ cuối cùng)
* [ ] **Mốc T+26:00 (Còn 6 tiếng trước giờ hết hạn) — SOFT CODE FREEZE:**
  * [ ] **[PM]:** Tuyên bố ngừng toàn bộ việc code thêm tính năng mới.
  * [ ] **[QA + Toàn đội]:** Chạy **End-to-End Regression Test** cho cả luồng cũ (Vòng 2) kết hợp với luồng mới (CR Vòng 3) để đảm bảo CR mới không làm gãy tính năng cũ.
* [ ] **Mốc T+28:00 (Còn 4 tiếng trước giờ hết hạn) — HARD CODE FREEZE:**
  * [ ] **[DEV]:** Merge nhánh CR đã kiểm thử ổn định vào nhánh phát hành, gắn Git Tag `v3.0-final-release`, kiểm tra hạn mức API Key và giữ môi trường Staging ở trạng thái tĩnh hoàn toàn.
  * [ ] **[BA + PO + DEV]:** Quay ngay **1 Video Demo dự phòng (Backup Video 3–5 phút)** thể hiện trọn vẹn luồng xử lý Change Request mượt mà trên Staging.
* [ ] **Mốc T+29:00 $\rightarrow$ T+30:30 (90 phút Tổng duyệt Pitching):**
  * [ ] **[Toàn đội]:** Thực hiện 2 lượt **Dry-run Pitching** bấm giờ chuẩn xác từng phút.
  * [ ] **[PO + PM]:** Chuẩn bị sẵn 5 slide phụ lục (Appendix Slides) giải thích: *(1) Quy trình Agile Scrum & Burndown/Kanban thực tế của nhóm trong 16 ngày + 32h; (2) Cách nhóm phân tích & xử lý Change Request; (3) Kiến trúc chống Hallucination & Bảo mật PII; (4) Bài toán chi phí Token & ROI cho VPBank; (5) Bảng phân công RACI của 5 thành viên*.
* [ ] **Mốc T+30:30 (Trước hạn chót 90 phút) — NỘP BÀI CHÍNH THỨC (FINAL SUBMISSION):**
  * [ ] **[PM]:** Upload toàn bộ Source Code, Tài liệu, Slide Pitching, Link Staging và Backup Video lên cổng nộp bài của Ban Tổ chức; chụp màn hình xác nhận nộp thành công.
