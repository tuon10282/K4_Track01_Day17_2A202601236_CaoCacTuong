# Chặng 1 — Đặt giả thuyết · Checkpoint 1 (CP1)

**Track 1 - Day 17 — Finding and Validating Pain Points**  
**Case đã chọn:** Case A — AI Tutor: Diagnostic Refresher  
**Người thực hiện Checkpoint 1:** Đinh Lê Quỳnh Phương (MSSV: 2A202601865)  
**Thành viên nhóm:** Đinh Lê Quỳnh Phương (2A202601865) · Cao Các Tường (2A202601236)  

---

## 1. Solution — Gỡ solution khỏi hình thức cụ thể

**Case đã chọn:** Case A — AI Tutor: Diagnostic Refresher

**Solution directive:**
> Thêm nút **"Tôi vẫn chưa hiểu"** vào bài học. Khi học viên bấm nút, **AI Tutor** dùng nội dung bài hiện tại, các câu trả lời gần đây và lịch sử học tập để đặt 2–3 câu hỏi chẩn đoán ngắn, chọn một khái niệm nền để ôn lại, tạo một phần giải thích ngắn, rồi đưa học viên trở về bài đang học.

**Capability trung tính:**
> Khi người học bị mắc ở một đoạn trong bài đang học, họ được giúp xác định đúng chỗ hổng kiến thức đang chặn mình và lấp chỗ hổng đó đủ nhanh để quay lại tiếp tục bài học trong cùng phiên học mà không bị mất đà.

---

## 2. Change — Làm lộ chuỗi thay đổi được kỳ vọng

**Chuỗi thay đổi kỳ vọng:**
```
Solution 
  → Learner gọi tên được chỗ hổng cụ thể (thay đổi nhận thức) 
  → Learner dừng lại ôn đúng khái niệm đó rồi quay lại bài (thay đổi hành vi) 
  → Learner tiếp tục hoàn thành bài đang học và các bài phụ thuộc (thay đổi trạng thái) 
  → Outcome: Giảm tỉ lệ bỏ dở ở các bài khó, tăng tỉ lệ hoàn thành khoá học.
```

**Các thay đổi được kỳ vọng:**
1. **Nhận thức:** Chuyển từ *"bài này khó quá / mình không đủ khả năng"* sang *"mình đang hổng khái niệm X, chỉ cần lấp X là đi tiếp được"*.
2. **Hành vi:** Thay vì bỏ qua/tra lan man trên Google, ChatGPT/tắt máy, learner chủ động yêu cầu trợ giúp tại chỗ và ôn ngắn có mục tiêu trong vài phút.
3. **Trạng thái:** Thời gian mắc kẹt giảm từ 20–40 phút xuống vài phút; nợ kiến thức không bị tích luỹ sang bài sau.

---

## 3. Actor — Xác định các nhóm người có liên quan *(Phương chủ trì)*

| Actor | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Họ hưởng lợi thế nào? |
|---|---|---|---|
| **Learner tự học (self-paced)** *(bấm nút)* | Học bài theo lộ trình một mình, xem video, làm quiz | Mắc kẹt không biết thiếu gì; tra lan man; nản lòng và bỏ khoá | Đi tiếp được ngay trong phiên học mà không mất đà |
| **Instructor / Giảng viên** | Soạn bài, theo dõi tiến độ lớp | Không biết learner mắc ở đâu; nhận câu hỏi nền lặp đi lặp lại | Thấy được chỗ hổng phổ biến để cải thiện nội dung bài |
| **Trợ giảng / Coach** | Hỗ trợ 1-1 cho học viên | Tốn thời gian dò lại từ đầu xem learner đang hổng kiến thức gì | Nhận yêu cầu trợ giúp đã gom sẵn chỗ hổng cụ thể |

* **Actor nhóm chọn để điều tra trước:** Learner tự học (self-paced), đang học khoá học có tính tích luỹ (bài sau dựa trên bài trước) và trong 7 ngày gần đây từng gặp khó khăn khi học.
* **Vì sao chọn nhánh này thay vì actor khác:** Learner vừa là người trực tiếp trải nghiệm pain ngay tại thời điểm mắc kẹt, vừa là người **phải thay đổi hành vi** (báo mắc kẹt) để outcome xảy ra. Đây là nhánh rẻ nhất và nhanh nhất để kiểm chứng hoặc bác bỏ giả thuyết.

---

## 4. Situation & Job — User đang cố làm gì trong tình huống nào? *(Phương chủ trì)*

* **Mô tả Situation & Job:**
  > Khi **đang học một bài mới và trả lời sai quiz / đọc lại một đoạn nhiều lần mà vẫn không hiểu**, **learner tự học** đang cố **hiểu đủ đoạn đang mắc để tiếp tục bài học trong phiên hôm nay** bằng cách **đọc lại, tua video, tự tra Google/ChatGPT bằng từ khoá đoán, hoặc bỏ qua học tiếp**.

* **JTBD Hypothesis:**
  > Khi **mắc ở một đoạn trong bài đang học và không chắc mình đang thiếu kiến thức nền nào**, tôi muốn **xác định và lấp đúng chỗ hổng đó thật nhanh**, để có thể **tiếp tục bài học ngay trong phiên này mà không mất đà và không phải quay lại học lại từ đầu**.

---

## 5. Pain — Viết các cách giải thích cạnh tranh

* **Pain Hypothesis A (Diagnosis gap):**
  > Khi **mắc ở một đoạn trong bài đang học**, **learner tự học** gặp khó khăn trong việc **hiểu đủ để đi tiếp** vì **họ không xác định được mình đang thiếu khái niệm nền nào (không biết mình không biết gì)**, dẫn đến **tra cứu lan man 20–40 phút rồi hiểu lệch, hoặc bỏ qua và tích luỹ nợ kiến thức, cuối cùng bỏ dở khoá học**.

* **Pain Hypothesis B — Cách giải thích cạnh tranh (Momentum/Cost gap) *(Phương chủ trì)*:**
  > Khi **mắc ở một đoạn trong bài đang học**, **learner tự học** gặp khó khăn trong việc **hiểu đủ để đi tiếp** vì **việc rời khỏi bài để ôn nền tốn quá nhiều thời gian và làm mất đà**, dẫn đến **họ chủ động bỏ qua chỗ chưa hiểu dù biết rõ mình hổng ở đâu, học tiếp trong trạng thái hiểu nửa vời và sai lặp lại ở các bài sau**.

* **Giả thuyết nhóm chọn để điều tra trước:** **Pain Hypothesis A**
* **Lý do chọn:** A là mắt xích đắt nhất của directive (nếu learner tự gọi tên được chỗ hổng thì phần AI chẩn đoán mất giá trị); đồng thời A là giả thuyết rẻ nhất để bác bỏ bằng phỏng vấn.

---

## 6. Evidence — Xác định điều cần tìm trước khi viết câu hỏi

| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
|---|---|---|
| **Situation có thật** | Kể được 1 lần cụ thể trong 7 ngày qua (bài nào, lúc nào, đoạn nào). | Không nhớ lần nào cụ thể, chỉ nói chung chung "thỉnh thoảng cũng khó". |
| **Pain có ý nghĩa** | Cảm giác mắc kẹt đi kèm hành động thật (học tới 1h sáng, mất 30+ phút). | "Cũng không sao, đọc tiếp là quen", quên ngay chuyện đó hôm sau. |
| **Workaround tồn tại** | Tra Google/ChatGPT, xem video khác, hỏi bạn (có từ khoá/bằng chứng). | Không làm gì cả, chỉ đọc lại 1 lần rồi đi tiếp và thấy đủ. |
| **Consequence tồn tại** | Hậu quả thật: sai bài sau cùng lý do, nộp bài muộn, điểm quiz thấp. | Không có hậu quả nào, vẫn làm bài tiếp theo bình thường. |
| **Pattern có lặp** | Chuyện xảy ra ≥2–3 lần/tuần hoặc lặp ở nhiều bài khác nhau. | Chỉ xảy ra 1 lần duy nhất do hoàn cảnh riêng (mệt, mất mạng). |

---

## Chốt Problem Hypothesis và park solution

* **Problem Hypothesis nhóm mang sang Chặng 2:**
  > **Khi learner tự học mắc ở một đoạn trong bài đang học (trả lời sai quiz hoặc đọc lại nhiều lần vẫn không hiểu), họ không xác định được mình đang thiếu khái niệm nền nào, nên không biết phải tra cứu hay hỏi cái gì. Kết quả là họ mất 20–40 phút tra cứu lan man rồi hiểu lệch, hoặc bỏ qua và học tiếp trong trạng thái hổng — làm các bài phụ thuộc sau đó càng khó và tăng nguy cơ bỏ dở khoá học.**

* **Điều gì phải đúng để giả thuyết đứng vững:**
  1. Learner nhận ra mình chưa hiểu ngay tại thời điểm đó.
  2. Learner không tự gọi tên được khái niệm nền đang thiếu.
  3. Nguyên nhân mắc kẹt thật sự là do thiếu kiến thức nền có trước.
  4. Learner đã bỏ công sức thật để tự xử lý (có workaround).
  5. Việc bỏ qua chỗ hổng để lại hậu quả quan sát được ở bài sau.

* **Điều gì có thể khiến nhóm sửa hoặc bác bỏ giả thuyết:**
  * Learner gọi tên chính xác được chỗ hổng → **Chuyển sang Pain B**.
  * Learner không có workaround và không thấy cần → **Pain không quan trọng (Bác bỏ)**.
  * Bỏ qua mà không có hậu quả nào ở bài sau → **Consequence không tồn tại (Bác bỏ)**.
  * Các câu chuyện tụ lại ở đúng 1–2 bài cụ thể → **Vấn đề do nội dung bài viết kém (Chuyển sang Pain D)**.

* **Solution Parking Lot:**

| Hướng giải quyết có thể có | AI / Không sử dụng AI |
|---|---|
| 1. Nút "Tôi vẫn chưa hiểu" + AI chẩn đoán & tạo bài ôn ngắn (directive gốc) | AI |
| 2. Overlay chèn sẵn 1–2 khái niệm nền tĩnh do giảng viên gắn tại từng đoạn | Không sử dụng AI |
| 3. Readiness check 3 câu hỏi trước khi vào bài dựa trên bảng điều kiện | Không sử dụng AI |
| 4. "Sổ chỗ chưa hiểu": learner đánh dấu chỗ mắc để gom lại ôn cuối phiên | Không sử dụng AI |
| 5. Hệ thống tự phát hiện dấu hiệu mắc kẹt từ log hành vi (tua lại nhiều lần, đứng yên lâu) | AI |

---

## 🛑 CHECKPOINT 1 — Problem Hypothesis (Tự kiểm)

- [x] Lần theo được đủ chuỗi **Solution → Change → Actor → Situation & Job → Pain → Evidence**.
- [x] Solution đã được gỡ khỏi hình thức cụ thể thành **capability trung tính**.
- [x] Chuỗi Change phân biệt rõ **Output và Outcome**.
- [x] Nêu rõ **Actor chọn điều tra trước** và giải thích lý do lựa chọn.
- [x] Situation là **khoảnh khắc cụ thể**, Job tồn tại độc lập với AI và feature.
- [x] Pain được phát biểu dưới dạng **Barrier + Consequence**.
- [x] Nêu rõ **2 cách giải thích cạnh tranh (A vs B)** và tiêu chí làm giả thuyết bị bác bỏ.
- [x] **Solution Parking Lot** có đủ các hướng sử dụng AI và không sử dụng AI.
