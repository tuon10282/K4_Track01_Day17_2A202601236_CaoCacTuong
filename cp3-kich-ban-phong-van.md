# Kịch bản phỏng vấn — Q&A mẫu (khoá Controlled Agent Security)

**Chặng 3 · Track 1 Day 17 · Case A — AI Tutor: Diagnostic Refresher**
**Nhóm:** Tường (2A202601236) · Phương (2A202601865)

| Lượt | Interviewer | Đóng vai User |
|---|---|---|
| 1 | Tường | Phương |
| 2 | Phương | Tường |

> Bối cảnh mẫu: learner đang học một **khoá lập trình online về Controlled Agent Security** (xây agent
> cho VinBank: guardrails, HITL, red-teaming), mắc ở một bước trong bài lab, không hiểu khái niệm nền.

---

## Mở đầu

> "Cảm ơn bạn đã dành thời gian. Bọn mình đang tìm hiểu trải nghiệm học tập thật của mọi người. Không có
> câu trả lời đúng hay sai, chỉ muốn nghe câu chuyện thật của bạn thôi."

---

## Câu hỏi + câu trả lời mẫu

**Q1. Trong 7 ngày gần đây, có lần nào bạn học mà xem lại video/code vẫn không hiểu một phần không?**

> **A (User — kể thật):** Có. Tối thứ 6 em học bài lab `Controlled Agent Security` thì làm bước dựng
> `egress policy` chạy test trượt 2 lần, xem lại đoạn video hướng dẫn vẫn không hiểu tại sao bị chặn.

---

**Q2. Kể mình nghe về lần gần nhất đó — bài gì, học lúc nào?**

> **A:** Bài `Guardrails, HITL & Red Teaming` của khoá `AI Agent Security`. Em học khoảng 10h tối, đang
> code theo starter repo thì bước `HITL approve` không chạy như hướng dẫn.

---

**Q3. Lúc đó bạn có biết mình đang thiếu kiến thức nền nào không? Nói được cụ thể không?**

> **A (nghiêng A — không gọi tên được):** Em không biết nữa. Em chỉ thấy test fail, log đầy lỗi lạ.
> Không biết nên hỏi hay tìm từ khoá gì.
>
> **A (nghiêng B — gọi tên được):** Em biết là em thiếu khái niệm `correlation ID` và luồng `audit trail`
> trong HITL. Nhưng tối rồi, mở lại bài cũ ra đọc thì mất cả tiếng, em thôi làm tiếp cho xong.

---

**Q4. Bạn đã tra từ khoá gì khi tìm kiếm? Vì sao chọn từ khoá đó?**

> **A:** Em gõ "pytest HITL fail" trên Google. Vì em đoán là do cấu hình, nhưng kết quả ra đủ thứ kiểu
> "mock", "async timeout", "fixture" — mỗi bài một khác, em phải tự dịch lại. Loay hoay 30 phút vẫn không
> hiểu.

---

**Q5. Sau khi thấy không hiểu, bạn đã làm gì tiếp theo?**

> **A:** Em tua lại video, rồi mở tab mới tra Google, rồi hỏi trong nhóm chat của khoá. Hỏi xong em chờ 20
> phút mới có người trả lời, mà trả lời chung chung "chắc do chưa có API key" — không đúng chỗ em mắc.

---

**Q6. Bạn mất bao lâu từ lúc thấy không hiểu đến khi xử lý xong?**

> **A:** Khoảng 40 phút. Cuối cùng em sửa theo đại cho test pass, thấy khuya quá nên thôi. Code chạy nhưng
> em không hiểu vì sao đúng, hôm sau nhìn lại vẫn mơ hồ.

---

**Q7. Vì không hiểu hết bước đó, về sau có chuyện gì xảy ra không?**

> **A:** Có. Bài sau (viết red-team script) em lại lặp đúng cái sai egress policy đó. Em phải học lại từ
> đầu bài trước, tốn thêm một buổi tối. Tuần đó em gần như muốn bỏ khoá luôn.

---

**Q8. Chuyện kiểu vậy có phải một lần duy nhất hay bạn hay gặp?**

> **A:** Em gặp hoài. Tuần này ít nhất 2–3 lần ở mấy bài nền tảng (guard, HITL, tool permission).

---

**Q9. Lúc đó bạn có cảm thấy phiền không? Hôm sau còn nhớ chuyện đó không?**

> **A:** Có chứ. Em thấy nản, tắt máy lúc 11h30. Sáng hôm sau vẫn còn bực vì chưa hiểu code.

---

## Khi user bắt đầu lệch

**User khen:** "Ý tưởng của bạn hay đó."
→ **Interviewer:** "Cảm ơn bạn. Mình quay lại lúc gặp bước khó đó nhé — lúc đó bạn làm gì?"

**User chung chung:** "Chắc sau này mình sẽ học kỹ hơn."
→ **Interviewer:** "Ừ. Lần gần nhất chuyện đó xảy ra là khi nào?"

**User đề xuất feature:** "Nếu có nút hỏi AI thì hay."
→ **Interviewer:** "Điều đó giúp bạn làm được gì? Hiện tại bạn xử lý kiểu đó ra sao?"

---

## Kết thúc

> "Mình hiểu rồi. Còn điều gì về cách bạn học mà mình chưa hỏi tới, bạn muốn nói không?"
>
> "Cảm ơn bạn nhiều. Câu chuyện của bạn giúp ích cho bọn mình lắm."