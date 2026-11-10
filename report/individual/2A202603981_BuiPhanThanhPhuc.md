# Báo cáo cá nhân — 2A202603981_BuiPhanThanhPhuc

## 1. Thông tin học viên

- Họ tên: Bùi Phan Thanh Phúc
- MSSV: 2A202603981
- Email trường (không bắt buộc):
- Tên nhóm: Nhóm 1
- Link repo nhóm: https://github.com/cduyminh/K5-L3B-DAY02-Nhom1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

|   # | Lăng kính                         | Job Story: Khi… tôi muốn… để…                                                                                               | Ai chịu ảnh hưởng? | Dấu hiệu thật                                                                                                                          |
| --: | --------------------------------- | --------------------------------------------------------------------------------------------------------------------------- | ------------------ | -------------------------------------------------------------------------------------------------------------------------------------- |
|   1 | Cần đọc, tổng hợp nhiều thông tin | Khi cần mua một món trên Shopee (ví dụ khăn), tôi muốn biết shop nào đáng mua nhất, để không mua nhầm hàng kém hoặc giá cao | Tôi                | Khoảng 30 phút đến 1h. Khoảng 2,3 lần/tháng. |
|   2 | Tốn thời gian                     | Khi vừa họp nhóm xong, tôi muốn có danh sách việc, người phụ trách và hạn, để không ai bỏ sót                               | Cả nhóm (4 người)  | Họp 1 buổi/tuần, viết lại ghi chú khoảng 30'/buổi            |
|   3 | Lặp lại                           | Khi tới hạn nộp lab, tôi muốn có sẵn khung báo cáo đúng format, để không dựng lại từ đầu                                    | Tôi                | Khoảng 20'/lab, 1 lần/tuần.                                                                   |
|   4 | Pain từ người khác                | Khi người thân cần mua một món online, họ muốn có người chọn hộ shop đáng tin, để không mua nhầm                            | Mẹ tôi, tôi        | Mẹ nhờ chọn hộ khoảng 2 lần/tháng, khoảng 30'/lần.                                                                   |
|   5 | Cần đọc, tổng hợp nhiều thông tin | Khi phải đọc tài liệu dài của khóa, tôi muốn nắm nhanh phần liên quan tới lab, để không phải lục lại từng phần              | Tôi                | Khoảng 45'/lần, 2 lần/tuần                                                                                   |

**Nếu có dùng AI để gợi ý thêm:**

- Giữ lại: dòng 2–5 do AI gợi ý, vì chúng đủ 4 lăng kính và tôi cũng gặp thật.
- Bỏ: mua đồ trên Facebook và đặt đồ ăn, vì tần suất thấp hơn Shopee và quy trình khó đo hơn.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem                | Vì sao chọn                                        | Điều còn chưa chắc                                   |
| ---: | ---------------------- | -------------------------------------------------- | ---------------------------------------------------- |
|    1 | Mua đồ Shopee (#1)     | Quy trình rõ | Sàn đã có lọc sao và tóm tắt đánh giá: còn thiếu gì? |
|    2 | Việc sau họp nhóm (#2) | Cả nhóm bị ảnh hưởng       | Chỉ 1 lần/tuần, impact có đủ lớn không?              |
|    3 | Đọc tài liệu dài (#5)  | Gặp thường xuyên khi làm lab                       | "Nắm nhanh" đo thế nào?                              |

### Problem Card #1

| Trường                        | Nội dung                                                                                                       |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Job Story                     | Khi cần mua một món trên Shopee, tôi muốn biết shop nào đáng mua nhất, để không mua nhầm hàng kém hoặc giá cao |
| Actor                         | Tôi, người mua cá nhân                                                                                         |
| Thời điểm / bối cảnh          | Khi cần mua một món có nhiều shop bán cùng loại (ví dụ khăn)                                                   |
| Quy trình hiện tại (3–7 bước) | 1 Tìm từ khóa · 2 Mở nhiều shop cùng loại · 3 Đọc đánh giá từng shop · 4 So giá + phí ship · 5 Chọn, đặt       |
| Bottleneck                    | Bước 3, đọc đánh giá từng shop: 20' đến 50' trên tổng 30' đến 60'/lần                                          |
| Impact                        | Khoảng 50'-120'/tháng.                                         |
| Success metric                | Baseline 30'-60'/lần → target 15'-30'/lần (≤50%)                                             |
| Phương án không dùng AI       | Lọc theo sao + số đơn đã bán; checklist                                                                    |
| Giả thuyết về AI              | Dùng tóm tắt đánh giá có sẵn của sàn để tham khảo, người quyết định                                            |
| Cảm nhận nhanh                | Rule                                                                                                           |

Quy trình nháp hiện tại:

```text
[1 Tìm từ khóa] → [2 Mở nhiều shop] → [3 Đọc đánh giá từng shop: 20'-50'] ← BOTTLENECK
→ [4 So giá + ship] → [5 Chọn, đặt]   Tổng: 30'-60'/lần
```

### Problem Card #2

| Trường                        | Nội dung                                                                                                                 |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Job Story                     | Khi vừa họp nhóm xong, tôi muốn có danh sách việc, người phụ trách và hạn, để không ai bỏ sót                            |
| Actor                         | Thành viên nhóm ghi chú sau họp                                                                                          |
| Thời điểm / bối cảnh          | Ngay sau mỗi buổi họp nhóm lab                                                                                           |
| Quy trình hiện tại (3–7 bước) | 1 Nhớ lại nội dung họp · 2 Tách việc cụ thể từ ghi chú · 3 Gán người + hạn · 4 Viết lại gửi nhóm · 5 Nhắc người chưa làm |
| Bottleneck                    | Bước 2, tách việc từ ghi chú lộn xộn: 10' trên tổng 30'                                                                  |
| Impact                        | 30'/buổi.                                                       |
| Success metric                | Baseline 30'/buổi → target 15'.                                                         |
| Phương án không dùng AI       | Mẫu biên bản có cột Việc / Người / Hạn, điền ngay trong họp                                                              |
| Giả thuyết về AI              | Nháp danh sách việc từ ghi chú họp, người duyệt trước khi gửi                                                            |
| Cảm nhận nhanh                | Workflow                                                                                                                 |

```text
[1 Nhớ lại nội dung họp: 5'] → [2 Tách việc cụ thể: 10'] ← BOTTLENECK → [3 Gán người + hạn: 5']
→ [4 Viết lại gửi nhóm: 7'] → [5 Nhắc người chưa làm: 3']   Tổng: 30'
```

### Problem Card #3

| Trường                        | Nội dung                                                                                                       |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------- |
| Job Story                     | Khi phải đọc tài liệu dài của khóa, tôi muốn nắm nhanh phần liên quan tới lab, để không phải lục lại từng phần |
| Actor                         | Tôi, học viên làm lab                                                                                          |
| Thời điểm / bối cảnh          | Trước và trong lúc làm lab                                                                                     |
| Quy trình hiện tại (3–7 bước) | 1 Mở tài liệu · 2 Đọc lướt toàn bộ · 3 Tìm phần liên quan tới lab · 4 Ghi ý cần dùng · 5 Quay lại tra khi làm  |
| Bottleneck                    | Bước 3, tìm phần liên quan tới lab: 20' trên tổng 45'                                                          |
| Impact                        | 45'/lần, 2 lần/tuần, khoảng 90'/tuần                                                                           |
| Success metric                | Baseline 45' → target 20', tìm được đoạn liên quan trong ≤10'. Đo bằng tự bấm giờ                              |
| Phương án không dùng AI       | Đọc mục lục + tìm từ khóa của đề lab                                                                           |
| Giả thuyết về AI              | Tóm tắt phần liên quan tới đề lab, người kiểm tra lại                                                          |
| Cảm nhận nhanh                | Workflow                                                                                                       |

```text
[1 Mở tài liệu: 2'] → [2 Đọc lướt toàn bộ: 15'] → [3 Tìm phần liên quan lab: 20'] ← BOTTLENECK
→ [4 Ghi ý cần dùng: 5'] → [5 Quay lại tra khi làm: 3']   Tổng: 45'
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: quy trình rõ nhất
- Câu hỏi muốn nhóm phản biện: Nếu sàn đã có sẵn tóm tắt đánh giá, bài này còn đáng làm không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra                                           | Đồng ý?         | Đã sửa gì                                                                                                                |
| ------------------------------------------------------------ | --------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Sàn đã có lọc sao, số đơn và tóm tắt đánh giá: còn thiếu gì? | Đồng ý một phần | Mở thử app: tóm tắt chỉ cho từng sản phẩm, không so được giữa các shop. Tôi thu hẹp vấn đề thành "so sánh giữa các shop" |
| Chưa có baseline đo thật                                     | Đồng ý          | Hiện chỉ ước chừng 30'-60'/lần. Sẽ bấm giờ 5 lần mua để có baseline thật                                                   |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì?                                                                                         | Kết quả / ảnh hưởng tới bài nhóm                                                                   |
| -------------------------- | ------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------- |
| Pitch Problem Card | Thêm 3 Problem Card của tôi vào bảng pitch (`group_report.md` 2.1) | Card của tôi nằm trong 12 candidate để nhóm gom cluster và chấm điểm |
| Phản biện bài của bạn khác | Đặt câu hỏi phản biện trên Google Form. Câu hỏi tôi đã đặt: 〔câu hỏi cụ thể〕 | 〔ảnh hưởng tới bài nhóm〕 |
| Nhận phản biện | Câu hỏi tôi nhận được: 〔câu hỏi〕 | Tôi đã sửa gì: 〔sửa gì〕 |
| Gom cluster / cây OST | Không phụ trách (Minh làm, mục 2.2–2.3) | — |
| Chọn candidate problem | Chấm 7 tiêu chí cho các candidate trên Google Form (mục 2.4) | Điểm của tôi nằm trong bảng chấm điểm nhóm dùng để chọn candidate #4 |
| Kiểm chứng / research | Không phụ trách (Quân, CP4) | — |
| Quy trình nhóm | Không phụ trách (Bảo, CP5) | — |
| Problem Statement | Viết Problem Statement v1 (mục 7) và 5 tiêu chí đánh giá đầu ra của AI | v1 thu hẹp bottleneck về bước viết tiêu đề và mô tả vì BigSeller đã phủ bước điền trường; thêm 2 chỉ số; thêm ngưỡng 0,8 cho ngành hàng. Commit `a1949ae` |
| Mức can thiệp AI | Không phụ trách mục 6 (Minh làm). Ghi mức Workflow và 3 điểm AI can thiệp trong v1 | Mức chọn trong v1: Workflow |
| Quyết định | Không phụ trách (Quân, CP6) | — |

---

## 5. Dùng AI

| Checkpoint                     | Tôi dùng AI để làm gì?                      | AI hữu ích ở đâu?                                        | AI sai hoặc hời hợt ở đâu?                         | Tôi sửa gì bằng nhận định của mình?                             |
| ------------------------------ | ------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------- | --------------------------------------------------------------- |
| CP1 Scan                       | Gợi ý thêm 4 dòng scan                      | Nhắc tôi việc "người thân nhờ chọn hộ", tôi chưa nghĩ ra | Trả lời nhầm câu hỏi về CP1, và số phút do AI đoán | Tôi nói rõ mình cần kiến thức nền; thay số đoán bằng số bấm giờ |
| CP2 Problem Card               | Soạn nháp 3 card, đóng vai "PM hoài nghi"   | Chỉ ra baseline đang dựa vào ước chừng                   | Đoán bước nghẽn của card 2 và 3                    | Giữ bước nghẽn card 1 vì tôi đã đo, sửa card 3                  |
| CP4 Research                   | Soạn câu hỏi Mom Test, tìm giải pháp có sẵn | Tìm ra Shopee đã có tính năng tóm tắt đánh giá bằng AI   | Nguồn là blog bên thứ ba, link chưa kiểm           | Tự mở app Shopee kiểm có hiển thị thật không                    |
| CP5 Quy trình                  | Soạn nháp quy trình trước/sau               | Nhanh, đúng khung                                        | Gộp "đọc đánh giá" và "so giá" thành 1 bước        | Tách lại vì bottleneck nằm ở đọc đánh giá                       |
| CP5–6 Problem Statement        | Soạn nháp v0 và v1                          | Gợi ý thêm metric "số lần mua nhầm không tăng"           | Metric ban đầu chỉ đo thời gian                    | Giữ metric chất lượng ở v1                                      |
| CP6 Mức can thiệp / quyết định | Soạn nháp mức Rule và quyết định Not Yet    | So sánh được 4 mức                                       | Chấm rủi ro Value "Cao" khi chưa có phỏng vấn      | Giữ "Cao" vì thấy hợp lý, ghi rõ lý do                          |

---

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Nghe các bạn pitch, tôi nhận ra phần lớn card đều là việc "đọc rồi tóm lại" hoặc "nhắc việc", giống card của tôi. Lan pitch việc nhắc deadline nhóm, nhưng khi tôi hỏi bạn đo mất bao lâu thì Lan trả lời là ước chừng 20 phút. Điều đó làm tôi thấy card của mình cũng đang dựa nhiều vào ước chừng, nên sau buổi pitch tôi đi bấm giờ lại 3 lần mua.

**6.2. Nhóm có lúc nào bị "solution-first" không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có. Lúc đầu nhóm gọi vấn đề là "cần một công cụ tóm tắt đánh giá Shopee". Khi vẽ cây OST, Minh Anh chỉ ra cụm đó là giải pháp chứ không phải pain, và nhóm gạch nó đi, thay bằng "thông tin đánh giá người bán nằm rải rác, khó so sánh". Sau đó nhóm mới quay lại viết Problem Statement.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Tôi định làm một công cụ tự động tóm tắt đánh giá. Huy hỏi: "Sàn đã có tóm tắt đánh giá rồi, mình làm thêm gì?". Tôi mở thử app, thấy sàn có tóm tắt nhưng chỉ cho từng sản phẩm, không so được giữa các shop. Tôi đổi hướng sang bảng so sánh có ngưỡng lọc cố định và đưa việc đó vào mức Rule.

**6.4. Kết quả kiểm chứng có làm tôi bất ngờ không? Điều gì?**
Có. Tôi tưởng ai cũng mất thời gian ở bước đọc đánh giá. Nhưng anh Đạt nói chỉ nhìn số sao và số đơn là đủ, anh chưa từng mua nhầm. Hai người còn lại mất 20–40 phút. Vì vậy nhóm thêm phương án No AI cho người mua ít và ghi lại đây là tín hiệu phản bác.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là Success Metric. Tôi viết "nhanh hơn" nhưng nhóm yêu cầu có baseline, nên tôi phải bấm giờ thật mới có con số 35 phút. Phần Boundary cũng khó vì tôi phải quyết định rõ công cụ không được làm gì.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, tôi sẽ bấm giờ trước khi pitch thay vì sau. Tôi cũng sẽ phản biện mạnh hơn ở bước chấm điểm: nhóm cho điểm "Pain có bằng chứng" khá cao dù chưa có phỏng vấn, tôi nên hỏi "bằng chứng ở đâu" ngay lúc đó.

**6.7. Hiểu bài:** Vấn đề là khi mua đồ trên Shopee, tôi mất khoảng 35 phút mỗi lần vì phải đọc đánh giá của từng shop, trong đó bước đọc đánh giá chiếm 17 phút. Quy trình có 5 bước và nghẽn ở bước 3. Metric là đưa thời gian xuống ≤50% baseline (≤17 phút) mà số lần mua nhầm không tăng, đo bằng tự bấm giờ. Boundary: công cụ không chọn hay đặt hàng thay tôi, và tôi đọc ít nhất 5 đánh giá thấp sao tận gốc trước khi đặt. Mức can thiệp là Rule: bộ lọc cố định và bảng so sánh, có thể dùng thêm tóm tắt có sẵn của sàn. Quyết định là Not Yet vì chưa đủ baseline từ người khác. Nếu đo xong mà dưới 10 phút mỗi lần thì No-Go và kết luận không cần AI.

---

## 7. Tài liệu tham khảo

- https://www.bigseller.com/blog/articleDetails/3050.htm 
- https://extscope.org/extension/ajalfmcbjjomclnamliamgnohklnfeom 
- https://developer.chrome.com/docs/ai/evaluate-reviews?hl=vi 
