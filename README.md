# Track 1 - Day 27 — AI Team Lab

- **Team:** X (VinUni AI20K Build Phase — Cohort 3)
- **Thành viên (4 người):**
  - Phạm Đức Thiện — Team Lead (tài liệu, test, CI/CD) · *trưởng nhóm, người tổng hợp bài*
  - Đoàn Văn Tuyền — Input/sensor data, mô hình dự báo time-series (LSTM)
  - Nguyễn Minh Quang — Database Engineer (thiết kế DB, backend)
  - Võ Quốc Huy — LangGraph Agent
- **Tên dự án:** SC-07 — Hệ thống Giám sát Chất lượng Môi trường Đô thị Thông minh
- **Link sản phẩm/demo (nếu có):** _(cập nhật link demo/deploy tại đây)_

---

## Bài nộp

📄 [`Day27_AI-Team-Lab_TeamX.pdf`](./Day27_AI-Team-Lab_TeamX.pdf) — 4 trang:

| Trang | Nội dung |
| --- | --- |
| 1 | Stakeholder Map & Strategy — 8 stakeholder theo Influence × Interest, stance, 4 stakeholder ưu tiên + hành động cụ thể |
| 2 | Pitch "Conclusion First" tới BQL tòa nhà + phản biện & cách xử lý + RACI Matrix (6 công việc) |
| 3 | AI Team Design — kiến trúc Embedded, Core Roles, 3 capability gap + Priority Resourcing |
| 4 | Team Health & Growth Plan — điểm 4 khía cạnh, vấn đề ưu tiên, competency cần nâng, kế hoạch 30 ngày |

## Bối cảnh dự án

Hệ thống giám sát chất lượng môi trường theo thời gian thực cho Ban Quản Lý (BQL) tòa nhà / khu đô thị và cư dân, gồm 3 lớp:

- **Dự báo LSTM (PyTorch)** — dự báo PM2.5 / PM10 / CO2 cho 1–6 giờ tới theo từng khu vực.
- **LangGraph Incident Agent (13 node) + LLM** — phân tích nguyên nhân bất thường và đề xuất phương án xử lý.
- **Chat agent** — hỏi đáp trên web và Zalo, cá nhân hóa theo hồ sơ hộ gia đình.

Mức nguy hiểm được tính bằng threshold engine xác định (Python), **không** do LLM quyết định; mọi phương án xử lý đều human-in-the-loop, BQL duyệt và mỗi quyết định được ghi lại.

**Mục tiêu 1–3 tháng:** hoàn thiện MVP end-to-end và chạy pilot read-only 2 tuần với dữ liệu thật tại một tòa nhà.

## Checklist nộp bài

- [x] Repo có `README.md`
- [x] Repo có đúng 01 file PDF bài làm
- [x] PDF đúng 4 trang
- [x] README ghi đủ tên team, thành viên và tên dự án
- [x] Repo: `Track1_Day27_X_AirWatch`
- [ ] Repo mở quyền truy cập để giảng viên có thể xem
