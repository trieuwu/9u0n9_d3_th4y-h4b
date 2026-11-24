<div align="center">

# 🚀 Hack4Biz Competition 2026 — Team Preparation & Agile Scrum Hub

**Kho lưu trữ Tài liệu Nghiệp vụ, Cẩm nang Agile Scrum & Công cụ Luyện tập Trắc nghiệm Vòng 1**  
*Xây dựng giải pháp MVP AI Agent cho bài toán Ngân hàng VPBank theo quy trình Agile Scrum chuẩn quốc tế*

<p>
  <img src="https://img.shields.io/badge/Competition-Hack4Biz%202026-10B981?style=flat-square" alt="Hack4Biz 2026">
  <img src="https://img.shields.io/badge/Framework-Agile%20Scrum%202020-06B6D4?style=flat-square" alt="Agile Scrum">
  <img src="https://img.shields.io/badge/Domain-VPBank%20AI%20Agent-3B82F6?style=flat-square" alt="VPBank AI Agent">
  <img src="https://img.shields.io/badge/Quiz%20App-Single--File%20HTML5-F59E0B?style=flat-square" alt="Quiz HTML5">
</p>

</div>

---

## 1. Giới thiệu Tổng quan

Repository này là trung tâm lưu trữ tài liệu, công cụ ôn luyện và quy chuẩn làm việc của đội thi **Hack4Biz Competition 2026** (do **BUV** phối hợp cùng **VPBank** tổ chức), được thiết lập và quản lý bởi **Hà Tiến Triệu ([@trieuwu](https://github.com/trieuwu))**.

Đội hình dự thi gồm **5 vai trò chuẩn (5 Roles)** phối hợp xuyên suốt 3 vòng thi:
- **Vòng 1 — Online Assessment (`27/11/2026`):** Đánh giá kiến thức nền tảng và xử lý tình huống theo Agile Scrum cùng chuyên môn sâu của từng vị trí (`PM`, `PO`, `BA`, `DEV`, `QA`).
- **Vòng 2 — MVP Building (`08/12 – 23/12/2026`):** 16 ngày (chia làm 2 Sprint, 7 ngày/Sprint) phân tích nghiệp vụ (BRD, BPMN, Sequence Diagram) và phát triển sản phẩm **MVP AI Agent** chạy thực tế.
- **Vòng 3 — 32h Hackathon (`09/01 – 10/01/2027`):** Thi trực tiếp tại BUV (Ecopark), tiếp nhận và xử lý **Change Request (CR)** từ Ban Tổ chức ngay trên nền mã nguồn Vòng 2.

---

## 2. Cấu trúc Thư mục Chuẩn (Repository Structure)

```text
hack4biz/
├── .github/
│   └── pull_request_template.md          # Mẫu Pull Request chuẩn cho các nhánh đóng góp
├── docs/
│   ├── meetings/
│   │   └── report_18-11.md               # Biên bản họp triển khai đội thi & kế hoạch ôn tập (18/11/2026)
│   ├── pm/
│   │   └── pm_agile_scrum_handbook.md    # Cẩm nang chuyên sâu Project Manager & Agile Scrum (Playbook V1-V3)
│   └── slides/
│       ├── SLIDE.md                      # Đặc tả nội dung & thiết kế bộ Slide họp nội bộ 13 trang
│       └── slide_18-11.html              # Ứng dụng Web Slide Deck trình chiếu tương tác (Single-File HTML)
├── quiz/
│   ├── hack4biz_full_30.md               # Ngân hàng 30 câu hỏi trắc nghiệm chính thức & đáp án gốc (Markdown)
│   └── hack4biz_quiz.html                # Ứng dụng Web làm trắc nghiệm 30 câu tại local (Single-File HTML)
├── .gitignore                            # Cấu hình loại trừ tệp tạm, biến môi trường & công cụ AI cục bộ
└── README.md                             # Tài liệu hướng dẫn tổng quan dự án
```

---

## 3. Danh mục Tài liệu & Công cụ Trọng tâm

| Phân hệ | Đường dẫn Tệp | Mô tả Chi tiết |
| :--- | :--- | :--- |
| **Web Trắc Nghiệm Local (30 Câu)** | [`quiz/hack4biz_quiz.html`](quiz/hack4biz_quiz.html) | Ứng dụng web Single-File HTML5 luyện tập 30 câu hỏi trắc nghiệm chính thức tại local. Không có bộ đếm thời gian, hỗ trợ 2 chế độ (**Luyện tập chấm ngay** & **Thi thử nộp cuối**), lọc theo 6 chuyên đề (`Agile & Scrum`, `PM`, `PO`, `BA`, `DEV`, `QA`), trộn câu hỏi/đáp án, phím tắt bàn phím, giải thích chuyên môn và lưu tiến độ qua `localStorage`. |
| **Đề Trắc Nghiệm Gốc (Markdown)** | [`quiz/hack4biz_full_30.md`](quiz/hack4biz_full_30.md) | Văn bản gốc đầy đủ 30 câu hỏi kèm đáp án chuẩn (`Q1–Q30`). |
| **Cẩm Nang PM & Agile Scrum** | [`docs/pm/pm_agile_scrum_handbook.md`](docs/pm/pm_agile_scrum_handbook.md) | Tài liệu chuyên sâu gồm 5 phần: (1) Khung chuẩn Scrum Guide 2020; (2) Story Points, Velocity, Burndown/Burnup/CFD, DoR vs. DoD, INVEST, MoSCoW, RICE; (3) Nghiệp vụ PM trong Agile Hybrid & Ma trận RACI; (4) 25 câu hỏi tình huống có giải thích; (5) Playbook 16 ngày Vòng 2, Risk Register AI Ngân hàng & Quy trình 5 bước xử lý Change Request Vòng 3. |
| **Biên Bản Họp Đội Thi** | [`docs/meetings/report_18-11.md`](docs/meetings/report_18-11.md) | Biên bản thống nhất nguyên tắc làm việc nhóm, phân vai 5 thành viên và lịch trình ôn tập Vòng 1. |
| **Slide Trình Chiếu Nội Bộ** | [`docs/slides/slide_18-11.html`](docs/slides/slide_18-11.html) | Slide Deck tương tác 13 trang dùng trong buổi họp Kick-off ngày 18/11/2026 (hỗ trợ phím điều hướng, chế độ lưới `G`, toàn màn hình `F` và lưu dữ liệu nhập trực tiếp). |

---

## 4. Hướng dẫn Sử dụng Nhanh ở Local

Các công cụ web trong repository đều được đóng gói theo kiến trúc **Zero-Dependency Single-File HTML** (chỉ cần trình duyệt web hiện đại, không cần cài đặt server phức tạp):

```powershell
# 1. Clone repository về máy
git clone https://github.com/trieuwu/hack4biz.git
cd hack4biz

# 2. Mở trực tiếp ứng dụng Web Luyện tập Trắc nghiệm 30 câu trên trình duyệt mặc định
Start-Process .\quiz\hack4biz_quiz.html

# 3. Mở Slide Deck trình chiếu họp đội thi
Start-Process .\docs\slides\slide_18-11.html
```

### Phím tắt tiện ích trong ứng dụng `quiz/hack4biz_quiz.html` (Chế độ Từng câu)
- `A`, `B`, `C`, `D` hoặc `1`, `2`, `3`, `4`: Chọn nhanh phương án trả lời.
- `ArrowLeft` (`←`) / `ArrowRight` (`→`): Chuyển về câu trước / sang câu tiếp theo.
- `F`: Đánh dấu sao (`★`) câu hỏi cần xem lại.
- `E`: Ẩn / Hiện khung giải thích chuyên môn chi tiết.

---

## 5. Quy ước Quản lý Nhánh & Đóng góp (Git Workflow)

1. **Quy tắc đặt tên nhánh (`Branch Naming Convention`):**
   - `<type>/<mo-ta-tieng-viet-khong-dau>`
   - Ví dụ: `feat/web-trac-nghiem-30-cau`, `docs/chuan-hoa-tai-lieu-pm`, `fix/cap-nhat-cong-thuc-rice`.
2. **Quy tắc viết Commit Message (`Conventional Commits`):**
   - `<type>(<scope>): <mô tả tiếng Việt có dấu, ngắn gọn <= 72 ký tự>`
   - Các `type` hợp lệ: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`.
   - Các `scope` hợp lệ: `quiz`, `pm`, `docs`, `slides`, `meetings`, `repo`.
3. **Quy trình Pull Request:**
   - Mọi thay đổi đều được thực hiện trên nhánh riêng và tạo Pull Request hướng vào `main` theo mẫu [`.github/pull_request_template.md`](.github/pull_request_template.md).
