# Interview Record — Lượt phỏng vấn của Tường (Interviewer)

**Track 1 · Day 17 — Finding and Validating Pain Points · Case A — AI Tutor: Diagnostic Refresher**

| Thông tin | Chi tiết |
|---|---|
| Interviewer | Cao Các Tường (2A202601236) |
| Người đóng vai User | Đinh Lê Quỳnh Phương (2A202601865) |
| Kịch bản | Số 1 — Khoá Controlled Agent Security (VinBank / AI Security Lab) |
| Ngày | 17/08/2026 |
| Thời lượng | ~20 phút |
| Mục tiêu | Kiểm chứng Pain A (Diagnosis gap) và phân biệt với Pain B (Momentum/cost gap) |

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

## 5. Ghi chú khác

- Bản ghi âm: [recording1.m4a](recording1.m4a) (lượt 1 — Tường interviewer) ·
  [recording2.m4a](recording2.m4a) (lượt 2 — Phương interviewer).
- Toàn bộ là **dữ liệu luyện tập trong nhóm** (vai user do Phương đóng), chưa phải phỏng vấn người thật
  bên ngoài — dùng để chỉnh guide trước khi đi phỏng vấn thật.