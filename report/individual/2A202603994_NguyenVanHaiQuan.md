# Báo cáo cá nhân — 2A202603994_NguyenVanHaiQuan

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).

## 1. Thông tin học viên

- Họ tên: Nguyễn Văn Hải Quân
- MSSV: 2A202603994
- Tên nhóm: Nhom1
- Link repo nhóm: https://github.com/cduyminh/K5-L3B-DAY02-Nhom1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi vừa học xong một buổi ở lớp Đào tại AI Thực Chiến 20K (lý thuyết, Lab hoặc Workshop), tôi muốn ghi chú của buổi đó được sắp xếp gọn vào đúng chỗ, để tuần sau tra lại được mà không phải xem lại cả buổi | Tôi và các bạn học viên cùng lớp  20K | Riêng phần lý thuyết có 6 tuần × 5 buổi = 30 buổi. Mỗi buổi tôi mất 45 phút để dựng lại ghi chú. Trong tuần trước có hơn 10 lần phải mở lại slide hoặc recording vì ghi chú thiếu |
| 2 | Tốn thời gian | Khi một lỗi triển khai xuất hiện sau vài tuần không đụng tới (ví dụ DNS của api.tutora.vn), tôi muốn tìm ra cấu hình và lý do đã chọn ban đầu, để sửa nhanh mà không làm hỏng chỗ khác | Tôi và các thành viên nhóm Tutora | Hệ thống nối nhiều dịch vụ (VPS, GitHub Actions, Docker Hub, PayOS, Gemini). Lần gần nhất mất hơn 1 giờ để truy ra nguyên nhân, phải mở 10-12 nơi khác nhau (dashboard, repo, tin nhắn) |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi viết phần tài liệu liên quan cho bài CAR (dự định nộp RIVF/KSE), tôi muốn nắm nhanh phương pháp, dữ liệu và hạn chế của từng bài báo, để so sánh được với hướng của mình | Tôi và thầy hướng dẫn | Đã đọc 7-10 bài, trung bình 30 phút/bài. Có khoảng 2-3 lần phải mở lại một bài đã đọc vì quên chi tiết |
| 4 | Tốn thời gian | Khi chuẩn bị nộp CV cho một vị trí, tôi muốn biết CV của mình đáp ứng yêu cầu tuyển dụng đến đâu, để không nộp hàng chục nơi mà không có phản hồi | Sinh viên năm cuối, trong đó có tôi | Theo VietnamWorks, nhà tuyển dụng chỉ lướt CV khoảng 20–30 giây (bài viết tự ước lượng, không có khảo sát). Số liệu của tôi: đã nộp 22 CV, nhận 15 phản hồi, mất 30 phút sửa CV cho mỗi vị trí |
| 5 | Pain từ người khác | Khi đi khám ngoại trú có làm xét nghiệm, tôi muốn biết trước mình sẽ phải chờ bao lâu ở từng khâu, để sắp xếp được thời gian trong ngày | Bệnh nhân ngoại trú và người nhà | Khảo sát 255 người bệnh tại BV Lê Văn Việt (TP.HCM): thời gian chờ trung bình là 13,0 phút ở khâu đăng ký, 9,2 phút ở khâu khám, 12,9 phút ở khâu nhận thuốc, 7,5 phút ở khâu thanh toán. Riêng xét nghiệm chờ **61,0 ± 26,6 phút**, lâu nhất 240 phút. Lần gần nhất người nhà tôi đi khám mất hơn 2 giờ |
| 6 | Pain từ người khác | Khi brand gửi yêu cầu đổi giá hoặc ngừng bán một biến thể, tôi muốn chắc chắn thay đổi đã lên đúng trên cả Shopee, TikTok Shop và Lazada, để không bán sai giá hoặc bán hàng đã ngừng | Nhân sự vận hành tại enabler (bên nhận vận hành gian hàng thay brand), brand, khách mua | Số liệu thu thập được: 1–2 yêu cầu thay đổi/tuần, 10–12 phút kiểm tay mỗi yêu cầu cho đủ 3 sàn, 5 lần phát hiện lệch giá/biến thể trong 3 tháng qua (≈ 13–26 yêu cầu, tức khoảng 19–38% yêu cầu bị lệch). Kịch bản lỗi trong prototype LênSàn (giá 350.000đ nhập thành 35.000đ trên Lazada) là dữ liệu mô phỏng, không phải bằng chứng |
| 7 | Lặp lại | Khi nhận catalog của một brand mới (PDF, Excel, ảnh, có khi lệch nhau giữa các file), tôi muốn có listing đúng quy ước của từng sàn Shopee, TikTok Shop, Lazada cho mọi SKU, để mở bán đúng hẹn mà không bị sàn từ chối hay đình chỉ sản phẩm | Nhân sự vận hành tại enabler, brand | Số liệu thu thập được từ người từng làm vận hành enabler, về lần onboard gần nhất: 20–35 phút/SKU cho cả 3 sàn (≈ 7–12 phút/listing); 240 SKU; 4 ngày từ lúc nhận catalog đến lúc mở bán; 14 listing bị sàn từ chối. Tức 240 × 3 sàn = 720 listing, khoảng 80–140 giờ công dồn vào 4 ngày. Nguồn ngoài (bên bán công cụ đăng hàng loạt) ước tính đăng tay 10–20 phút/listing, cao hơn số thực tế này. Catalog mẫu trong prototype LênSàn là dữ liệu mô phỏng, không phải bằng chứng |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Dòng 4 và 5 lấy từ gợi ý của AI về tình hình chung ở Việt Nam. Tôi giữ lại vì có số liệu kiểm chứng được (dòng 5) hoặc tôi tự đo được trên chính mình (dòng 4). Tôi đã bỏ con số "60 giây/CV" và "37% nhà tuyển dụng (Pearson-AWS)" do AI đưa ra, vì khi tự tìm lại, nguồn VietnamWorks chỉ ghi 20–30 giây và tôi không tìm thấy nguồn cho con số 37%.
- Bỏ ý "hộ kinh doanh chuyển sang kế toán đầy đủ từ 2026": impact lớn nhưng tôi không tiếp cận được actor thật để phỏng vấn trong buổi lab.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | #7 Dựng listing đa sàn từ catalog brand (LênSàn) | Lần onboard gần nhất: 240 SKU × 3 sàn = 720 listing trong 4 ngày, 14 listing bị từ chối. Việc lặp theo từng SKU × sàn nên đo được rõ. Nhóm có thành viên làm đúng nghề này nên tìm được người thật để phỏng vấn | Số liệu do người từng làm nhớ lại, đã rời ngành một thời gian, cần kiểm lại với người đang làm. Phần mềm đa kênh và file đăng hàng loạt của sàn có thể đã giải phần lớn |
| 2 | #1 Sắp xếp ghi chú sau buổi học 20K | Lặp lại 30 buổi, tôi tự đo được (45 phút/buổi, hơn 10 lần mở lại trong tuần), cả lớp cùng gặp nên dễ kiểm chứng | Công cụ ghi chú đã có rất nhiều; có thể chỉ cần template cố định là đủ |
| 3 | #3 Đọc paper cho bài CAR | Tôi là actor thật, đã đo 30 phút/bài trên 7–10 bài | Số liệu trích sai trong bảng so sánh gây hại hơn việc đọc chậm; chỉ có 1–2 người gặp nên impact nhỏ |

### Problem Card #1 — Dựng listing đa sàn từ catalog của brand (LênSàn)

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận catalog của một brand mới (PDF, Excel, ảnh, có khi lệch nhau giữa các file), tôi muốn có listing đúng quy ước của từng sàn Shopee, TikTok Shop, Lazada cho mọi SKU, để mở bán đúng hẹn mà không bị sàn từ chối hay đình chỉ sản phẩm |
| Actor | Nhân sự vận hành tại enabler, giai đoạn onboard brand mới hoặc brand mở thêm sàn |
| Thời điểm / bối cảnh | Mỗi lần ký brand mới hoặc brand mở thêm sàn; thường có hạn mở bán cố định, dày nhất trước các kỳ sale lớn |
| Quy trình hiện tại (3–7 bước) | 1. Nhận catalog, đối chiếu các file khi giá hoặc quy cách lệch nhau · 2. Chọn danh mục cho từng SKU trên từng sàn · 3. Viết tiêu đề theo quy ước riêng từng sàn (Shopee tối đa 120 ký tự; TikTok Shop tối đa 100 ký tự, không nhắc sàn khác; Lazada bắt đầu bằng thương hiệu) · 4. Điền thuộc tính bắt buộc của từng sàn, thiếu thì hỏi brand · 5. Rà câu quảng cáo có nguy cơ vi phạm (ví dụ mỹ phẩm không được nói "trị dứt điểm") · 6. Đăng (thủ công hoặc file hàng loạt) và chờ sàn duyệt |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: cùng một SKU phải viết lại tiêu đề 3 lần theo 3 quy ước và điền 3 bộ thuộc tính khác nhau. Toàn bộ việc đăng mất 20–35 phút/SKU cho 3 sàn (≈ 7–12 phút/listing), chưa tách riêng bước 3–4. Bước 5 là điểm rủi ro: bỏ sót một câu vi phạm thì listing bị từ chối hoặc đình chỉ |
| Impact (nếu không giải thì sao) | Lần onboard gần nhất: 240 SKU × 3 sàn = 720 listing. Với 20–35 phút/SKU cho 3 sàn, đó là 80–140 giờ công dồn vào 4 ngày, tức cần khoảng 3–4 người làm toàn thời gian chỉ để đăng hàng. 14 listing bị sàn từ chối (≈ 1,9%) phải làm lại. Nếu không kịp thì mở bán trễ hạn với brand |
| Success metric (baseline → target) | Baseline: 20–35 phút/SKU cho 3 sàn (cần bấm giờ lại trên 5 SKU thật); 4 ngày cho 240 SKU; 14/720 ≈ 1,9% listing bị từ chối ở lần đăng đầu. Target: giảm ≥ 60% thời gian, tỉ lệ bị từ chối không tăng; 100% giá trị do hệ thống tự suy ra được đánh dấu và có người xác nhận. Cách đo: so 2 lần onboard trước/sau |
| Phương án không dùng AI | Template tiêu đề theo từng sàn + file Excel đăng hàng loạt của sàn + checklist thuộc tính bắt buộc + danh sách từ cấm. Giảm được công nhập liệu; cần kiểm ở CP4 xem phần mềm quản lý đa kênh có sẵn đã sao chép listing giữa các sàn tới đâu. Phần chưa giải được: đọc catalog lộn xộn, chọn danh mục và viết tiêu đề cho SKU chưa từng gặp |
| Giả thuyết về AI (nếu có) | AI đọc catalog thành một bản dữ liệu gốc (báo chỗ các nguồn lệch nhau), đề xuất danh mục kèm độ tin cậy, viết tiêu đề theo quy ước từng sàn, gạch chân câu có nguy cơ vi phạm. Người review từng listing như review pull request rồi mới đăng. Danh mục có độ tin cậy dưới 0,8 và mọi giá trị tự suy ra phải có người xác nhận |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 20–35 phút/SKU cho cả 3 sàn (≈ 7–12 phút/listing)
Một lần onboard: 240 SKU → 720 listing → 80–140 giờ công trong 4 ngày (≈ 3–4 người); 14 listing bị từ chối

[1 Nhận + đối chiếu catalog: ?'] → [2 Chọn danh mục × 3 sàn: ?']
→ [3 Viết tiêu đề × 3 sàn: ?'] ← BOTTLENECK
→ [4 Điền thuộc tính bắt buộc × 3 sàn: ?'] ← BOTTLENECK
→ [5 Rà câu quảng cáo vi phạm: ?'] ← điểm rủi ro (bỏ sót thì bị đình chỉ)
→ [6 Đăng, chờ sàn duyệt: ?']
```

### Problem Card #2 — Sắp xếp ghi chú sau buổi học 20K

| Trường | Nội dung |
|---|---|
| Job Story | Khi vừa học xong một buổi ở lớp AI Thực Chiến 20K (lý thuyết, Lab hoặc Workshop), tôi muốn ghi chú của buổi đó được sắp xếp gọn vào đúng chỗ, để tuần sau tra lại được mà không phải xem lại cả buổi |
| Actor | Học viên lớp 20K (tôi và các bạn cùng lớp) |
| Thời điểm / bối cảnh | Ngay sau mỗi buổi học; 6 tuần × 5 buổi lý thuyết = 30 buổi, chưa tính Lab và Workshop |
| Quy trình hiện tại (3–7 bước) | 1. Ghi nhanh trong buổi · 2. Sau buổi gom slide, link, recording · 3. Viết lại ghi chú có cấu trúc · 4. Đưa vào Notion đúng tuần, đúng buổi · 5. Tuần sau tra lại khi làm lab hoặc ôn tập |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, viết lại ghi chú có cấu trúc: [?] phút trong tổng 45 phút/buổi |
| Impact (nếu không giải thì sao) | 45 phút × 30 buổi ≈ 22,5 giờ cho riêng phần lý thuyết. Ghi chú thiếu làm tôi phải mở lại slide/recording hơn 10 lần trong tuần trước |
| Success metric (baseline → target) | Baseline: 45 phút/buổi; hơn 10 lần/tuần phải mở lại tài liệu gốc. Target: ≤ 20 phút/buổi; ≤ 3 lần/tuần. Cách đo: bấm giờ 3 buổi liên tiếp, đếm số lần mở lại trong 1 tuần |
| Phương án không dùng AI | Template ghi chú cố định theo buổi trong Notion (mục tiêu, khái niệm, ví dụ, câu hỏi còn lại); chia việc ghi chú luân phiên với bạn cùng lớp |
| Giả thuyết về AI (nếu có) | AI chuyển slide + ghi nhanh thành ghi chú theo template; người học đọc lại và sửa trước khi lưu |
| Cảm nhận nhanh | Workflow (có thể No AI nếu template đủ) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 45 phút/buổi

[1 Ghi nhanh trong buổi: trong giờ học] → [2 Gom slide/link/recording: ?']
→ [3 Viết lại ghi chú có cấu trúc: ?'] ← BOTTLENECK
→ [4 Đưa vào Notion đúng buổi: ?'] → [5 Tra lại tuần sau: hơn 10 lần/tuần]
```

### Problem Card #3 — Đọc paper cho phần tài liệu liên quan của bài CAR

| Trường | Nội dung |
|---|---|
| Job Story | Khi viết phần tài liệu liên quan cho bài CAR (dự định nộp RIVF/KSE), tôi muốn nắm nhanh phương pháp, dữ liệu và hạn chế của từng bài báo, để so sánh được với hướng của mình |
| Actor | Tôi (sinh viên làm nghiên cứu) và thầy hướng dẫn |
| Thời điểm / bối cảnh | Giai đoạn viết Related Work, trước hạn nộp hội nghị |
| Quy trình hiện tại (3–7 bước) | 1. Tìm và tải paper · 2. Đọc lướt abstract, intro, kết luận để quyết định đọc tiếp · 3. Đọc kỹ phần phương pháp · 4. Đọc thực nghiệm, ghi dataset, metric, kết quả · 5. Ghi vào bảng so sánh · 6. Quay lại tra khi viết bài |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4, đọc sâu để rút phương pháp và số liệu: [?] phút trong tổng 30 phút/bài |
| Impact (nếu không giải thì sao) | 7–10 bài × 30 phút ≈ 3,5–5 giờ, và còn tăng khi mở rộng tổng quan. 2–3 lần phải mở lại bài đã đọc vì bảng so sánh thiếu chi tiết. Mốc tham chiếu: Keshav ước tính lượt đọc thứ hai mất tới 1 giờ/bài |
| Success metric (baseline → target) | Baseline: 30 phút/bài; 2–3 lần mở lại. Target: ≤ 15 phút/bài; 0 lần mở lại; 0 số liệu sai so với bản gốc. Cách đo: bấm giờ trên 3 bài tiếp theo, đối chiếu bảng với PDF |
| Phương án không dùng AI | Mẫu ghi chú cố định cho mỗi bài (bài toán, phương pháp, dataset, kết quả, hạn chế, số trang) + đọc theo phương pháp ba lượt của Keshav |
| Giả thuyết về AI (nếu có) | AI trích các trường từ PDF, mỗi trường kèm số trang gốc; tôi đối chiếu rồi mới đưa vào bảng |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 30 phút/bài

[1 Tìm + tải: ?'] → [2 Đọc lướt: ?']
→ [3 Đọc kỹ phương pháp: ?'] ← BOTTLENECK
→ [4 Đọc thực nghiệm, ghi số liệu: ?'] ← BOTTLENECK
→ [5 Ghi vào bảng so sánh: ?'] → [6 Tra lại khi viết: 2–3 lần mở lại bài]
```

### Card muốn pitch nhất

- Card số: 1 (LênSàn)
- Vì sao: việc lặp lại theo SKU × sàn nên đo được rõ; câu "AI sai kiểu nào tệ hơn" có câu trả lời rõ: bỏ sót một câu vi phạm (listing bị đình chỉ) tệ hơn báo nhầm (người review mất thêm vài giây)
- Câu hỏi muốn nhóm phản biện: Template tiêu đề + file đăng hàng loạt + phần mềm đa kênh có sẵn đã đủ chưa? Nếu đủ, bài này chỉ cần Rule chứ không cần Workflow có AI

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| | | |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

- Thời gian chờ khám ngoại trú tại Bệnh viện Lê Văn Việt (255 người bệnh), Tạp chí Khoa học ĐH Nguyễn Tất Thành: https://jst.ntt.edu.vn/index.php/jst/article/download/606/541/2177
- VietnamWorks HR Insider, thời gian nhà tuyển dụng đọc CV: https://www.vietnamworks.com/hrinsider/ky-nang-doc-vi-cv-nhan-dien-nhan-tai.html
- S. Keshav, "How to Read a Paper": https://www.cs.princeton.edu/courses/archive/fall10/cos597B/papers/howtoread-keshav.pdf
- Prototype LênSàn (dữ liệu mô phỏng): https://github.com/haiquanng/demo
- Ước tính thời gian đăng sản phẩm thủ công (nguồn của bên bán công cụ, chưa kiểm độc lập): https://www.rewarx.com/blogs/aider-for-automated-ecommerce-product-listing-generation-speed-up-your-catalog ; https://closo.co/blogs/crosslisting/shopify-bulk-listing
