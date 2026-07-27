# 03 — Individual Reflection

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| **Scan cá nhân** | Thực hiện scan rộng 8 vấn đề thực tế xoay quanh vai trò Recruiter/HR. | Giúp nhóm có thêm góc nhìn và dữ liệu về mảng quy trình tuyển dụng và quản trị thông tin. |
| **Pitch Problem Card** | Trình bày chi tiết Problem Card về việc "Sàng lọc CV & Viết Shortlist Narrative". | Thuyết phục nhóm đưa đề xuất này vào danh sách so sánh và đánh giá để hội tụ. |
| **Challenge bài của bạn khác** | Đặt câu hỏi chất vấn về độ khả thi y khoa của bài "Giải thích phiếu xét nghiệm" và sự thiếu tập trung của bài "Gia sư + Q&A học sinh". | Giúp nhóm nhận diện các rủi ro lớn về mặt chuyên môn/pháp lý và loại bỏ các bài toán bị gộp workflow. |
| **Gom trùng / cluster** | Cùng nhóm phân tích các pattern chung của các candidate (feedback kỹ năng, giải thích thông tin chuyên môn, điều phối lịch). | Giúp nhóm phân loại rõ ràng các hướng tiếp cận bài toán trước khi chấm điểm. |
| **Chọn candidate problem** | Đồng thuận chọn bài toán "AI Gym cảnh báo lỗi squat khi tự tập", dù bài cá nhân của mình không được chọn. | Nhận thức được bài toán Gym Coach có workflow vật lý rõ ràng và dễ đo lường bằng rubric kỹ thuật của PT hơn. |
| **Validation / research** | Tìm hiểu các sản phẩm hiện có như Kaia Motion Coach và Tempo Studio, trích dẫn các tài liệu nghiên cứu về resistance training. | Rút ra bài học quan trọng về camera check và confidence gate trước khi đưa ra feedback. |
| **Workflow nhóm** | Thiết kế quy trình trước/sau cho bài tập Squat, đề xuất đưa khâu "Confidence Gate" vào quy trình tương lai. | Bảo vệ hệ thống khỏi việc đưa ra cảnh báo sai khi camera bị che khuất hoặc thiếu sáng. |
| **Problem Statement** | Viết metric cụ thể cho thời gian tìm rep (<10s) và độ đồng thuận với PT (tối thiểu 85%). | Chuyển đổi các mục tiêu mơ hồ thành các chỉ số kỹ thuật có thể đo lường trong pilot. |
| **Rule / Workflow / Agent** | Lập luận cùng nhóm chọn mức độ giải pháp là Workflow thay vì Agent. | Giảm thiểu tối đa rủi ro chấn thương cho người dùng bằng cách tước đi quyền tự quyết giáo án/mức tạ của AI. |
| **Decision** | Thuyết phục nhóm đưa ra kết luận "Not Yet" cho quyết định cuối cùng. | Đảm bảo tính trung thực khoa học, chỉ chạy pilot có giám sát chứ chưa vội vàng phát hành sản phẩm. |

---

## 2. Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| **Scan** | Gợi ý thêm các vấn đề thực tế trong ngành tuyển dụng dựa trên vai trò Recruiter. | Giúp mở rộng góc nhìn sang các mảng như Onboarding và lên lịch phỏng vấn. | Đưa ra các ý tưởng quá chung chung kiểu "Trợ lý AI viết email tự động". | Lọc bỏ và tự viết lại dựa trên quy trình thao tác thực tế của Lan. |
| **Problem Card** | Đóng vai một skeptical PM để phản biện Problem Card lọc CV. | Chỉ ra các lỗ hổng về bảo mật thông tin ứng viên (PII) và tính chủ quan của metric chất lượng. | Khuyên chuyển hướng giải pháp sang hệ thống Agent phức tạp ngay lập tức. | Giữ nguyên mức Workflow và bổ sung các boundary/fallback về bảo mật dữ liệu. |
| **Workflow** | Hỗ trợ chuyển tả ý tưởng workflow Squat sang định dạng text/Mermaid. | Tiết kiệm thời gian định dạng và sắp xếp sơ đồ quy trình. | Gộp chung bước AI Pose Estimation và Rule Check thành một khối duy nhất. | Tách riêng hai bước này để chèn Confidence Gate ở giữa nhằm lọc dữ liệu rác. |
| **Research** | Tìm thông tin về đối thủ Kaia Health và Tempo Studio. | Gợi ý nhanh các đối thủ và công nghệ landmarks họ sử dụng. | Đưa ra thông tin ước tính hiệu quả tiết kiệm thời gian mà không ghi nguồn rõ ràng. | Tự tìm các nghiên cứu khoa học chính thức về feedback trong thể thao để trích dẫn. |
| **Problem Statement** | Phản biện các trường thông tin trong bản thảo PS v0. | Chỉ ra rằng các thành công metric của nhóm vẫn hoàn toàn là giả định chưa được validate. | Khuyên sửa các metric thành các con số chắc chắn để "báo cáo đẹp hơn". | Giữ nguyên dưới dạng "giả định cần validate trong pilot" để đảm bảo tính trung thực. |
| **Rule / Workflow / Agent** | Phân tích ma trận độ phức tạp/mơ hồ cho bài toán squat. | Xác định đúng mức độ mơ hồ thấp và phức tạp cao trong phạm vi pilot. | AI khuyên chọn Agent vì có nhiều bước liên kết động. | Nhóm phản biện lại: Agent có quyền tự quyết quá cao gây nguy hiểm chấn thương, thống nhất hạ về Workflow. |
| **Decision** | Hỏi cách lập quy trình pilot tối thiểu (MVP) để kiểm chứng. | Gợi ý các bước thu thập video và cách thức gán nhãn chéo giữa các PT. | AI thiên vị nút "Go" vì cho rằng công nghệ landmarks đã rất sẵn sàng. | Quyết định chốt "Not Yet" vì nhóm chưa chạy thử nghiệm quan sát (observed test) và chưa có dữ liệu gán nhãn thực tế. |

---

## 3. Reflection câu hỏi mở

*   **Tôi học được gì khi nghe top 3 problems của các bạn khác?**
    *   Tôi nhận ra rằng một problem tốt luôn xuất phát từ hành vi cụ thể (behavior) và cảm xúc thực tế (emotion) của actor khi họ bị nghẽn, chứ không phải từ việc công nghệ AI đó "ngầu" thế nào. Ví dụ, bạn làm về Gym Coach tiếp cận bằng nỗi lo sợ chấn thương và sự bối rối khi tự xem video của người tập, giúp bài toán có tính thuyết phục rất cao.
*   **Nhóm có lúc nào bị solution-first không?**
    *   Có. Khi bắt đầu thảo luận bài toán Gym Coach, cả nhóm đã hào hứng vẽ ra một "AI PT toàn năng" có thể tự nói chuyện động viên, tự tăng tạ và kê giáo án dinh dưỡng. Nhưng sau khi soi chiếu kỹ lăng kính "Ranh giới & Rủi ro", nhóm nhận thấy việc để AI tự quyết giáo án/mức tạ mà không có khám sức khỏe trực tiếp rất nguy hiểm. Nhóm đã quyết định kéo scope về cực kỳ hẹp: chỉ hỗ trợ sửa 3 lỗi của động tác bodyweight squat.
*   **Tôi có thay đổi ý kiến sau khi bị challenge không?**
    *   Có. Ban đầu tôi rất muốn nhóm chọn bài "Sàng lọc CV" của mình. Tuy nhiên, sau khi bị các bạn challenge: *"Làm sao đo được chất lượng bản tóm tắt CV một cách khách quan?"* và *"Vấn đề bảo mật dữ liệu CV giải quyết thế nào?"*, tôi nhận thấy việc đo lường chất lượng chữ viết mang tính chủ quan cao và rủi ro pháp lý lớn hơn bài Squat (vốn có thể đo bằng rubric kỹ thuật rõ ràng của PT). Tôi đã vui vẻ đồng thuận chuyển sang bài Gym Coach.
*   **Tôi đóng góp gì thật sự vào artifact cuối của nhóm?**
    *   Tôi đề xuất bước "Confidence Gate" trong tương lai (nếu độ tin cậy của landmarks dưới ngưỡng do ánh sáng hoặc che khớp thì hệ thống im lặng, không đưa cue bừa bãi). Tôi cũng trực tiếp xây dựng bộ "Metric contract" rõ ràng cho buổi pilot (đo lường độ đồng thuận với PT và tỷ lệ false alert) và phần "Exit/Rollback".
*   **Điều khó nhất khi viết Problem Statement là gì?**
    *   Khó nhất là việc tách biệt giữa con số giả định và con số thực tế trong Success Metric. Nhóm rất dễ bị cám dỗ ghi bừa một con số như "giảm 50% chấn thương" hoặc "giảm 80% thời gian", nhưng thực tế nhóm chưa đo lường baseline. Khó khăn là phải thừa nhận "đây là con số giả định cần validate" và ghi rõ phương pháp đo lường (timed test, blind test) thay vì chỉ đưa ra target mơ hồ.
*   **Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?**
    *   Tôi sẽ challenge nhóm thực hiện một "Observed Test" nhanh ngay trong 4 tiếng lab. Thay vì chỉ ghi lý thuyết, nhóm nên gọi ngay 1-2 bạn trong lớp ra thực hiện thử động tác Squat trước camera điện thoại để kiểm chứng ngay xem việc đặt camera có thực sự là một bottleneck lớn không và họ có cảm thấy phiền phức khi phải căn chỉnh góc quay hay không.

---

## 4. Tự kiểm cuối bài (Self-Check)

- [x] **[12đ cá nhân]** Cá nhân có 5+ problems và top 3 Problem Cards.
- [x] **[12đ cá nhân]** Tôi đã pitch rõ và challenge nhóm đúng trọng tâm.
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài.
- [x] **[15đ nhóm]** Nhóm có workflow trước/sau.
- [x] **[20đ nhóm]** Nhóm có Problem Statement v0/v1 với metric và boundary rõ.
- [x] **[15đ nhóm]** Nhóm có so sánh No AI / Rule / Workflow / Agent.
- [x] **[10đ nhóm]** Nhóm có Go / Not Yet / No-Go và lý do rõ.
- [x] **[10đ cá nhân]** Reflection cá nhân có nói rõ vai trò trong nhóm, cách dùng AI, điều học được và nếu làm lại sẽ đổi gì.
- [x] **[6đ cá nhân]** Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp với AI.
