# K4 · Track 1 — Day 17: Finding and Validating Pain Points

## Thành viên nhóm

| Họ và tên | Mã sinh viên |
|---|---|
| Cao Các Tường | 2A202601236 |
| Đinh Lê Quỳnh Phương | 2A202601865 |

## Đề tài nhóm chọn

**Case A — AI Tutor: Diagnostic Refresher**

Thêm nút "Tôi vẫn chưa hiểu" vào bài học. Khi học viên bấm nút, AI Tutor dùng nội dung bài hiện tại,
các câu trả lời gần đây và lịch sử học tập để đặt 2–3 câu hỏi chẩn đoán ngắn, chọn một khái niệm nền
để ôn lại, tạo một phần giải thích ngắn, rồi đưa học viên trở về bài đang học.

| Thành phần | Solution đã mô tả |
|---|---|
| Trigger | Học viên bấm "Tôi vẫn chưa hiểu" |
| Input | Bài hiện tại, câu trả lời gần đây, lịch sử học tập |
| AI action | Chẩn đoán và lựa chọn khái niệm nền |
| Output | Một phần ôn lại ngắn trước khi quay lại bài hiện tại |
| User control | Học viên chủ động yêu cầu trợ giúp |

**Đối tượng phỏng vấn:** người trong 7 ngày gần đây đã có lúc không hiểu một phần bài học và phải tìm
cách xử lý.

## Tài liệu trong repo

| File | Nội dung |
|---|---|
| [chang-1-dat-gia-thuyet.md](chang-1-dat-gia-thuyet.md) | Chặng 1 — Đặt giả thuyết (bản phân tích chi tiết) |
| [cp1-phuong.md](cp1-phuong.md) | Chặng 1 — Checkpoint 1 (bản template điền sẵn - Phương) |
| [plan.md](plan.md) | Kế hoạch làm việc và phân công theo 4 chặng của buổi học |
| [README.md](README.md) | File này |

## Kết quả Chặng 1 (tóm tắt)

**Capability trung tính** (đã gỡ khỏi tên nút / tên feature / AI): khi người học bị mắc ở một đoạn
trong bài, họ được giúp xác định đúng chỗ hổng kiến thức đang chặn mình và lấp nó đủ nhanh để quay lại
tiếp tục bài học trong cùng phiên.

**Actor điều tra trước:** learner tự học (self-paced) trong khoá có tính tích luỹ — vì họ vừa trải pain
tại thời điểm mắc kẹt, vừa là người phải thay đổi hành vi để outcome xảy ra.

**Hai cách giải thích cạnh tranh:**
- **A — Diagnosis gap:** learner không gọi tên được khái niệm nền mình đang thiếu → tra cứu lan man
  hoặc bỏ qua. *(chọn điều tra trước)*
- **B — Momentum/cost gap:** learner biết mình thiếu gì, nhưng rời bài để ôn quá đắt về thời gian và
  mất đà → cố tình bỏ qua.

Nhóm chọn A trước vì nếu A sai thì phần lõi đắt nhất của directive — chẩn đoán bằng AI — mất lý do tồn
tại, và A là giả thuyết rẻ nhất để bác bỏ bằng phỏng vấn.

## Phân công

| Chặng | Tường | Phương |
|---|---|---|
| 1 · Đặt giả thuyết | Lớp Solution, Change, Evidence; chủ trì Pain Hypothesis A | Lớp Actor, Situation & Job, Pain; chủ trì Pain Hypothesis B |
| 2 · Chuẩn bị phỏng vấn | Câu hỏi warm-up và khai thác bối cảnh | Câu hỏi deep-dive và đánh giá mức độ ưu tiên của pain |
| 3 · Luyện phỏng vấn | Lượt 1 làm interviewer, lượt 2 đóng vai user | Lượt 1 đóng vai user, lượt 2 làm interviewer |
| 4 · Chỉnh guide & nộp | Rà soát lại interview guide sau khi phỏng vấn thử | Tổng hợp bộ giả thuyết, kiểm tra format và submit |

Chi tiết mốc thời gian của Chặng 1 nằm ở mục *Phân công task cho 2 người* trong
[chang-1-dat-gia-thuyet.md](chang-1-dat-gia-thuyet.md).

## Lưu ý

Mọi nội dung ở Chặng 1 là **hypothesis**, chưa phải fact về user. Nhóm chưa phỏng vấn ai ở thời điểm
viết tài liệu này; solution đã được park lại để không kéo kết luận về pain theo hình thức triển khai
được giao.
