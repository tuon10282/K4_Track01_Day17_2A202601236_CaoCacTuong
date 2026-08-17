# Interview Record — Luyện phỏng vấn Chặng 3 (2 lượt)

**Track 1 · Day 17 — Finding and Validating Pain Points · Case A — AI Tutor: Diagnostic Refresher**

> Gồm 2 lượt: **Lượt 1 — Tường làm interviewer** (kịch bản Controlled Agent Security) và
> **Lượt 2 — Phương làm interviewer** (kịch bản RAG Pipeline v2). Mục tiêu chung: kiểm chứng Pain A
> (Diagnosis gap) và phân biệt với Pain B (Momentum/cost gap).

---

# Lượt 1 — Tường (Interviewer) · Huy (User)

| Thông tin | Chi tiết |
|---|---|
| Interviewer | Cao Các Tường (2A202601236) |
| Người đóng vai User | Nguyễn Quang Huy — 2A202601873|
| Kịch bản | Số 1 — Khoá Controlled Agent Security (VinBank / AI Security Lab) |
| Ngày | 17/08/2026 |
| Thời lượng | ~20 phút |
| Bản ghi âm | [recording1.m4a](recording1.m4a) |

---

## 1. Recruitment check

> "Trong 7 ngày qua có lúc nào bạn đang học một bài/khoá mà đọc lại hoặc xem lại vẫn không hiểu một
> phần không? Kể ngắn: bài đó là bài nào?"

**Trả lời:** Có — tối thứ 6 học bài lab `Controlled Agent Security`, làm bước dựng `egress policy` chạy
test trượt 2 lần, xem lại video hướng dẫn vẫn không hiểu tại sao bị chặn.

**Đánh giá:** ✅ Đạt tiêu chí — sự kiện cụ thể trong 7 ngày, có hành động xử lý thật (xem lại video, tra
cứu, hỏi nhóm chat).

---

## 2. Diễn biến phỏng vấn (tóm tắt theo câu hỏi)

### Q1–Q2. Story opener — lần gần nhất mắc kẹt

- Bài: `Guardrails, HITL & Red Teaming` (khoá AI Agent Security), học khoảng 10h tối.
- Chỗ mắc: bước `HITL approve` không chạy như hướng dẫn dù code theo starter repo.

### Q3. Lúc đó có gọi tên được chỗ hổng không? *(câu "đáng sợ" — phân biệt A vs B)*

- Trả lời **nghiêng A**: *"Em không biết nữa. Em chỉ thấy test fail, log đầy lỗi lạ. Không biết nên hỏi
  hay tìm từ khoá gì."*
- Trả lời **nghiêng B** (bản đối chiếu để kiểm tra): *"Em biết là em thiếu khái niệm `correlation ID`
  và luồng `audit trail` trong HITL, nhưng tối rồi mở lại bài cũ ra đọc thì mất cả tiếng."*

### Q4. Từ khoá đã tra cứu

- Gõ `"pytest HITL fail"` trên Google vì đoán là do cấu hình.
- Kết quả trả về toàn `mock`, `async timeout`, `fixture` — mỗi bài một khác, phải tự dịch lại.

### Q5. Workaround

1. Tua lại video.
2. Mở tab mới tra Google.
3. Hỏi nhóm chat của khoá — chờ 20 phút mới có trả lời chung chung *"chắc do chưa có API key"*,
   không đúng chỗ mắc.

### Q6. Thời gian mất

- Khoảng 40 phút từ lúc thấy không hiểu đến khi xử lý xong.
- Cuối cùng sửa theo đại cho test pass, code chạy nhưng không hiểu vì sao đúng.

### Q7. Hậu quả ở bài sau

- Bài sau (viết red-team script) lặp lại đúng cái sai `egress policy`.
- Phải học lại từ đầu bài trước, tốn thêm một buổi tối; tuần đó gần như muốn bỏ khoá.

### Q8. Mức độ lặp lại

- "Gặp hoài" — tuần này ít nhất 2–3 lần ở mấy bài nền tảng (guard, HITL, tool permission).

### Q9. Cảm xúc / ghi nhớ

- Thấy nản, tắt máy lúc 11h30; sáng hôm sau vẫn bực vì chưa hiểu code.

---

## 3. Bảng đọc evidence → kết luận giả thuyết

| Nghe được từ interviewee | Kết luận |
|---|---|
| Không gọi tên được khái niệm hổng ("em không biết nữa", "không biết tìm từ khoá gì") | → nghiêng **A — Diagnosis gap** |
| Trả lời nghiêng B nêu rõ tên khái niệm (`correlation ID`, `audit trail`) | → cảnh báo: nếu learner gọi tên được thì A yếu đi, lệch về **B** |
| Chuỗi workaround dài (tua video → Google → nhóm chat) + mất ~40 phút | → pain có ý nghĩa, đã bỏ công sức thật |
| Sai lặp ở bài sau, phải học lại từ đầu, gần như bỏ khoá | → consequence tồn tại và quan sát được |
| Lặp 2–3 lần/tuần ở nhiều bài nền tảng | → pattern có lặp, không phải lần cá biệt |
| Chỉ biết hổng khi trợ giảng chỉ ra? | → **không** — learner tự phát hiện và tự xử lý, vẫn giữ nhánh learner |

**Kết luận sơ bộ sau lượt 1:** Pain A (diagnosis gap) **chưa bị bác bỏ** — learner không tự gọi tên được
chỗ hổng, có workaround tốn thời gian, có hậu quả và pattern lặp lại. Pain B chỉ xuất hiện ở bản kịch
bản đối chiếu, cần thêm lượt 2 (Phương làm interviewer) để chốt.

---

## 4. Điều chỉnh guide sau khi luyện (đầu vào Chặng 4)

- [x] Câu Q3 phải bấm sâu hơn: sau câu *"bạn có biết mình thiếu gì không"*, thêm *"bạn tra từ khoá gì?"*
  để có bằng chứng hành vi, không dừng ở lời khẳng định chủ quan.
- [x] Thêm follow-up Q8 (mức độ lặp) trước khi kết thúc — ban đầu guide bỏ sót, dễ rơi vào đánh giá
  chủ quan *"cũng hay gặp"*.
- [x] Khi user trả lời nghiêng B (gọi tên được chỗ hổng), không được chuyển hướng guide ngay — giữ
  nguyên chuỗi workaround/consequence để so sánh hai cách đọc của cùng một câu chuyện.

---

# Lượt 2 — Phương (Interviewer) · Huế (User)

| Thông tin | Chi tiết |
|---|---|
| Interviewer | Đinh Lê Quỳnh Phương (2A202601865) |
| Người đóng vai User | Lăng Thị Phương Huế — 2A202601915  |
| Kịch bản | Số 2 — Khoá RAG Pipeline v2 (Retrieval Hybrid, Vectorless Fallback & Generation có Citation) |
| Ngày | 17/08/2026 |
| Thời lượng | ~20 phút |
| Bản ghi âm | [recording2.m4a](recording2.m4a) |

## 1. Recruitment check

> "Trong 7 ngày qua có lúc nào bạn đang học một bài/khoá mà đọc lại hoặc xem lại vẫn không hiểu một
> phần không? Kể ngắn: bài đó là bài nào?"

**Trả lời:** Có — tối thứ 4 học bài lab `RAG Pipeline v2`, bị kẹt ở đoạn cấu hình `Vectorless Fallback`
dùng BM25 khi vector database bị timeout; chạy suite test fallback toàn báo lỗi, xem lại slide + video
3 lần vẫn không hiểu nguyên do.

**Đánh giá:** ✅ Đạt tiêu chí — sự kiện cụ thể trong 7 ngày, có hành động xử lý thật.

## 2. Diễn biến phỏng vấn (tóm tắt theo câu hỏi)

### Q1–Q2. Story opener — lần gần nhất mắc kẹt

- Bài: lab "RAG Pipeline v2: Retrieval Hybrid, Vectorless Fallback & Generation có Citation" (khoá AI
  Engineering), học khoảng 10h tối thứ 4.
- Chỗ mắc: gộp kết quả tìm kiếm giữa BM25 với Dense Vector để sinh Citation metadata thì unit test
  trượt ngay dòng tính điểm fusion.

### Q3. Có gọi tên được chỗ hổng không? *(câu "đáng sợ" — phân biệt A vs B)*

- Trả lời **nghiêng A**: *"Terminal chỉ hiện dòng `KeyError: citation_score`. Em không phân biệt nổi là do
  hổng toán Reciprocal Rank Fusion (RRF), chưa nắm Pydantic Schema của LangChain, hay hiểu sai luồng BM25
  Fallback. Chẳng biết gõ từ nào lên mạng để tìm cách sửa."*
- Trả lời **nghiêng B** (bản đối chiếu): *"Em biết là quên công thức tính weight của RRF, nhưng 10h30 tối
  rồi, nghĩ tới lội lại bài đọc RRF cũ mất 45 phút thì ngán, đành gõ bừa một con số cố định cho qua."*

### Q4. Từ khoá đã tra cứu

- Gõ `langchain RAG hybrid search citation error` vì nghĩ lỗi tại thư viện.
- Kết quả ra toàn bài hướng dẫn LlamaIndex / LangChain v0.1 cũ, không dùng được cho v2; lướt mất 30 phút
  mà không giải quyết gì.

### Q5. Workaround

1. Xem lại slide + tua lại video 3 lần.
2. Tra Google với từ khoá.
3. Chụp màn hình lỗi gửi Zalo/Discord hỗ trợ của lớp — 11h đêm không có trợ giảng reply; bạn học nhắn
   *"xem lại API Key Embedding xem"* — càng rối vì lỗi không liên quan API key.

### Q6. Thời gian mất

- ~45 phút từ lúc bị kẹt tới lúc bỏ cuộc; cuối cùng comment tạm dòng `assert citation_score` trong file
  test cho test xanh để kịp bấm nộp trước 12h đêm — nộp đối phó, chưa hiểu.

### Q7. Hậu quả ở bài sau

- Bài lab tuần sau (Evaluations & Hallucination Guardrails) yêu cầu đo độ chính xác Citation dựa trên
  Hybrid Retrieval — mất gốc vì bài trước làm lấp liếm, test trượt hàng loạt, phải bỏ ra cả ngày Chủ
  nhật làm lại từ đầu.

### Q8. Mức độ lặp lại

- "Tuần nào cũng 2–3 lần" — mấy bài lab kiến trúc nâng cao (Router, Hybrid Search, Multi-query) bài dài,
  cứ hổng một khái niệm nhỏ là đứng hình.

### Q9. Cảm xúc / ghi nhớ

- Bực và áp lực (đi làm về mệt mà học không thông); sáng hôm sau lên công ty vẫn lấn cấn cảm giác nợ bài.

## 3. Bảng đọc evidence → kết luận giả thuyết

| Nghe được từ interviewee | Kết luận |
|---|---|
| Không gọi tên được chỗ hổng ("không phân biệt nổi", "chẳng biết gõ từ nào") | → nghiêng **A — Diagnosis gap** |
| Nghiêng B nêu rõ tên (`RRF weight`) nhưng ngại thời gian | → cảnh báo: nếu learner gọi tên chính xác chỗ hổng thì A yếu đi, lệch về **B** |
| Chuỗi workaround dài (slide → video → Google → chat lớp) + ~45 phút | → pain có ý nghĩa, đã bỏ công sức thật |
| Nộp đối phó → mất gốc bài sau, làm lại cả ngày | → consequence tồn tại và quan sát được |
| 2–3 lần/tuần ở nhiều bài khác nhau | → pattern có lặp, không phải lần cá biệt |
| Learner tự phát hiện mắc và tự xử lý | → giữ nhánh learner, không chuyển sang F/instructor |

## 4. Kết luận chung sau 2 lượt

- **Pain A (Diagnosis gap) chưa bị bác bỏ:** cả hai lượt, learner đều không tự gọi tên được chỗ hổng, có
  workaround tốn 40–45 phút, có hậu quả ở bài sau và pattern lặp 2–3 lần/tuần.
- **Pain B** chỉ xuất hiện ở bản kịch bản đối chiếu (gọi tên được chỗ hổng nhưng ngại chi phí ngắt mạch)
  — chưa có bằng chứng thật, cần kiểm tra song song khi phỏng vấn người thật.
- Guide sau khi chỉnh (Mục 4 lượt 1) đã hoạt động ổn ở lượt 2; sẵn sàng phỏng vấn người trong 7 ngày gần
  đây có lúc không hiểu một phần bài học.

---

## 5. Ghi chú khác

- Bản ghi âm: [recording1.m4a](recording1.m4a) (lượt 1 — Tường interviewer) ·
  [recording2.m4a](recording2.m4a) (lượt 2 — Phương interviewer).
- Toàn bộ là **dữ liệu luyện tập trong nhóm** (lượt 1: Phương đóng user; lượt 2: Tường đóng user), chưa
  phải phỏng vấn người thật bên ngoài — dùng để chỉnh guide trước khi đi phỏng vấn thật.