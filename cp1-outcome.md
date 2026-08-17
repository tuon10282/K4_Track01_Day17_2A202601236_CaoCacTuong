# ✅ CP1 — Outcome: Đặt giả thuyết (Tổng hợp cuối)

**Track 1 · Day 17 — Finding and Validating Pain Points**
**Case đã chọn:** Case A — AI Tutor: Diagnostic Refresher
**Nhóm:** Cao Các Tường (2A202601236) · Đinh Lê Quỳnh Phương (2A202601865)
**Ngày:** 17/08/2026
**Trạng thái:** ✅ Chặng 1 hoàn thành — giả thuyết đã được chốt, sẵn sàng sang Chặng 2 (viết interview guide)

> File này là **bản tổng hợp cuối** của Chặng 1, hợp nhất từ `chang-1-dat-gia-thuyet.md` (file gốc),
> `cp1-tuong.md` và `cp1-phuong.md`. Toàn bộ nội dung là **hypothesis**, chưa phải fact về user —
> mọi dòng đều phải có thể bị evidence ở Chặng 3 làm thay đổi.

---

## 1. Solution — Gỡ khỏi hình thức cụ thể

**Solution directive (nguyên văn):**
> Thêm nút **"Tôi vẫn chưa hiểu"** vào bài học. Khi học viên bấm nút, **AI Tutor** dùng nội dung bài
> hiện tại, các câu trả lời gần đây và lịch sử học tập để: (1) đặt 2–3 câu hỏi chẩn đoán ngắn;
> (2) chọn một khái niệm nền để học viên ôn lại; (3) tạo một phần giải thích ngắn; (4) đưa học viên
> trở về bài đang học.

**Capability trung tính** *(không tên nút, không tên feature, không "AI")*:
> Khi người học bị mắc ở một đoạn trong bài đang học, họ được giúp xác định đúng chỗ hổng kiến thức
> đang chặn mình và lấp chỗ hổng đó đủ nhanh để quay lại tiếp tục bài học trong cùng phiên học mà
> không phải học lại từ đầu và không mất đà.

**Ba khả năng con có thể test riêng:** ① Định vị chỗ hổng (biến "không hiểu bài" → "hổng khái niệm X") ·
② Lấp hổng vừa đủ (đúng lượng nội dung nền) · ③ Giữ mạch (quay lại đúng chỗ mắc, không mất ngữ cảnh).

**Giả định ngầm phải kéo ra** (nếu sai, solution đổi hướng):

| # | Giả định ngầm | Nếu sai thì sao? |
|---|---|---|
| A1 | Learner tự nhận biết được mình chưa hiểu | Nút chủ động không bao giờ được bấm |
| A2 | Learner sẵn sàng chủ động yêu cầu trợ giúp | Sợ tốn thời gian/ngại thừa nhận → im lặng bỏ qua |
| A3 | Nguyên nhân không hiểu là thiếu khái niệm nền | Có thể do bài khó, ví dụ kém, thiếu tập trung, thiếu luyện tập |
| A4 | Một phần ôn ngắn là đủ để đi tiếp | Có thể cần luyện tập/áp dụng |
| A5 | Learner muốn quay lại bài ngay | Có thể họ muốn đánh dấu, xử lý sau |
| A6 | Chỗ mắc định vị được từ dữ liệu hệ thống | Nhiều đoạn mắc không để lại dấu vết trong log |

---

## 2. Change — Chuỗi thay đổi được kỳ vọng

```
Solution
  → Learner nhận ra và gọi tên được chỗ hổng cụ thể (thay đổi nhận thức)
  → Learner dừng lại ôn đúng khái niệm đó rồi quay lại bài, thay vì bỏ qua hoặc rời phiên học (thay đổi hành vi)
  → Learner tiếp tục hoàn thành bài đang học và các bài phụ thuộc nó (thay đổi trạng thái)
  → Outcome: giảm bỏ dở tại các bài khó, tăng tỉ lệ hoàn thành khoá và độ tự tin của learner
```

| | Nội dung | Nhóm kiểm soát được? |
|---|---|---|
| **Output** | Cơ chế báo "chưa hiểu", luồng chẩn đoán, đoạn ôn nền, đường quay lại bài | Có |
| **Intermediate outcome** | Learner thực sự bấm/báo khi mắc; đọc và làm phần ôn | Không — phụ thuộc hành vi |
| **Outcome** | Learner đi tiếp được, hoàn thành bài, hiểu chắc hơn, không bỏ khoá | Không — còn yếu tố khác |

> ⚠️ **Mắt xích mong manh nhất:** *learner có chịu dừng lại và báo mình chưa hiểu hay không.* Nếu learner
> vẫn im lặng bỏ qua để "xong bài cho kịp", outcome bằng 0 dù phần chẩn đoán chính xác đến đâu. → **Hành
> vi báo mắc kẹt là đối tượng cần điều tra, không phải chất lượng phần giải thích.**

---

## 3. Actor — Nhóm người có liên quan

| Actor | Đang làm gì? | Pain/hậu quả có thể có | Hưởng lợi thế nào? |
|---|---|---|---|
| **Learner tự học (self-paced)** | Học theo lộ trình một mình, xem video, làm quiz | Mắc kẹt không biết thiếu gì; tra lan man; nản lòng, bỏ khoá | Đi tiếp được ngay trong phiên học, không mất đà |
| **Learner trong lớp có deadline** | Học để kịp bài tập/kiểm tra | Ưu tiên "xong bài" hơn "hiểu bài"; cố tình bỏ qua | Lấp hổng nhanh mà không mất tiến độ |
| **Instructor / Giảng viên** | Soạn bài, theo dõi tiến độ lớp | Không biết learner mắc ở đâu; nhận câu hỏi nền lặp lại | Thấy chỗ hổng phổ biến để sửa nội dung |
| **Trợ giảng / Coach** | Hỗ trợ 1-1 | Tốn thời gian dò lại từ đầu | Nhận yêu cầu đã kèm chỗ hổng cụ thể |
| **Bạn học / Peer** | Học cùng khoá, bị hỏi trong nhóm chat | Mất thời gian giải thích lại; trả lời sai/nửa vời | Ít bị hỏi câu cơ bản |
| **Product / Course team** | Theo dõi hoàn thành, drop-off | Drop-off tập trung ở vài bài khó, không rõ nguyên nhân | Giảm drop-off, dữ liệu cải thiện nội dung |

**Actor chọn điều tra trước:** **Learner tự học (self-paced)**, trong khoá có tính tích luỹ, trong 7
ngày gần đây có lúc không hiểu một phần bài học và phải tìm cách xử lý.

**Vì sao chọn nhánh này:**
- Learner vừa trải pain ngay tại thời điểm mắc kẹt, vừa là người **phải thay đổi hành vi** (mắt xích
  yếu nhất của Change chain nằm ở họ).
- Instructor/trợ giảng có pain thật nhưng là **hệ quả phía sau** — chỉ can thiệp sau khi learner đã mắc.
- Nếu learner không có pain thật, nhánh instructor cũng sụp theo → đây là nhánh **rẻ nhất để bác bỏ**.

> ⚠️ Người nhận feature (learner bấm nút) **chưa chắc** là người sở hữu pain chính — cần kiểm tra ở Chặng
> 2, không được giả định sẵn.

---

## 4. Situation & Job — Khoảnh khắc cụ thể

**Situation:**
> Learner học buổi tối, đang giữa một bài mới trong khoá tích luỹ; làm câu quiz trả lời sai, đọc lại đoạn
> giải thích 2–3 lần mà vẫn không nối được ý; còn ~30 phút và muốn xong bài trong hôm nay.

**JTBD Hypothesis:**
> Khi **tôi mắc ở một đoạn trong bài đang học và không chắc mình đang thiếu kiến thức nền nào**, tôi
> muốn **xác định và lấp đúng chỗ hổng đó thật nhanh**, để có thể **tiếp tục bài học ngay trong phiên
> này mà không mất đà và không phải quay lại học lại từ đầu**.

**Job có tồn tại nếu bỏ AI + feature?** Có — người học đã tự làm việc này từ trước (tra Google, hỏi bạn,
xem lại vở cũ, tìm video khác). Job được phát biểu đúng cao độ, không phải "job dùng feature".

---

## 5. Pain — Hai cách giải thích cạnh tranh

### Pain Hypothesis A — Diagnosis gap *(Tường chủ trì)*

> Khi **mắc ở một đoạn trong bài đang học**, **learner tự học** gặp khó khăn trong việc **hiểu đủ để
> đi tiếp** vì **họ không xác định được mình đang thiếu khái niệm nền nào — không biết mình không biết
> gì, nên không biết phải tra hay hỏi cái gì**, dẫn đến **tra cứu lan man 20–40 phút rồi hiểu lệch,
> hoặc bỏ qua và tích luỹ nợ kiến thức làm các bài sau càng khó, cuối cùng bỏ dở khoá học**.

### Pain Hypothesis B — Momentum / cost gap *(Phương chủ trì)*

> Khi **mắc ở một đoạn trong bài đang học**, **learner tự học** gặp khó khăn trong việc **hiểu đủ để
> đi tiếp** vì **việc rời khỏi bài để ôn lại nền tốn quá nhiều thời gian và làm mất đà — phải mở tab
> khác, mất chỗ đang đọc, sợ không xong bài trong buổi tối hôm nay**, dẫn đến **họ chủ động bỏ qua chỗ
> chưa hiểu dù biết rõ mình hổng ở đâu, học tiếp trong trạng thái hiểu nửa vời và sai lặp lại ở các bài
> sau**.

### Các cách giải thích dự phòng (giữ lại, chưa điều tra vòng đầu)

- **C — Confidence gap:** hiểu nhưng không có gì xác nhận mình hiểu *đúng* → thiếu kiểm chứng.
- **D — Content gap:** mắc do bài giảng nhảy bước/ví dụ kém → phải sửa nội dung bài.
- **E — Practice gap:** thiếu luyện tập, không thiếu lời giải thích.
- **F — Awareness gap:** learner **không nhận ra** mình chưa hiểu → mọi cơ chế chủ động đều thất bại.

### So sánh A vs B — vì sao quan trọng

| | Nếu A đúng | Nếu B đúng |
|---|---|---|
| Learner có gọi tên được chỗ hổng? | Không | Có |
| Lõi giá trị nằm ở | Phần **chẩn đoán** | Phần **giảm chi phí ngắt mạch** |
| Nếu bỏ phần chẩn đoán AI | Solution mất giá trị | Solution vẫn hoạt động |
| Hành vi quan sát được | Tra cứu lan man, nhiều từ khoá, hỏi câu mơ hồ | Bỏ qua có ý thức, đánh dấu "để sau", hỏi câu rất cụ thể |

### Giả thuyết nhóm chọn để điều tra trước: **A**

1. **A là mắt xích đắt nhất của directive** — phần "AI chẩn đoán" chỉ có lý do tồn tại nếu learner không
   tự định vị được chỗ hổng.
2. **A rẻ nhất để bác bỏ** — chỉ cần yêu cầu kể lại lần gần nhất bị mắc và nghe họ có gọi tên được
   khái niệm hổng không.
3. **A và B dẫn tới hai solution hoàn toàn khác nhau** → phải phân biệt trước khi làm bất cứ thứ gì;
   B sẽ được kiểm tra song song bằng cùng bộ câu hỏi.

---

## 6. Evidence — Điều cần tìm trước khi viết câu hỏi

| Cần kiểm tra | Tin hơn nếu | Nghi ngờ / bác bỏ nếu |
|---|---|---|
| **Situation có thật** | Kể được lần cụ thể trong 7 ngày qua: bài, đoạn, thời điểm, trình tự thời gian | Không nhớ lần nào cụ thể; chỉ nói chung chung; được gợi ý mới nhớ |
| **Pain có ý nghĩa** | Cảm giác mắc kẹt gắn với hành động thật (học tới 1h sáng, mất 30+ phút) | "Cũng không sao, học tiếp là quen"; không có hành động đi kèm |
| **Workaround tồn tại** | Kể chuỗi workaround cụ thể: từ khoá, video, hỏi ai, chờ bao lâu; còn bằng chứng (tab, tin nhắn) | Không làm gì và không thấy cần; chỉ "đọc lại rồi đi tiếp" |
| **Consequence tồn tại** | Hậu quả quan sát được: sai bài sau, nộp muộn, học lại chương, điểm quiz thấp, dừng khoá | Không có hậu quả; vẫn xong bài đúng hạn |
| **Pattern có lặp** | ≥2–3 lần/7 ngày hoặc lặp ở nhiều bài/khoá | Chỉ một lần cá biệt; nguyên nhân hoàn cảnh (mệt, mất mạng) |
| **Phân biệt A vs B** | Không gọi tên được khái niệm hổng → **A** | Gọi tên đúng chỗ hổng nhưng "không có thời gian ôn" → **B** |
| **Ai sở hữu pain** | Learner tự phát hiện mình mắc và tự xử lý | Chỉ biết hổng khi điểm thấp/trợ giảng chỉ ra → **F/instructor** |

### Điều phải đúng để giả thuyết đứng vững

1. Learner **nhận ra được** ngay lúc đó là mình chưa hiểu (không tưởng là đã hiểu).
2. Learner **không tự gọi tên được** khái niệm nền đang thiếu — chỗ hổng mơ hồ, không có tên.
3. Nguyên nhân thật sự là **thiếu kiến thức nền có trước**, không phải bài viết tệ/thiếu luyện tập/mất tập trung.
4. Learner **đã bỏ công sức thật** để tự xử lý (có workaround, có thời gian) → có động lực.
5. Bỏ qua chỗ hổng **để lại hậu quả quan sát được** ở bài sau.
6. Tình huống **lặp lại**, không phải một lần cá biệt.
7. Learner **muốn giải quyết ngay trong phiên học**, không muốn ghi lại để xử lý sau.

---

## 7. Chốt Problem Hypothesis

### Problem Hypothesis nhóm mang sang Chặng 2

> **Khi learner tự học mắc ở một đoạn trong bài đang học (trả lời sai quiz hoặc đọc lại nhiều lần vẫn
> không nối được ý), họ không xác định được mình đang thiếu khái niệm nền nào, nên không biết phải tra
> cứu hay hỏi cái gì. Kết quả là họ mất 20–40 phút tra cứu lan man và hiểu lệch, hoặc bỏ qua và học
> tiếp trong trạng thái hổng — làm các bài phụ thuộc sau đó càng khó và tăng nguy cơ bỏ dở khoá học.**

### Điều gì có thể khiến nhóm sửa hoặc bác bỏ giả thuyết

| Tín hiệu từ phỏng vấn | Hành động của nhóm |
|---|---|
| Learner gọi tên được chính xác chỗ hổng | Sửa sang **Pain B** (chi phí ngắt mạch) |
| Không có workaround nào, không thấy cần | **Pain không đủ quan trọng — bác bỏ** |
| Bỏ qua mà không có hậu quả nào ở bài sau | **Consequence không tồn tại — bác bỏ** |
| Chỉ biết mình hổng khi bị điểm thấp/trợ giảng chỉ ra | **Actor & trigger sai — chuyển sang F** |
| Câu chuyện tụ lại ở cùng 1–2 bài cụ thể | **Nguyên nhân là nội dung bài — chuyển sang D** |
| Learner thích ghi lại rồi ôn cuối buổi/cuối tuần | **Giả định "quay lại bài ngay" sai** |

---

## 8. Solution Parking Lot (đã park — không thiết kế ở chặng này)

| # | Hướng giải quyết có thể có | AI / Không AI |
|---|---|---|
| 1 | Nút "Tôi vẫn chưa hiểu" + AI chẩn đoán & tạo phần ôn nền ngắn (directive gốc) | AI |
| 2 | Overlay chèn sẵn 1–2 khái niệm nền tĩnh do giảng viên gắn tại từng đoạn | Không AI |
| 3 | Readiness check 3 câu trước khi vào bài dựa trên bảng prerequisite tĩnh | Không AI |
| 4 | "Sổ chỗ chưa hiểu": highlight đoạn mắc, gom danh sách ôn cuối phiên, đẩy cho trợ giảng | Không AI |
| 5 | Hệ thống phát hiện dấu hiệu mắc kẹt từ log hành vi (tua lại, đứng yên lâu) và đề nghị ôn | AI |
| 6 | Routing tới người: câu hỏi tại đúng đoạn mắc đẩy tới trợ giảng/bạn học, cam kết phản hồi 15 phút | Không AI |
| 7 | Phân tích drop-off theo đoạn rồi sửa nội dung bài: chèn "cầu nối" 60 giây tại chỗ nhiều người mắc | Không AI |

*5/7 hướng không dùng AI — vượt yêu cầu tối thiểu 1 hướng không AI.*

---

## 9. Tiêu chí tuyển người phỏng vấn (đầu vào Chặng 2)

**Screener — chỉ hỏi về quá khứ, không mô tả solution:**
1. Trong 7 ngày qua bạn có học một bài/khoá nào không? Bài gần nhất là hôm nào?
2. Trong 7 ngày qua có lúc nào bạn đọc/xem một phần bài học mà vẫn không hiểu không? Kể ngắn: bài nào?
3. Lúc đó bạn đã làm gì để xử lý? *(Phải có ≥1 hành động thật — nếu "không làm gì" thì xếp nhóm đối chứng.)*

**Loại ra:** người học lý thuyết rời rạc không tích luỹ; không nhớ sự kiện cụ thể; mắc vì hoàn cảnh
(mất mạng, thiếu thời gian). **Nhóm đối chứng:** 1 người "hầu như không bị mắc" để nghe evidence phản bác.

---

## ✅ CHECKPOINT 1 — Problem Hypothesis (validate cuối cùng)

| # | Tiêu chí | Trạng thái |
|---|---|---|
| 1 | Lần theo đủ chuỗi Solution → Change → Actor → Situation & Job → Pain → Evidence | ✅ |
| 2 | Solution gỡ khỏi hình thức cụ thể thành capability trung tính (không tên nút, không tên feature, không "AI") | ✅ |
| 3 | Chuỗi Change rõ mắt xích, phân biệt Output vs Outcome, chỉ ra mắt xích yếu nhất | ✅ |
| 4 | Nhiều actor, người nhận feature ≠ người sở hữu pain chính, lý do chọn learner | ✅ |
| 5 | Situation là khoảnh khắc cụ thể; Job tồn tại khi bỏ AI + feature | ✅ |
| 6 | Pain dạng barrier + consequence, không phải "thiếu feature" | ✅ |
| 7 | Hai cách giải thích cạnh tranh A & B + 4 dự phòng C–F; A/B dẫn tới 2 solution khác nhau | ✅ |
| 8 | Nêu rõ điều gì làm giả thuyết sai (falsifier) | ✅ |
| 9 | Solution đã park: 7 hướng, 5 không dùng AI | ✅ |

**Kết luận:** Chặng 1 đạt Checkpoint 1. Nhóm chọn điều tra **Pain A (Diagnosis gap)** với 4 falsifier,
dự phòng B kiểm tra song song cùng bộ câu hỏi. Đầu ra chuyển sang Chặng 2: viết Conversation Guide
(xem [plan-cp2.md](plan-cp2.md)).

---

## 10. Phân công theo Chặng (đã thực hiện)

| Chặng | Tường | Phương |
|---|---|---|
| 1 · Đặt giả thuyết | Lớp Solution, Change, Evidence; chủ trì Pain A; Parking Lot hướng không AI | Lớp Actor, Situation & Job, Pain; chủ trì Pain B |
| 2 · Chuẩn bị phỏng vấn | Warm-up + khai thác bối cảnh | Deep-dive + đánh giá mức độ ưu tiên pain |
| 3 · Luyện phỏng vấn | Lượt 1 interviewer, lượt 2 đóng user | Lượt 1 đóng user, lượt 2 interviewer |
| 4 · Chỉnh guide & nộp | Rà soát interview guide | Tổng hợp giả thuyết, kiểm tra format, submit |

**Nguồn tham chiếu:** [chang-1-dat-gia-thuyet.md](chang-1-dat-gia-thuyet.md) ·
[cp1-tuong.md](cp1-tuong.md) · [cp1-phuong.md](cp1-phuong.md) · [plan-cp2.md](plan-cp2.md)
