# Báo cáo cá nhân — 2A202604072_NguyenKhacBao

> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).

## 1. Thông tin học viên

- Họ tên: Nguyễn Khắc Bào
- MSSV: 2A202604072
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhóm 1
- Link repo nhóm: https://github.com/cduyminh/K5-L3B-DAY02-Nhom1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi nhận bản vẽ/đặc tả nội thất (PDF scan, Excel tự do) từ khách hàng/KTS, tôi muốn trích xuất đúng danh mục vật tư và định mức, để lập bảng dự toán BOM báo giá không bị sót linh kiện. | Chủ xưởng, kỹ sư báo giá | ~120'/hồ sơ 10–15 hạng mục (`TB-DUOI-PM` có 11 vật tư), 3–4 hồ sơ/tuần. |
| 2 | Pain từ người khác | Khi người dùng xưởng hoặc tester báo lỗi với mô tả mơ hồ (thiếu bước tái hiện, màn hình, log), tôi muốn gom đủ ngữ cảnh và đối chiếu spec ngay lần đầu, để khoanh vùng lỗi không phải hỏi lại nhiều vòng. | Dev bảo trì FurniCore, tester, chủ xưởng | Đợt test `001-app-shell` (`claude-desktop-tests.md`) có 9 góp ý cần đối chiếu 40+ FR trong `spec.md`; mất ~55'/ca + chờ 2–4h hỏi lại bối cảnh/log. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi kết thúc một phiên dev hoặc test thủ công trên FurniCore, tôi muốn tổng hợp việc còn mở, lỗi đã sửa và bẫy kỹ thuật từ các checklist, để phiên sau làm tiếp ngay không phải rà lại lịch sử. | Lập trình viên phát triển liên phiên | 3–4 lần/tuần; mất 30–45'/lần đọc chéo `tasks.md`, `release.md`, `claude-desktop-tests.md` (370 dòng) và `git log` để cập nhật `SESSION_HANDOFF.md` (252 dòng). |
| 4 | Lặp lại | Khi khách chuyển khoản tiền cọc (40%) hoặc nghiệm thu (60%) qua mã VietQR của xưởng, tôi muốn đối chiếu nhanh giao dịch ngân hàng với mã đơn và đợt trả, để gạch nợ chính xác không sót hay nhầm công nợ. | Chủ xưởng, thu ngân/kế toán xưởng | 15–25 giao dịch/tuần (`HD-2610-001`, nội dung `Thanh toan {MA_DON}` tối đa 25 ký tự ở `spec.md` FR-025); mất ~30'/ngày dò tay khi khách gõ sai mã đơn. |
| 5 | Tốn thời gian | Khi chốt đơn tủ bếp/nội thất sản xuất theo đơn (MTO), tôi muốn bóc tách tổng vật tư so với tồn kho và xuất riêng hóa đơn khách lẫn phiếu xuất xưởng, để đủ vật tư gia công mà không lộ công thức BOM. | Chủ xưởng, thủ kho, thợ xưởng | Đơn 3–4 hạng mục (6–11 vật tư/món theo `DESKTOP_SALES_SPEC.md`) mất 25–35'/đơn nhân tay kiểm kho + tách 2 mẫu in; 1–2 lần/tuần thiếu ván Pima/MDF đột xuất. |

**Nếu có dùng AI để gợi ý thêm:**

- Tự scan các pain thực tế từ quá trình xây dựng app nội thất trước, sau đó nhờ AI rà lại theo 4 lăng kính. Giữ lại các ý có input/output đo được (#1, #2, #4).

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Bóc tách & đối soát bảng BOM nội thất (#1) | Thiệt hại đo bằng tiền trực tiếp nếu báo giá sai, quy trình 5 bước rõ, có số liệu đối chứng thật từ người dùng test. | Tỷ lệ bản vẽ khách gửi dạng PDF scan mờ/viết tay thực tế chiếm bao nhiêu %? |
| 2 | Đối chiếu chuyển khoản VietQR & gạch nợ công nợ (#4) | Lặp lại hằng ngày ở xưởng, tách biệt rõ mức Rule (regex mã đơn) với Workflow (xử lý ca gõ sai/người thân chuyển hộ). | Xưởng nhỏ có xuất được file sao kê CSV/Excel từ app ngân hàng để chạy đối chiếu local không? |
| 3 | Chuẩn hóa phản hồi lỗi xưởng/tester & đối chiếu log (#2) | Tốn nhiều thời gian chờ hỏi qua lại; có sẵn 9 feedback thật từ `claude-desktop-tests.md` và cơ chế log local (`FR-038`). | Người dùng xưởng có chịu bấm nút xuất gói log trong app thay vì chỉ chụp Zalo gửi sang không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận bản vẽ/đặc tả nội thất (PDF scan, Excel tự do) từ khách hàng/KTS, tôi muốn trích xuất đúng danh mục vật tư (ván Pima, MDF, bản lề, ray trượt) và giá vốn chuẩn, để lập bảng dự toán BOM báo giá không bị sót linh kiện hay lỗ chi phí. |
| Actor | Chủ xưởng nội thất / Kỹ sư dự toán báo giá. |
| Thời điểm / bối cảnh | Khi nhận yêu cầu báo giá tủ bếp/nội thất mới (hẹn phản hồi trong 24–48h) hoặc nhập định mức BOM vào phần mềm xưởng (feature `002` FurniCore). |
| Quy trình hiện tại (3–7 bước) | 1. Mở file PDF/Excel khách gửi (10') · 2. Đọc & đánh dấu tay từng vật tư cấu thành (20') · 3. Gõ mã vật tư, ĐVT (`md`, `tấm`, `bộ`), định mức vào bảng BOM (50') · 4. Tra giá nhà cung cấp để cộng giá vốn (15') · 5. Nhờ đồng nghiệp rà soát chéo từng dòng (25'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3 (nhập tay định mức: 50') và Bước 5 (rà soát chéo chờ người: 25') — dễ gõ nhầm hoặc lệch giá vốn. |
| Impact (nếu không giải thì sao) | Tốn 6–8h/tuần (3–4 hồ sơ); sai số lượng/giá vốn (lệch ~190k–400k/md) gây trượt thầu nếu đội giá hoặc lỗ trực tiếp khi sản xuất. |
| Success metric (baseline → target) | Thời gian lập bảng BOM: `120'` → `≤ 20'`/hồ sơ; tỷ lệ dòng sai số lượng/giá vốn: `~8%` → `< 0,5%`. |
| Phương án không dùng AI | Template Excel chuẩn bắt khách/KTS điền sẵn + Rule tự cộng giá vốn BOM (chặn lệch số nguyên). Hạn chế: không đọc được PDF scan hay Excel tự do. |
| Giả thuyết về AI (nếu có) | OCR + LLM bóc tách bảng từ PDF/Excel tự do thành JSON chuẩn, gợi ý map danh mục vật tư xưởng và gắn cờ ô độ tin cậy thấp để người duyệt. |
| Cảm nhận nhanh | Workflow (AI bóc tách + map gợi ý; Rule tính tổng giá vốn; người duyệt lưu). |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 120 phút/hồ sơ

[1 Mở file PDF/Excel: 10'] → [2 Đọc & đánh dấu tay: 20'] → [3 Nhập tay BOM: 50'] ← BOTTLENECK CHÍNH
→ [4 Tra giá & cộng giá vốn: 15'] → [5 Rà soát chéo: 25'] ← BOTTLENECK PHỤ
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách chuyển khoản tiền cọc (40%) hoặc nghiệm thu (60%) qua mã VietQR của xưởng, tôi muốn đối chiếu nhanh giao dịch ngân hàng với đúng mã đơn hàng và đợt thanh toán, để gạch nợ chính xác mà không bỏ sót hay nhầm công nợ. |
| Actor | Chủ xưởng nội thất / Thu ngân xưởng. |
| Thời điểm / bối cảnh | Cuối ngày hoặc trước khi giao hàng lắp đặt (cần xác nhận khách đã chuyển đủ đợt cọc 40% hoặc 60% còn lại theo `DESKTOP_SALES_SPEC.md`). |
| Quy trình hiện tại (3–7 bước) | 1. Mở app ngân hàng lọc giao dịch tiền vào trong ngày (3') · 2. Đọc nội dung CK dò khớp mã đơn `HD-2610-001` trong sổ/app (12') · 3. Nhắn hỏi khách/sale khi thiếu mã đơn hoặc CK từ TK người thân (10') · 4. Cập nhật đã thu tiền đợt và lưu ảnh sao kê (5'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 & 3 (22'/ngày): dò tay nội dung CK bị cắt/sai cú pháp (`Thanh toan {MA_DON}` giới hạn 25 ký tự ở `spec.md` FR-025) và nhắn xác minh chủ tài khoản chuyển hộ. |
| Impact (nếu không giải thì sao) | Mất ~2,5–3h/tuần đối soát (15–25 giao dịch/tuần); gạch nhầm đợt hoặc sót khoản cọc dẫn đến giao hàng trễ hoặc nhầm công nợ khách. |
| Success metric (baseline → target) | Thời gian đối soát mỗi ngày: `30'` → `≤ 5'`; tỷ lệ giao dịch phải nhắn hỏi lại khách: `~25%` → `< 5%`. |
| Phương án không dùng AI | Rule/Regex đọc file sao kê CSV/Excel ngân hàng, tự động khớp đúng chuỗi `{MA_DON}` (`HD-xxxx-xxx`) và khớp chính xác số tiền đợt 40%/60% theo dữ liệu đơn. |
| Giả thuyết về AI (nếu có) | Sau bước Rule, LLM gợi ý ghép cặp (fuzzy match) các giao dịch ngoại lệ (viết tắt tên khách, sai 1–2 ký tự mã đơn, trùng số tiền lẻ) kèm mức độ tin cậy để chủ xưởng xác nhận 1 chạm. |
| Cảm nhận nhanh | Rule / Workflow (Rule khớp giao dịch chuẩn; AI gợi ý ca mơ hồ; con người bấm duyệt gạch nợ). |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 30 phút/ngày (15–25 giao dịch/tuần)

[1 Lọc GD ngân hàng: 3'] → [2 Dò tay mã đơn: 12'] ← BOTTLENECK CHÍNH
→ [3 Hỏi lại ca thiếu mã/CK hộ: 10'] ← BOTTLENECK PHỤ → [4 Gạch nợ công nợ: 5']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi người dùng xưởng hoặc tester gửi phản hồi lỗi với mô tả mơ hồ (thiếu bước tái hiện, màn hình, mức zoom, log), tôi muốn gom đủ ngữ cảnh kỹ thuật và đối chiếu đúng FR trong `spec.md` ngay từ đầu, để khoanh vùng sửa lỗi nhanh mà không hỏi lại nhiều vòng. |
| Actor | Lập trình viên bảo trì app FurniCore (và chủ xưởng / tester báo lỗi). |
| Thời điểm / bối cảnh | Trong và sau các phiên test thủ công (`CD-01`–`CD-12` trong `claude-desktop-tests.md`) hoặc khi xưởng dùng bản cài thử nghiệm gặp sự cố. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc mô tả/ảnh lỗi thô từ người dùng (5') · 2. Nhắn hỏi lại màn hình đang mở, mức zoom/kích thước cửa sổ và xin file log (20' + chờ 2–4h) · 3. Tìm dòng `WARN`/`ERROR` trong `logs/furnicore.*.log` (10') · 4. Đối chiếu 40+ FR trong `spec.md` để phân biệt lỗi code hay thiếu spec (15') · 5. Chốt phiếu lỗi có bước tái hiện (5'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 (hỏi lại bối cảnh & log: 20' thao tác + 2–4h chờ) và Bước 4 (đối chiếu thủ công với `spec.md`: 15'). |
| Impact (nếu không giải thì sao) | Vòng xử lý 1 lỗi kéo dài nửa ngày; dễ đánh giá sai mức độ lỗi (như vụ `Ctrl+R` ở đợt `KL-01` làm mất nháp Cài đặt nặng hơn mô tả ban đầu, hay `CD-07`/`CD-08` tắc vì thiếu log). |
| Success metric (baseline → target) | Thời gian khoanh vùng lỗi: `55'` (+ chờ 2–4h) → `≤ 15'`; tỷ lệ ca lỗi phải hỏi bổ sung vòng 2: `~60%` → `< 15%`. |
| Phương án không dùng AI | Thêm nút "Xuất gói chẩn đoán" trong *Thông tin ứng dụng* để gom phiên bản app, kích thước cửa sổ, mức zoom và 200 dòng log cuối (đã ẩn PII) + checklist 3 câu ngắn. Hạn chế: người dùng ít điền đủ mô tả và dev vẫn tự đối chiếu spec. |
| Giả thuyết về AI (nếu có) | Kết hợp nút xuất gói chẩn đoán (Rule) với LLM đọc mô tả lỗi + log sạch để tóm tắt bước tái hiện nháp, gợi ý câu hỏi còn thiếu và chỉ ra FR liên quan trong `spec.md`. |
| Cảm nhận nhanh | Rule / Workflow (Rule gom log + trạng thái máy; AI chuẩn hóa & map FR; dev kiểm chứng trước khi sửa). |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 55 phút thao tác/ca lỗi (+ 2–4h chờ phản hồi)

[1 Đọc mô tả/ảnh lỗi: 5'] → [2 Hỏi lại bối cảnh & xin log: 20' (+2–4h chờ)] ← BOTTLENECK CHÍNH
→ [3 Đọc log WARN/ERROR: 10'] → [4 Đối chiếu spec.md: 15'] ← BOTTLENECK PHỤ → [5 Chốt ticket: 5']
```

### Card muốn pitch nhất

- Card số: 1 (Bóc tách & đối soát bảng BOM nội thất)
- Vì sao: Impact đo thẳng bằng tiền (tránh lệch giá vốn `190k–400k/md`), quy trình 5 bước và input/output sắc nét, dễ tách rạch ròi phần Rule (tính giá vốn số nguyên) với phần AI (bóc tách PDF/Excel tự do).
- Câu hỏi muốn nhóm phản biện: *"Nếu khách gửi bản vẽ PDF scan mờ hoặc ghi tên vật tư không chuẩn (ví dụ 'nhựa đặc 18' thay vì 'Tấm Pima 18mm SP028'), nên đặt điểm fallback về nhập tay ở đâu để không sai giá vốn BOM?"*

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Map tên vật tư phi chuẩn sang mã nội bộ dễ bị bịa (hallucination), gây báo giá sai. | Đồng ý | Đặt boundary HITL: AI chỉ gợi ý top-3 mã kèm cờ cảnh báo, người dùng bắt buộc chọn xác nhận trước khi Rule tính giá vốn. |
| Sơ đồ nháp Card #1 thiếu số phút cho bước rà soát chéo và chưa khớp tổng `120'`. | Đồng ý | Đồng bộ đủ 5 bước có số phút cho cả 3 sơ đồ (`10+20+50+15+25 = 120'` ở Card #1). |
| Card #2, #3 dễ sa vào làm chatbot trước khi kiểm tra Rule đã đủ chưa. | Đồng ý một phần | Bổ sung phương án Rule rõ ràng trước khi lên Workflow (regex sao kê CSV ở Card #2; nút xuất gói chẩn đoán log ở Card #3). |

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
| CP1 Scan | Rà lại danh sách vấn đề đã tự scan theo 4 lăng kính và chuẩn hóa Job Story. | Gom đúng 4 lăng kính, lọc các bài toán đo được thời gian/lỗi. | Gợi ý các ý ngoài phạm vi MVP (nesting CNC, thiết kế 3D) và thiếu số liệu thật. | Bỏ các ý lệch `constitution.md`; đối chiếu `furnicore` điền số liệu thật cho 5 dòng. |
| CP2 Problem Card | Đóng vai PM hoài nghi phản biện 3 Problem Cards và kiểm sơ đồ quy trình. | Chỉ ra rủi ro bịa mã vật tư BOM và điểm thiếu nhất quán số phút ở Card #1. | Ban đầu thiên về Workflow/chatbot ở Card #2, #3 mà bỏ qua Rule. | Thêm boundary người duyệt chốt số, sửa số phút khớp 100%, bổ sung Rule làm mốc so sánh. |
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

-
