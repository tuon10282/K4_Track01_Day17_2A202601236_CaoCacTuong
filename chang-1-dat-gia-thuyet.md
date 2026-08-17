# Chặng 1 — Đặt giả thuyết (60 phút)

**Track 1 · Day 17 — Finding and Validating Pain Points**
**Case đã chọn:** Case A — AI Tutor: Diagnostic Refresher
**Nhóm:** Cao Các Tường (2A202601236) · Đinh Lê Quỳnh Phương (2A202601865)
**Ngày:** 17/08/2026

> ⚠️ Toàn bộ nội dung trong file này là **hypothesis**, chưa phải fact về user.
> Chưa có dữ liệu phỏng vấn nào ở chặng này. Mọi dòng đều phải có thể bị evidence làm thay đổi.

---

## 0. Phân công task cho 2 người (60 phút)

**Nguyên tắc chia việc:** 15 phút đầu **hai người suy luận độc lập, không dùng AI**, và mỗi người đi
theo **một nhánh actor khác nhau** để nhóm chắc chắn có hai cách giải thích cạnh tranh thật (chứ
không phải hai biến thể của cùng một suy nghĩ). Sau đó mới hợp nhánh và chia lớp để viết cho nhanh.

| Thời lượng | Tường (2A202601236) | Phương (2A202601865) | Sản phẩm ra |
|---|---|---|---|
| 0–15' (không AI) | Tự đi hết chuỗi Solution → Evidence với **nhánh actor = learner tự học (self-paced)** | Tự đi hết chuỗi với **nhánh actor = instructor / trợ giảng** | 2 bản nháp độc lập |
| 15–25' | So nhánh: giữ lại khác biệt, chọn actor điều tra trước, chốt Change chain | So nhánh cùng Tường, ghi lại các điểm chưa thống nhất | Mục 2 + 3 |
| 25–45' | Viết **Lớp 1 (Solution), Lớp 2 (Change), Lớp 6 (Evidence)** | Viết **Lớp 3 (Actor), Lớp 4 (Situation & Job), Lớp 5 (Pain A/B)** | Mục 1–6 |
| 45–55' | Chủ trì **Pain Hypothesis A** (Diagnosis gap) + viết falsifier | Chủ trì **Pain Hypothesis B** (Momentum/cost gap) + viết falsifier | Hai cách giải thích cạnh tranh |
| 55–60' | Review chéo bài của Phương: pain có phải "thiếu feature" không? | Review chéo bài của Tường: outcome có bị nhảy bậc không? | Chốt Problem Hypothesis + Parking Lot |

**Solution Parking Lot:** mỗi người brainstorm tối thiểu 2 hướng, Tường bắt buộc đóng góp ít nhất
1 hướng **không dùng AI**, Phương chốt lại bảng cuối.

**Người giữ vai "phản biện" luân phiên:** ai không viết lớp đó thì có quyền hỏi *"câu này là fact hay
đang là mong đợi của nhóm?"* trước khi lớp đó được chốt.

---

## 1. Solution — Gỡ solution khỏi hình thức cụ thể

### Solution directive (nguyên văn)

> Thêm nút **"Tôi vẫn chưa hiểu"** vào bài học.
> Khi học viên bấm nút, **AI Tutor** sử dụng nội dung bài hiện tại, các câu trả lời gần đây và lịch sử
> học tập để: (1) đặt 2–3 câu hỏi chẩn đoán ngắn; (2) chọn một khái niệm nền để học viên ôn lại;
> (3) tạo một phần giải thích ngắn; (4) đưa học viên trở về bài đang học.

| Thành phần | Solution đã mô tả |
|---|---|
| Trigger | Học viên bấm "Tôi vẫn chưa hiểu" |
| Input | Bài hiện tại, câu trả lời gần đây, lịch sử học tập |
| AI action | Chẩn đoán và lựa chọn khái niệm nền |
| Output | Một phần ôn lại ngắn trước khi quay lại bài hiện tại |
| User control | Học viên chủ động yêu cầu trợ giúp |

### Phần nào trong directive đang mô tả giao diện / tên feature / công nghệ?

- **Giao diện:** "nút", nhãn nút "Tôi vẫn chưa hiểu", "đưa học viên trở về bài đang học" (điều hướng).
- **Tên feature:** "AI Tutor", "Diagnostic Refresher".
- **Công nghệ / cách triển khai:** "AI sử dụng lịch sử học tập để chẩn đoán".
- **Tham số triển khai bị coi như yêu cầu:** con số "2–3 câu hỏi", "một khái niệm nền", "ngắn".

### Capability trung tính (không dùng tên feature)

> **Khi người học bị mắc ở một đoạn trong bài đang học, họ được giúp xác định đúng chỗ hổng kiến
> thức đang chặn mình và lấp chỗ hổng đó đủ nhanh để quay lại tiếp tục bài học trong cùng phiên học,
> mà không phải học lại từ đầu và không mất đà.**

Ba khả năng con, có thể tách rời và test riêng:
1. **Định vị:** biến "em không hiểu bài này" thành "em đang hổng khái niệm X".
2. **Lấp hổng vừa đủ:** cung cấp đúng lượng nội dung nền cần thiết, không phải cả chương.
3. **Giữ mạch:** trở lại đúng chỗ đang mắc mà không mất ngữ cảnh.

### Nhóm có đang mặc định cách triển khai được giao là cách duy nhất không?

Có — và đây là các giả định ngầm bị nén trong directive, phải được kéo ra thành thứ có thể sai:

| # | Giả định ngầm trong directive | Nếu sai thì sao? |
|---|---|---|
| A1 | Learner **tự nhận biết** được mình chưa hiểu | Nếu learner không biết mình đang hổng, nút bấm chủ động sẽ không bao giờ được bấm |
| A2 | Learner **sẵn sàng chủ động** yêu cầu trợ giúp | Tâm lý sợ tốn thời gian / ngại thừa nhận → im lặng bỏ qua |
| A3 | Nguyên nhân không hiểu là **thiếu khái niệm nền** | Có thể do bài giảng viết khó, ví dụ kém, thiếu tập trung, hoặc thiếu luyện tập |
| A4 | Một phần ôn **ngắn** là đủ để đi tiếp | Có thể cần luyện tập/áp dụng, không phải thêm lời giải thích |
| A5 | Learner **muốn quay lại bài ngay** | Có thể họ muốn đánh dấu và học tiếp, xử lý sau |
| A6 | Chỗ mắc **định vị được từ dữ liệu hệ thống** | Nhiều đoạn mắc không để lại dấu vết nào trong log |

---

## 2. Change — Chuỗi thay đổi được kỳ vọng

Không nhảy thẳng từ feature tới outcome. Các mắt xích mà nhóm **đang ngầm tin** sẽ xảy ra:

```
Solution
  → Learner nhận ra và gọi tên được chỗ hổng cụ thể (thay đổi nhận thức)
  → Learner dừng lại ôn đúng khái niệm đó rồi quay lại bài, thay vì bỏ qua hoặc rời phiên học (thay đổi hành vi)
  → Learner tiếp tục hoàn thành bài đang học và các bài phụ thuộc nó (thay đổi trạng thái)
  → Outcome: giảm bỏ dở tại các bài khó, tăng tỉ lệ hoàn thành khoá và độ tự tin của learner
```

### Các thay đổi được kỳ vọng

1. **Nhận thức:** từ *"bài này khó quá / mình không đủ khả năng"* → *"mình đang hổng khái niệm X, chỉ
   cần lấp X là đi tiếp được"*. Đây là thay đổi từ **hổng mơ hồ** sang **hổng có tên**.
2. **Hành vi:** từ *bỏ qua và học tiếp cho xong / tra lan man ở tab khác / hỏi nhóm chat rồi chờ / tắt
   máy* → *yêu cầu trợ giúp ngay tại chỗ và ôn có mục tiêu trong vài phút*.
3. **Trạng thái:** thời gian mắc kẹt giảm từ hàng chục phút (hoặc "không bao giờ giải quyết") xuống
   vài phút; learner không rơi khỏi phiên học; nợ kiến thức không tích luỹ sang bài sau.
4. **Kết quả cuối:** learner hoàn thành bài/khoá nhiều hơn, sai lặp ở các bài phụ thuộc ít hơn, số
   câu hỏi nền tảng lặp lại gửi tới trợ giảng giảm.

### Output vs Outcome

| | Nội dung | Nhóm kiểm soát được? |
|---|---|---|
| **Output** (nhóm tạo ra) | Cơ chế báo "chưa hiểu", luồng chẩn đoán, đoạn ôn nền, đường quay lại bài | Có — làm là có |
| **Intermediate outcome** (chỉ ảnh hưởng) | Learner thực sự bấm/báo khi mắc; learner đọc và làm phần ôn | Không — phụ thuộc hành vi |
| **Outcome** (chỉ ảnh hưởng) | Learner đi tiếp được, hoàn thành bài, hiểu chắc hơn, không bỏ khoá | Không — còn nhiều yếu tố khác |

### Nếu user không thay đổi hành vi, solution còn tạo được outcome không?

**Không.** Mắt xích mong manh nhất của cả chuỗi là *"learner chịu dừng lại và báo mình chưa hiểu"*.
Nếu learner vẫn chọn im lặng bỏ qua để "xong bài cho kịp", thì dù phần chẩn đoán và đoạn ôn có chính
xác đến đâu, outcome vẫn bằng 0. Vì vậy **hành vi báo mắc kẹt là đối tượng cần điều tra, không phải
chất lượng của phần giải thích.**

---

## 3. Actor — Các nhóm người có liên quan

| Actor | Họ đang làm gì? | Pain hoặc hậu quả có thể có | Họ hưởng lợi thế nào? |
|---|---|---|---|
| **Learner tự học (self-paced)** — người bấm nút | Học bài theo lộ trình, xem video/đọc bài, làm quiz, thường học tối hoặc giờ rảnh, một mình | Mắc ở một đoạn, không biết mình thiếu gì; tra lan man; bỏ qua rồi càng mù các bài sau; mất tự tin, bỏ khoá | Đi tiếp được ngay trong phiên học, không phải học lại từ đầu |
| **Learner trong lớp có deadline** | Học để kịp bài tập/kiểm tra | Ưu tiên "xong bài" hơn "hiểu bài"; cố tình bỏ qua chỗ chưa hiểu | Lấp hổng nhanh mà không mất tiến độ |
| **Instructor / giảng viên** | Soạn bài, trả lời câu hỏi trong forum, xem báo cáo lớp | Không biết ai đang mắc ở đâu; nhận cùng một câu hỏi nền tảng lặp lại; chỉ biết learner mắc khi họ đã bỏ học | Thấy được các chỗ hổng phổ biến để sửa nội dung bài |
| **Trợ giảng / coach / mentor** | Hỗ trợ 1-1, giải đáp trong giờ hỗ trợ | Bị hỏi lại kiến thức nền mà không có ngữ cảnh learner đang mắc ở đâu; tốn thời gian dò lại từ đầu | Nhận yêu cầu đã kèm chỗ hổng cụ thể → hỗ trợ nhanh hơn |
| **Bạn học / peer** | Học cùng khoá, bị hỏi trong nhóm chat | Mất thời gian giải thích lại; trả lời sai/nửa vời | Ít bị hỏi những câu cơ bản |
| **Product / Course team (VLearn)** | Theo dõi tỉ lệ hoàn thành, drop-off theo bài | Drop-off tập trung ở vài bài khó; không rõ nguyên nhân là nội dung hay năng lực nền | Giảm drop-off, có dữ liệu về chỗ hổng để cải thiện nội dung |

**Actor nhóm chọn để điều tra trước:** **Learner tự học (self-paced), đang học một khoá có tính tích
luỹ (bài sau dựa trên bài trước) và trong 7 ngày gần đây đã có lúc không hiểu một phần bài học.**

**Vì sao chọn nhánh này thay vì actor khác:**

- Learner là người **trải pain ngay tại thời điểm mắc kẹt** và cũng chính là người **phải thay đổi
  hành vi** để outcome xảy ra (mắt xích yếu nhất ở Lớp 2 nằm ở họ).
- Instructor và trợ giảng cũng có pain thật, nhưng pain của họ là **hệ quả phía sau** (thiếu tín hiệu,
  câu hỏi lặp lại) và họ chỉ can thiệp được **sau khi** learner đã mắc — không chặn được nguyên nhân.
- Nếu điều tra ở learner mà pain không tồn tại như nhóm nghĩ, thì toàn bộ nhánh instructor cũng sụp
  theo. Đây là nhánh **rẻ nhất để bác bỏ nhanh nhất**.

**Lưu ý rủi ro chọn actor:** người nhận feature (learner bấm nút) **chưa chắc** là người sở hữu pain
chính. Nếu learner *không tự nhận ra* mình chưa hiểu, thì người phát hiện pain thật sự là
instructor/trợ giảng, và solution đúng sẽ chuyển từ "learner chủ động bấm" sang "hệ thống hoặc người
dạy phát hiện trước". Đây là điều nhóm phải kiểm tra ở Chặng 2, không được giả định sẵn.

---

## 4. Situation & Job — User đang cố làm gì trong tình huống nào?

### Khoảnh khắc cụ thể được chọn

```
Tình huống bắt đầu
  → Learner học buổi tối, đang ở giữa một bài mới trong khoá tích luỹ; làm câu quiz thì trả lời sai,
    đọc lại đoạn giải thích 2–3 lần mà vẫn không nối được các ý với nhau. Họ còn khoảng 30 phút và
    muốn xong bài trong hôm nay.
→ User muốn hoàn thành việc gì
  → Hiểu đủ đoạn đang mắc để đi tiếp bài, chứ không phải học lại cả chương.
→ Hiện tại họ làm như thế nào
  → Đọc lại đoạn đó; tua lại video (0.75x hoặc nhảy tới nhảy lui); mở tab mới tra Google/YouTube/
    ChatGPT bằng từ khoá đoán được; hỏi trong nhóm chat rồi chờ; hoặc bỏ qua và tự nhủ "học tiếp
    rồi sẽ hiểu".
→ Điểm bắt đầu gặp vướng mắc
  → Họ không biết mình đang thiếu cái gì, nên không biết tra từ khoá nào. Mỗi kết quả tìm được lại ở
    một mức độ / một ký hiệu khác với bài đang học, phải tự dịch lại. Sau 20–40 phút, hoặc họ hiểu
    lệch, hoặc bỏ qua, và đã mất mạch của bài ban đầu.
```

### Mô tả Situation & Job

> Khi **đang học một bài mới và trả lời sai một câu quiz / đọc lại một đoạn nhiều lần mà vẫn không
> hiểu**, **learner tự học** đang cố **hiểu đủ đoạn đang mắc để tiếp tục bài trong phiên học hôm nay**
> bằng cách **đọc lại, tua lại video, tự tra cứu bên ngoài bằng từ khoá họ đoán, hỏi nhóm chat, hoặc
> bỏ qua và học tiếp**.

### JTBD Hypothesis

> Khi **tôi mắc ở một đoạn trong bài đang học và không chắc mình đang thiếu kiến thức nền nào**, tôi
> muốn **xác định và lấp đúng chỗ hổng đó thật nhanh**, để có thể **tiếp tục bài học ngay trong phiên
> này mà không mất đà và không phải quay lại học lại từ đầu**.

### Job này có còn tồn tại nếu bỏ AI và feature khỏi bối cảnh không?

**Có.** Người học đã phải tự làm việc này từ trước khi có VLearn: tra Google, hỏi bạn, xem lại vở cũ,
tìm video khác. Job "vượt qua chỗ mắc để đi tiếp" tồn tại độc lập với nút bấm và với AI Tutor. Đây là
dấu hiệu cho thấy job được phát biểu ở đúng cao độ, không phải là "job dùng feature".

---

## 5. Pain — Các cách giải thích cạnh tranh

> Pain là **barrier chặn actor hoàn thành job** cộng với **consequence** đi kèm — không phải sự vắng
> mặt của feature. "Learner không có nút Tôi vẫn chưa hiểu" **không phải** là pain.

### Pain Hypothesis A — Diagnosis gap (không định vị được chỗ hổng)

> Khi **mắc ở một đoạn trong bài đang học**, **learner tự học** gặp khó khăn trong việc **hiểu đủ để
> đi tiếp** vì **họ không xác định được mình đang thiếu khái niệm nền nào — không biết mình không biết
> gì, nên không biết phải tra hay hỏi cái gì**, dẫn đến **tra cứu lan man 20–40 phút rồi hiểu lệch,
> hoặc bỏ qua và tích luỹ nợ kiến thức làm các bài sau càng khó, cuối cùng bỏ dở khoá học**.

*Người chủ trì: Tường.*

### Pain Hypothesis B — Momentum / cost gap (biết mình thiếu gì nhưng ngắt mạch quá đắt)

> Khi **mắc ở một đoạn trong bài đang học**, **learner tự học** gặp khó khăn trong việc **hiểu đủ để
> đi tiếp** vì **việc rời khỏi bài để ôn lại nền tốn quá nhiều thời gian và làm mất đà — phải mở tab
> khác, mất chỗ đang đọc, sợ không xong bài trong buổi tối hôm nay**, dẫn đến **họ chủ động bỏ qua chỗ
> chưa hiểu dù biết rõ mình hổng ở đâu, học tiếp trong trạng thái hiểu nửa vời và sai lặp lại ở các
> bài sau**.

*Người chủ trì: Phương.*

### Cách giải thích dự phòng (giữ lại, chưa điều tra ở vòng đầu)

- **C — Confidence gap:** learner hiểu được, nhưng không có gì xác nhận là mình hiểu *đúng*, nên không
  dám đi tiếp; pain thật là thiếu kiểm chứng, không phải thiếu giải thích.
- **D — Content gap:** chỗ mắc do bài giảng nhảy bước / ví dụ kém, không phải do learner thiếu nền.
  Nếu D đúng thì phải sửa nội dung bài, không phải thêm luồng ôn.
- **E — Practice gap:** learner thiếu luyện tập, không thiếu lời giải thích. Thêm một đoạn giải thích
  nữa sẽ không thay đổi gì.
- **F — Awareness gap:** learner **không nhận ra** mình chưa hiểu (tưởng là đã hiểu). Nếu F đúng thì
  mọi cơ chế do learner chủ động khởi động đều thất bại.

### So sánh A và B — vì sao khác biệt này quan trọng

| | Nếu A đúng | Nếu B đúng |
|---|---|---|
| Learner có gọi tên được chỗ hổng? | Không | Có |
| Lõi giá trị nằm ở | Phần **chẩn đoán** | Phần **giảm chi phí ngắt mạch** (giữ chỗ, gọn, quay lại nhanh) |
| Nếu bỏ phần chẩn đoán AI | Solution mất giá trị | Solution vẫn hoạt động |
| Hành vi quan sát được | Tra cứu lan man, nhiều từ khoá khác nhau, hỏi câu mơ hồ | Bỏ qua có ý thức, tự đánh dấu "để sau", hỏi câu rất cụ thể |

### Giả thuyết nhóm chọn để điều tra trước: **A**

**Lý do chọn A:**

1. **A là mắt xích đắt nhất của directive.** Toàn bộ phần "AI chẩn đoán và chọn khái niệm nền" chỉ có
   lý do tồn tại nếu learner thật sự *không* tự định vị được chỗ hổng. Nếu A sai, phần lõi và tốn kém
   nhất của solution mất lý do tồn tại — đây là thứ nhóm cần biết sớm nhất.
2. **A rẻ nhất để bác bỏ.** Chỉ cần yêu cầu learner kể lại lần gần nhất bị mắc và nghe xem họ có tự
   gọi tên được khái niệm hổng hay không; không cần prototype, không cần số liệu.
3. **A và B dẫn tới hai solution hoàn toàn khác nhau**, nên phải phân biệt trước khi làm bất cứ thứ gì.
   B sẽ được kiểm tra song song bằng cùng bộ câu hỏi (cùng một câu chuyện, hai cách đọc khác nhau).

**Pain này có còn tồn tại nếu solution directive biến mất khỏi đầu nhóm không?**
Có — cả A và B đều mô tả một khó khăn đã tồn tại trước khi có nút bấm, và cả hai đều có thể được giải
quyết bằng nhiều cách không liên quan tới AI (xem Solution Parking Lot).

---

## 6. Evidence — Điều cần tìm trước khi viết câu hỏi

> Evidence phải đến từ **sự kiện đã xảy ra, hành vi thật, workaround và hậu quả quan sát được**. Một
> problem statement nghe hợp lý, hoặc một câu "nếu có tính năng đó thì em sẽ dùng", **không phải
> evidence**.

| Cần kiểm tra | Evidence làm nhóm tin hơn | Evidence làm nhóm nghi ngờ hoặc bác bỏ |
|---|---|---|
| **Situation có thật** | Kể được một lần cụ thể trong 7 ngày qua: bài nào, đoạn nào, học lúc nào, đang làm gì khi mắc, kể được trình tự theo thời gian | Không nhớ được lần nào cụ thể; chỉ nói chung chung "thỉnh thoảng cũng khó"; phải được gợi ý mới nhớ ra |
| **Pain có ý nghĩa** | Mô tả được cảm giác mắc kẹt gắn với hành động thật (đóng máy, học tới 1h sáng, hôm sau vẫn mở lại đoạn đó); nói được đã mất bao lâu | Kể xong rồi nói "cũng không sao, học tiếp là quen"; không có hành động nào đi kèm; đã quên chuyện đó ngay hôm sau |
| **Workaround tồn tại** | Kể được chuỗi workaround cụ thể: tra Google với từ khoá gì, xem video nào, hỏi ai, chờ bao lâu; có tab/screenshot/tin nhắn còn lại để chỉ ra | Không làm gì cả và cũng không thấy cần làm gì; workaround duy nhất là "đọc lại một lần rồi đi tiếp" và thấy thế là đủ |
| **Consequence tồn tại** | Có hậu quả quan sát được: làm sai bài sau vì cùng lý do, nộp muộn, phải học lại chương, điểm quiz thấp, dừng khoá 2 tuần | Không có hậu quả nào; vẫn hoàn thành bài đúng hạn; chỗ chưa hiểu đó về sau không cần dùng lại |
| **Pattern có lặp** | Chuyện này xảy ra ≥2–3 lần trong 7 ngày hoặc lặp ở nhiều bài/khoá khác nhau; learner tự nhận ra đây là kiểu tình huống quen thuộc | Chỉ xảy ra một lần với một bài đặc biệt khó; nguyên nhân là hoàn cảnh riêng (mệt, mất tập trung, mất mạng) |
| **Phân biệt A vs B** *(hàng thêm của nhóm)* | Learner **không** gọi tên được khái niệm hổng, chỉ nói "em không hiểu cả đoạn này" → nghiêng về **A** | Learner gọi tên chính xác chỗ hổng nhưng nói "biết thiếu gì nhưng lúc đó không có thời gian ôn lại" → nghiêng về **B** |
| **Ai sở hữu pain** *(hàng thêm của nhóm)* | Learner tự phát hiện mình mắc và tự đi xử lý | Learner chỉ biết mình hổng khi bị điểm thấp hoặc khi trợ giảng chỉ ra → pain thuộc về nhánh **F/instructor** |

### Evidence nào sẽ khiến nhóm sửa hoặc bác bỏ hypothesis?

- **Bác bỏ A, chuyển sang B:** đa số learner kể lại được và **gọi tên đúng** khái niệm mình thiếu ngay
  lúc mắc → phần chẩn đoán không phải là giá trị chính.
- **Bác bỏ cả A và B:** learner bỏ qua chỗ chưa hiểu và **không có hậu quả nào** ở các bài sau → pain
  không đủ quan trọng để đầu tư.
- **Chuyển sang F:** learner không hề biết mình đang hiểu sai cho tới khi làm bài kiểm tra → cơ chế do
  learner chủ động khởi động sẽ không được dùng.
- **Chuyển sang D:** các câu chuyện tụ lại ở **cùng một vài bài** cụ thể → vấn đề nằm ở nội dung bài,
  không ở năng lực nền của learner.

---

## Chốt Problem Hypothesis và park solution

### Problem Hypothesis nhóm mang sang Chặng 2

> **Khi learner tự học mắc ở một đoạn trong bài đang học (trả lời sai quiz hoặc đọc lại nhiều lần vẫn
> không nối được ý), họ không xác định được mình đang thiếu khái niệm nền nào, nên không biết phải tra
> cứu hay hỏi cái gì. Kết quả là họ mất 20–40 phút tra cứu lan man và hiểu lệch, hoặc bỏ qua và học
> tiếp trong trạng thái hổng — làm các bài phụ thuộc sau đó càng khó và tăng nguy cơ bỏ dở khoá học.**

### Điều gì phải đúng để giả thuyết đứng vững

1. Learner **nhận ra được** ngay tại thời điểm đó là mình chưa hiểu (chứ không tưởng là đã hiểu).
2. Learner **không tự gọi tên được** khái niệm nền đang thiếu — chỗ hổng là mơ hồ, không có tên.
3. Nguyên nhân mắc thật sự là **thiếu kiến thức nền có trước**, không phải do bài giảng viết tệ, thiếu
   luyện tập hay mất tập trung.
4. Learner **đã bỏ công sức thật** để tự xử lý (có workaround, có thời gian bỏ ra) → chứng tỏ họ có
   động lực.
5. Việc bỏ qua chỗ hổng **để lại hậu quả quan sát được** ở các bài sau, không tự biến mất.
6. Tình huống này **lặp lại**, không phải một lần cá biệt.
7. Learner **muốn giải quyết ngay trong phiên học**, chứ không muốn ghi lại để xử lý sau.

### Điều gì có thể khiến nhóm sửa hoặc bác bỏ giả thuyết

- Learner gọi tên được chính xác chỗ hổng → **sửa sang Pain B** (vấn đề là chi phí ngắt mạch, không
  phải chẩn đoán).
- Learner không có workaround nào và cũng không thấy cần → **pain không đủ quan trọng**, bác bỏ.
- Bỏ qua chỗ chưa hiểu mà không có hậu quả nào → **consequence không tồn tại**, bác bỏ.
- Learner chỉ biết mình hổng khi bị điểm thấp / khi trợ giảng chỉ ra → **actor và trigger sai**, phải
  chuyển sang cơ chế phát hiện chủ động (nhánh F).
- Các câu chuyện tụ lại ở cùng một vài bài cụ thể → **nguyên nhân là nội dung bài** (nhánh D).
- Learner nói họ thích ghi lại rồi ôn cuối buổi/cuối tuần → **giả định "quay lại bài ngay" sai**.

### Solution Parking Lot

Đã park lại. Không thiết kế solution ở chặng này; danh sách chỉ để chứng minh nhóm không bị dính vào
một hình thức triển khai duy nhất.

| # | Hướng giải quyết có thể có | AI / Không AI |
|---|---|---|
| 1 | Nút "Tôi vẫn chưa hiểu" + AI chẩn đoán rồi tạo phần ôn nền ngắn (directive gốc) | AI |
| 2 | Mỗi đoạn bài gắn sẵn 1–2 "khái niệm nền cần có" do người soạn bài khai báo, mở ngay trong overlay tại chỗ, không rời bài | Không AI |
| 3 | Readiness check 3 câu trước khi vào bài, dựa trên bảng prerequisite tĩnh; sai thì gợi bài nền tương ứng | Không AI |
| 4 | "Sổ chỗ chưa hiểu": learner highlight đoạn mắc, đánh dấu và học tiếp; hệ thống gom thành danh sách ôn cuối phiên và đẩy cho trợ giảng | Không AI (có thể tăng cường bằng AI để xếp ưu tiên) |
| 5 | Hệ thống phát hiện dấu hiệu mắc kẹt từ hành vi (tua lại nhiều lần, đứng yên lâu, sai lặp cùng dạng câu) và chủ động đề nghị ôn | AI |
| 6 | Routing tới người: câu hỏi tại đúng đoạn đó được đẩy tới trợ giảng hoặc bạn học đã qua bài, cam kết phản hồi trong 15 phút | Không AI |
| 7 | Phân tích drop-off theo đoạn rồi **sửa nội dung bài**: chèn đoạn "cầu nối" 60 giây tại các chỗ nhiều người mắc | Không AI (phần fix) |

*Hướng 2, 3, 4, 6, 7 không dùng AI — vượt yêu cầu tối thiểu 1 hướng không AI.*

---

## Tiêu chí tuyển người phỏng vấn (chuẩn bị cho Chặng 2)

Theo directive: *"trong bảy ngày gần đây đã có lúc không hiểu một phần bài học và phải tìm cách xử lý."*

**Câu hỏi sàng lọc (screener) — chỉ hỏi về quá khứ, không mô tả solution:**

1. Trong 7 ngày qua bạn có học một bài/khoá nào không? Bài gần nhất là hôm nào?
2. Trong 7 ngày qua có lúc nào bạn đọc/xem một phần bài học mà vẫn không hiểu không? Kể ngắn: bài nào?
3. Lúc đó bạn đã làm gì để xử lý? *(Phải có ít nhất một hành động thật — nếu "không làm gì" thì ghi lại
   nhưng xếp vào nhóm đối chứng, không phải nhóm chính.)*

**Loại ra:** người chỉ học lý thuyết rời rạc không có tính tích luỹ; người không nhớ được sự kiện cụ
thể; người mắc vì lý do hoàn cảnh (mất mạng, không có thời gian) chứ không phải vì nội dung.

**Nhóm đối chứng nên có 1 người:** learner nói mình "hầu như không bị mắc" hoặc "bị mắc nhưng bỏ qua
và thấy ổn" — để nghe cho được evidence phản bác, không chỉ evidence ủng hộ.

---

## ✅ CHECKPOINT 1 — Problem Hypothesis (tự kiểm)

- [x] Lần theo được đủ chuỗi **Solution → Change → Actor → Situation & Job → Pain → Evidence**
- [x] Solution đã được gỡ khỏi hình thức cụ thể thành **capability trung tính** (không tên nút, không
      tên feature, không "AI")
- [x] Chuỗi Change viết rõ các mắt xích, **phân biệt được output và outcome**, và chỉ ra mắt xích yếu
      nhất (learner có chịu báo mắc kẹt hay không)
- [x] Liệt kê **nhiều actor**, nêu rõ người nhận feature chưa chắc là người sở hữu pain chính, và giải
      thích **vì sao chọn nhánh learner** thay vì instructor/coach
- [x] Situation là **một khoảnh khắc cụ thể**, và **job vẫn tồn tại** khi bỏ AI + feature khỏi bối cảnh
- [x] Pain được viết dưới dạng **barrier + consequence**, không phải "thiếu feature"
- [x] Có **hai cách giải thích cạnh tranh** A (diagnosis gap) và B (momentum/cost gap), cộng 4 cách giải
      thích dự phòng C–F, và nêu rõ A/B dẫn tới hai solution khác nhau
- [x] Nói rõ **điều gì có thể làm giả thuyết được chọn trở nên sai** (mục *Điều gì có thể khiến nhóm sửa
      hoặc bác bỏ giả thuyết*, cột phải của bảng Evidence)
- [x] Solution đã được **park**: 7 hướng, trong đó 5 hướng không dùng AI

**Trạng thái:** sẵn sàng sang Chặng 2 — viết interview guide để kiểm chứng Pain Hypothesis A (và phân
biệt với B) bằng câu hỏi về sự kiện đã xảy ra.
