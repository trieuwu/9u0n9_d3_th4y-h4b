# BIÊN BẢN HỌP NỘI BỘ — TEAM `</ProPTIT> Gương Dễ Thay` (HACK4BIZ 2026)

- **Tên đội thi:** `</ProPTIT> Gương Dễ Thay`
- **Ngày họp:** `18/11/2026` (`20:00 – 21:30`)
- **Hình thức:** Online Meeting (Discord)
- **Thành phần tham dự:** Đầy đủ 5 thành viên (`1 BA - NEU` + `4 Developers`)
- **Mục tiêu buổi họp:**
  1. Làm quen giữa các thành viên và thống nhất nguyên tắc phối hợp xuyên suốt 3 vòng thi.
  2. Nắm rõ cấu trúc cuộc thi **Hack4Biz 2026**, khung **Agile Scrum (3-5-3)** và phạm vi công việc của 5 Role (`PM`, `PO`, `BA`, `DEV`, `QA`).
  3. Chốt phân vai (Role) thi Vòng 1 (Online Assessment — `27/11/2026`).
  4. Chốt thông tin đăng ký dự thi, giờ check-in hàng tối và kế hoạch ôn tập Tuần 1 (`19/11 – 26/11/2026`).

---

## 1. NGUYÊN TẮC LÀM VIỆC CHUNG ĐÃ THỐNG NHẤT

- **Phản hồi tin nhắn:** Phản hồi trong vòng `2 tiếng` (khung giờ `08:00 – 23:00`). Sau `23:00` phản hồi trước `10:00` sáng hôm sau. Nếu bận đột xuất cần nhắn báo trước vào nhóm để cả đội chủ động điều phối.
- **Quỹ thời gian cam kết:** Dành `1.5 – 2 tiếng/ngày` từ `18/11` đến `27/11/2026` để nghiên cứu tài liệu và hoàn thành đầu việc được phân công.
- **Văn hóa trao đổi:** Chủ động hỏi ngay khi có phần chưa rõ; góp ý thẳng vào công việc trên tinh thần hỗ trợ lẫn nhau và tôn trọng chuẩn Definition of Done (DoD).
- **Khung giờ check-in tối hàng ngày (Daily Standup 10–15 phút):** `22:30`.
- **Kênh làm việc chính thức:**
  - **GitHub Repository:** [https://github.com/trieuwu/hack4biz](https://github.com/trieuwu/hack4biz)
  - **Notion Workspace (Tài liệu & Kanban Board):** Đã khởi tạo cho 5 thành viên
  - **Kênh họp trực tuyến:** Discord / Google Meet

---

## 2. TỔNG QUAN CUỘC THI & ĐỊNH HƯỚNG KỸ THUẬT

- **Đơn vị tổ chức & Bài toán:** BUV tổ chức, giải quyết bài toán thực tế khối Ngân hàng của **VPBank** bằng giải pháp **AI Agent**, vận hành theo quy trình **Agile Scrum**.
- **Lộ trình 3 Vòng thi:**
  - **Hạn đăng ký:** `22/11/2026` (Đội hoàn tất nộp hồ sơ sớm vào ngày `19/11/2026`).
  - **Vòng 1 – Online Assessment (`27/11/2026`):** Trắc nghiệm kiến thức chuyên môn từng Role + Agile Scrum (Lấy **Top 20** bước vào Vòng 2).
  - **Vòng 2 – MVP Building (`08/12 – 23/12/2026`):** Chia làm 2 Sprint (`7 ngày/Sprint`). Nộp bộ tài liệu phân tích nghiệp vụ (BRD, sơ đồ luồng) + Source Code **MVP AI Agent** chạy thực tế (Lấy **Top 4** vào Chung kết).
  - **Vòng 3 – 32h Hackathon (`09/01 – 10/01/2027`):** Thi Offline tại BUV (Ecopark), nhận **Change Request (CR)** trực tiếp từ Ban Tổ chức, phát triển tính năng bổ sung trên nền mã nguồn Vòng 2 và thuyết trình trước Ban Giám khảo.
- **Định hướng kỹ thuật cho 4 Developers (Chặng 2 sau 27/11):**
  - Áp dụng **Spec-Driven Development**: Viết đặc tả `specs.md` rõ ràng (API Contract, DB Schema, luồng dữ liệu) $\rightarrow$ Sử dụng công cụ AI hỗ trợ sinh code từng module nhỏ $\rightarrow$ Tự review chéo, kiểm thử cục bộ và quản lý nhánh qua Git Flow / Pull Request.
  - **Tech Stack dự kiến:** Python (`FastAPI`), `LangGraph` / `OpenAI Agents SDK` (`RAG`, `Tool/Function Calling`, `Guardrails`), Frontend `Next.js` hoặc `Chainlit / Streamlit`.

---

## 3. KẾT QUẢ CHỌN ROLE & CHIA VAI VÒNG 1

> *Lưu ý: Phân vai dưới đây dùng để đăng ký hồ sơ và làm bài thi đánh giá năng lực Vòng 1 (27/11). Sang Vòng 2 & Vòng 3, cả 4 thành viên kỹ thuật đều cùng tham gia thiết kế kiến trúc, lập trình và kiểm thử hệ thống AI Agent.*

| STT | Họ và Tên | Vai trò đăng ký Vòng 1 | Trọng tâm ôn luyện Vòng 1 | Ghi chú phân công |
| :---: | :--- | :---: | :--- | :--- |
| `01` | **Đặng Việt Anh** | **BA** | BABOK, BRD/SRS, User Story (INVEST), Acceptance Criteria, Use Case / BPMN | Phụ trách phân tích nghiệp vụ (NEU) |
| `02` | **Hà Tiến Triệu** | **PM** | Agile Scrum Guide 2020, Capacity, Velocity, Burndown/CFD, Risk & Change Management | Phụ trách điều phối dự án & Git |
| `03` | **Nguyễn Tú Anh** | **PO** | Product Vision, Backlog Ordering, MoSCoW, RICE, Problem vs. Solution, ROI | Phụ trách tối ưu giá trị sản phẩm |
| `04` | **Phùng Hải Đăng** | **DEV** | RESTful API, Backend Lifecycle, RAG vs. Function Calling, Resilience, AuthN/AuthZ | Phụ trách kiến trúc & AI Pipeline |
| `05` | **Đàm Thuận Khải** | **Tester (QA)** | ISO/IEC/IEEE 29119-3, ISTQB v4.0 Defect Lifecycle, Regression Test, AI Eval | Phụ trách kiểm thử & tiêu chuẩn DoD |

---

## 4. KẾ HOẠCH CÔNG VIỆC & ÔN TẬP TUẦN 1 (19/11 – 26/11/2026)

| Thời gian | Đầu việc cụ thể | Phụ trách | Kết quả đầu ra (Deliverables) | Trạng thái |
| :--- | :--- | :---: | :--- | :---: |
| **19/11 (Thứ 5)** | Nộp đơn đăng ký sớm (hạn 22/11) & khởi tạo Notion / GitHub / Discord | PM + Cả đội | Ảnh xác nhận nộp form thành công gửi vào nhóm | `[x]` |
| **20/11 – 21/11** | Ôn kỹ khung Agile Scrum (3 Accountabilities, 5 Events, 3 Artifacts, DoD) | Cả 5 người | Sơ đồ quy trình Scrum & tóm tắt lý thuyết cốt lõi | `[x]` |
| **22/11 – 23/11** | Biên soạn & chuẩn hóa Cẩm nang chuyên sâu theo từng Role (`PM`, `PO`, `BA`, `DEV`, `QA`) | Từng Role | Tài liệu cẩm nang (`docs/pm/pm_agile_scrum_handbook.md`) | `[x]` |
| **24/11 (Thứ 3)** | Tổng hợp bộ 30 câu hỏi trắc nghiệm chính thức & xây dựng Web Quiz luyện tập local | PM / DEV | Ứng dụng [`quiz/hack4biz_quiz.html`](../../quiz/hack4biz_quiz.html) & [`quiz/hack4biz_full_30.md`](../../quiz/hack4biz_full_30.md) | `[x]` |
| **25/11 (Tối T4)** | Làm thử toàn bộ đề trên Web Quiz local & họp chữa chéo các câu tình huống bẫy | Cả đội | Nắm chắc mảng chính & hiểu rõ ranh giới phối hợp 5 Roles | `[ ]` |
| **26/11 (Tối T5)** | Rà soát lần cuối các phần kiến thức còn hổng & kiểm tra thiết bị/đường truyền | Cả đội | Sẵn sàng 100% trước giờ thi Online Assessment ngày `27/11/2026` | `[ ]` |

---

## 5. CHECKLIST HÀNH ĐỘNG ĐÃ HOÀN TẤT & THEO DÕI TIẾP THEO

- [x] **1.** Hoàn tất bảng thông tin cá nhân và chốt 5 vị trí (`BA`, `PM`, `PO`, `DEV`, `QA`) của cả 5 thành viên.
- [x] **2.** Điền form đăng ký chính thức của Hack4Biz 2026 và lưu ảnh xác nhận.
- [x] **3.** Khởi tạo kho lưu trữ GitHub chuẩn hóa, bổ sung Cẩm nang Agile Scrum (`docs/pm/pm_agile_scrum_handbook.md`) và ứng dụng Web làm trắc nghiệm 30 câu tại local (`quiz/hack4biz_quiz.html`).
- [ ] **4.** Duy trì phiên check-in nhanh hàng tối lúc `22:30` để rà soát kết quả luyện đề cho tới ngày thi `27/11/2026`.
