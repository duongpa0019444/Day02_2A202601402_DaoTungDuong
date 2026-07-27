# 01 — Individual Problem Scan (Case 1: Tuyển dụng / HR)

## Scan rộng

Dưới đây là bảng scan 8 problems thực tế trong công việc của Lan (Talent Acquisition Specialist), sử dụng 4 lăng kính khác nhau để tìm ra điểm nghẽn thực sự.

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại | Đọc CV và đối chiếu với JD để viết bản tóm tắt nhận xét (shortlist narrative) cho Hiring Manager. | Lan, Hiring Manager | Mất 10-15 phút/CV. Với 50 CV/tuần, Lan tốn từ 8-12 tiếng chỉ để đọc và viết đánh giá. |
| 2 | Lặp lại | Soạn thư mời nhận việc (Offer Letter) dựa trên thông tin ứng viên và chính sách phúc lợi tiêu chuẩn của công ty. | Lan, Ứng viên | Lặp lại 5-7 lần/tuần, mất 15 phút/thư để điền thông tin thủ công. |
| 3 | Tốn thời gian | Tìm kiếm lịch trống của 3-4 Hiring Manager khác nhau để xếp lịch phỏng vấn chéo cho ứng viên. | Lan, Hiring Managers | Mất 15-20 phút cho mỗi buổi phỏng vấn được lên lịch, thường xuyên phải nhắn tin qua lại để xác nhận. |
| 4 | Tốn thời gian | Đọc các bài viết kỹ thuật hoặc bài test của ứng viên dev để kiểm tra tính hợp lệ sơ bộ trước khi gửi cho Tech Lead. | Lan, Tech Lead | 30-40 phút/bài test. Lan phải tự đối chiếu kết quả với barem điểm thô. |
| 5 | AI có thể tốt hơn | Tổng hợp các phản hồi phỏng vấn (interviewer feedback) rải rác từ Slack, email thành email quyết định cuối cùng (offer/reject). | Lan, HR Manager | Mất 20-30 phút/ứng viên. Khó đồng nhất giọng văn và các điểm cần lưu ý của từng người phỏng vấn. |
| 6 | AI có thể tốt hơn | Viết tin tuyển dụng (Job Posting) hấp dẫn, thu hút ứng viên từ một bản JD kỹ thuật thô và khô khan. | Lan | Mất 45 phút/bản. Bản tin dễ bị đơn điệu, thiếu sáng tạo nếu tuyển dụng nhiều vị trí cùng lúc. |
| 7 | Pain từ người khác | Ứng viên phàn nàn trên mạng xã hội hoặc gửi mail hỏi thăm do không nhận được phản hồi sau khi nộp CV. | Ứng viên, Uy tín công ty | Nhận 10-15 email hỏi tình trạng hồ sơ mỗi tuần. Gây ảnh hưởng xấu đến Employer Branding. |
| 8 | Pain từ người khác | Hiring Manager phàn nàn rằng CV Lan gửi qua không đúng yêu cầu chi tiết của dự án vì JD viết quá chung chung. | Lan, Hiring Manager | Mất 30-45 phút họp lại để làm rõ yêu cầu cho mỗi vị trí mới mở. |

---

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | **Lọc CV & Viết Shortlist Narrative** | Tần suất lặp lại cực cao (hằng ngày), tốn nhiều thời gian nhất trong workflow tuyển dụng, ảnh hưởng trực tiếp đến tốc độ phản hồi ứng viên. | Làm sao để AI tóm tắt chính xác các dự án thực tế của ứng viên mà không bị ảo tưởng (hallucination). |
| 2 | **Xếp lịch phỏng vấn chéo** | Gây nghẽn tiến độ phỏng vấn do giao tiếp bất đối xứng giữa Lan, ứng viên và nhiều Hiring Manager. | Có cần thiết dùng AI không hay chỉ cần tích hợp hệ thống calendar tự động (như Calendly/tidycal). |
| 3 | **Viết tin tuyển dụng từ JD thô** | Có pain thật về tính sáng tạo và thu hút ứng viên, AI rất mạnh về mảng tạo nội dung này. | Chất lượng tin tuyển dụng do AI tạo ra có thực sự giúp tăng số lượng CV nộp về hay không. |

---

## Problem Card #1 — Lọc CV & Viết Shortlist Narrative

**Problem 1 câu:**  
Lan mất khoảng 8-12 tiếng mỗi tuần để đọc thủ công hàng chục CV và viết bản nhận xét tóm tắt (shortlist narrative) đối chiếu với JD gửi cho Hiring Manager, dẫn đến chậm phản hồi cho ứng viên và kéo dài thời gian tuyển dụng.

**Actor:**  
Lan, Talent Acquisition Specialist chịu trách nhiệm sàng lọc hồ sơ ứng viên Tech.

**Thời điểm / bối cảnh:**  
Mỗi ngày khi có CV mới đổ về từ LinkedIn và TopCV.

**Current workflow:**
1. Tải CV của ứng viên dưới dạng PDF/Docx về máy.
2. Mở file JD vị trí tương ứng để đối chiếu tiêu chí (Kỹ năng, Kinh nghiệm, Dự án liên quan).
3. Đọc kỹ CV và viết nhận xét chi tiết (điểm mạnh, điểm yếu, mức độ phù hợp) vào bản tóm tắt.
4. Copy nhận xét gửi qua kênh Slack cho Hiring Manager duyệt.
5. Gửi email phản hồi cho ứng viên (từ chối hoặc hẹn phỏng vấn).

**Bottleneck:**  
Bước 3 — Viết bản nhận xét tóm tắt chi tiết cho từng hồ sơ mất trung bình 7-10 phút/CV, yêu cầu độ tập trung cao và dễ bị mệt mỏi về cuối ngày.

**Impact:**  
Mất 8-12 tiếng/tuần cho 1 recruiter. Thời gian phản hồi ứng viên vòng hồ sơ bị kéo dài lên 5-7 ngày. Tỷ lệ ứng viên rút khỏi quy trình tuyển dụng tăng vì chờ đợi quá lâu.

**Success metric:**  
Giảm tổng thời gian xử lý mỗi CV từ 15 phút xuống dưới 3 phút (bao gồm cả thời gian review của Lan). Thời gian gửi CV shortlist sang Hiring Manager giảm từ 2 ngày xuống còn dưới 12 giờ kể từ khi ứng viên ứng tuyển.

**Non-AI alternative:**  
Dùng hệ thống ATS lọc từ khóa tự động. Tuy nhiên, cách này chỉ lọc được từ khóa cứng (keywords), dễ bỏ sót các ứng viên viết CV theo cách khác, và không tạo ra được bản nhận xét (narrative) chi tiết gửi Hiring Manager.

**AI hypothesis:**  
AI sẽ đọc nội dung CV và JD, đối chiếu các yêu cầu và tự động soạn thảo bản nhận xét tóm tắt (shortlist narrative) theo các tiêu chí (Điểm mạnh, Điểm yếu, Đánh giá chung). Lan chỉ đóng vai trò review và chỉnh sửa bản thảo.

**Quick gut:**  
[x] Workflow  
(Quy trình tuyến tính rõ ràng: Input là CV + JD -> AI xử lý ngôn ngữ và soạn thảo -> Lan duyệt và gửi đi).

### Draft current workflow
```text
CURRENT STATE — 15 phút/CV

[1 Tải CV từ các nguồn: 1']
→ [2 Đọc CV đối chiếu JD: 5']
→ [3 Viết shortlist narrative: 7']  <-- bottleneck
→ [4 Gửi Slack cho Hiring Manager: 1']
→ [5 Gửi phản hồi cho ứng viên: 1']
```

### Draft future workflow
```text
FUTURE STATE — 3 phút/CV

[1 AI trích xuất và đối chiếu CV với JD: 0.5']  -- Workflow step (AI)
→ [2 AI draft shortlist narrative: 0.5']         -- Workflow step (AI)
→ [3 Lan review + edit nhận xét: 1.5']            -- Human boundary
→ [4 Lan gửi duyệt & phản hồi ứng viên: 0.5']

Fallback: AI draft sai hoặc thiếu thông tin quan trọng -> Lan bỏ draft và tự viết lại dựa trên CV gốc.
```

---

## Problem Cards #2 và #3 — tóm tắt

| Card | Actor | Bottleneck | Metric | Quick gut | Vì sao chưa chọn làm #1 |
|---|---|---|---|---|---|
| **Xếp lịch phỏng vấn** | Lan | Tìm giờ khớp giữa các bên và chờ ứng viên phản hồi. | 20 phút → 2 phút | Rule / Workflow | Có thể xử lý tốt bằng công cụ rule-based (như Calendly) để tự động hóa xếp lịch mà không nhất thiết cần đến AI. |
| **Viết tin tuyển dụng** | Lan | Bí ý tưởng viết tin tuyển dụng sáng tạo, chuẩn kỹ thuật từ JD thô. | 45 phút → 10 phút | Workflow | Tần suất sử dụng thấp (chỉ viết khi có job mới, khoảng 1-2 lần/tháng), impact tổng thể không lớn bằng sàng lọc CV hằng ngày. |

---

## Chọn card muốn pitch nhất

### Card tôi muốn pitch nhất:
`Problem Card #1 — Lọc CV & Viết Shortlist Narrative`

### Vì sao:
* Vấn đề này có tần suất lặp lại hằng ngày và chiếm nhiều thời gian nhất trong tuần của một Recruiter.
* Giải quyết được điểm nghẽn này sẽ cải thiện trực tiếp trải nghiệm ứng viên (Candidate Experience) nhờ đẩy nhanh tốc độ phản hồi, giúp doanh nghiệp giành lợi thế trong việc săn đón nhân tài.
* Điểm nghẽn nằm ở khâu đọc hiểu ngữ cảnh (kinh nghiệm dự án của ứng viên đối chiếu với yêu cầu JD) và diễn đạt ngôn ngữ (viết nhận xét) - đây là thế mạnh cốt lõi của các mô hình ngôn ngữ lớn (LLM).

### Câu hỏi tôi muốn nhóm challenge:
1. "Làm sao để thiết lập prompt hoặc cấu trúc dữ liệu để AI không bỏ sót các thông tin ngầm định (implicit skills) trong CV của ứng viên tech?"
2. "Làm cách nào để đảm bảo tính bảo mật thông tin cá nhân (PII) của ứng viên khi đưa CV vào các công cụ AI để xử lý?"
