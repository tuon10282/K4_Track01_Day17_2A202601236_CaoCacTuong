# 🎭 Kịch bản phỏng vấn — Q&A mẫu (Chặng 3)

**Chặng 3 · Track 1 Day 17 · Case A — AI Tutor: Diagnostic Refresher**  
**Nhóm:** Cao Các Tường (2A202601236) · Đinh Lê Quỳnh Phương (2A202601865)

| Lượt | Interviewer | Đóng vai User | Kịch bản áp dụng |
|---|---|---|---|
| 1 | Tường | Phương | **Kịch bản số 1** (Khoá Controlled Agent Security) |
| 2 | Phương | Tường | **Kịch bản số 2** (Khoá VLearn Python & Data Analytics) |

---

## 1. Mở đầu chung (Mom Test Compliant)

> "Cảm ơn bạn đã dành thời gian. Bọn mình đang tìm hiểu trải nghiệm học tập thật của mọi người để hiểu rõ hơn cách học diễn ra trong đời thường. Không có câu trả lời đúng hay sai — bọn mình chỉ muốn nghe câu chuyện thật của bạn thôi. Bạn kể mình nghe nhé."

---

## 2. Kịch bản số 1: Khoá Controlled Agent Security (VinBank / AI Security Lab)

> **Bối cảnh:** Learner đang học khoá lập trình online về *Controlled Agent Security* (xây agent cho VinBank: guardrails, HITL, red-teaming), mắc ở một bước trong bài lab và không hiểu khái niệm nền.

### **Q1. Trong 7 ngày gần đây, có lần nào bạn học mà xem lại video/code vẫn không hiểu một phần không?**

> **A (User — kể thật):** Có. Tối thứ 6 em học bài lab `Controlled Agent Security` thì làm bước dựng `egress policy` chạy test trượt 2 lần, xem lại đoạn video hướng dẫn vẫn không hiểu tại sao bị chặn.

---

### **Q2. Kể mình nghe về lần gần nhất đó — bài gì, học lúc nào?**

> **A:** Bài `Guardrails, HITL & Red Teaming` của khoá `AI Agent Security`. Em học khoảng 10h tối, đang code theo starter repo thì bước `HITL approve` không chạy như hướng dẫn.

---

### **Q3. Lúc đó bạn có biết mình đang thiếu kiến thức nền nào không? Nói được cụ thể không?** *(Phân biệt Pain A vs Pain B)*

> **A (Nghiêng A — Không gọi tên được):** Em không biết nữa. Em chỉ thấy test fail, log đầy lỗi lạ. Không biết nên hỏi hay tìm từ khoá gì.  

> **A (Nghiêng B — Gọi tên được):** Em biết là em thiếu khái niệm `correlation ID` và luồng `audit trail` trong HITL. Nhưng tối rồi, mở lại bài cũ ra đọc thì mất cả tiếng, em thôi làm tiếp cho xong.

---

### **Q4. Bạn đã tra từ khoá gì khi tìm kiếm? Vì sao chọn từ khoá đó?**

> **A:** Em gõ `"pytest HITL fail"` trên Google. Vì em đoán là do cấu hình, nhưng kết quả ra đủ thứ kiểu `"mock"`, `"async timeout"`, `"fixture"` — mỗi bài một khác, em phải tự dịch lại. Loay hoay 30 phút vẫn không hiểu.

---

### **Q5. Sau khi thấy không hiểu, bạn đã làm gì tiếp theo?**

> **A:** Em tua lại video, rồi mở tab mới tra Google, rồi hỏi trong nhóm chat của khoá. Hỏi xong em chờ 20 phút mới có người trả lời, mà trả lời chung chung *"chắc do chưa có API key"* — không đúng chỗ em mắc.

---

### **Q6. Bạn mất bao lâu từ lúc thấy không hiểu đến khi xử lý xong?**

> **A:** Khoảng 40 phút. Cuối cùng em sửa theo đại cho test pass, thấy khuya quá nên thôi. Code chạy nhưng em không hiểu vì sao đúng, hôm sau nhìn lại vẫn mơ hồ.

---

### **Q7. Vì không hiểu hết bước đó, về sau có chuyện gì xảy ra không?**

> **A:** Có. Bài sau (viết red-team script) em lại lặp đúng cái sai egress policy đó. Em phải học lại từ đầu bài trước, tốn thêm một buổi tối. Tuần đó em gần như muốn bỏ khoá luôn.

---

### **Q8. Chuyện kiểu vậy có phải một lần duy nhất hay bạn hay gặp?**

> **A:** Em gặp hoài. Tuần này ít nhất 2–3 lần ở mấy bài nền tảng (guard, HITL, tool permission).

---

### **Q9. Lúc đó bạn có cảm thấy phiền không? Hôm sau còn nhớ chuyện đó không?**

> **A:** Có chứ. Em thấy nản, tắt máy lúc 11h30. Sáng hôm sau vẫn còn bực vì chưa hiểu code.

---

## 3. Kịch bản số 2: Khoá VLearn Python & Data Analytics (Quiz & Bài tập tích lũy)

> **Bối cảnh:** Learner tự học khóa *"Python & Data Analytics cơ bản"* trên nền tảng VLearn, mắc kẹt ở câu bài tập Quiz cuối bài do không hiểu bản chất cú pháp nền tảng.

### **Q1. Trong 7 ngày gần đây, có lần nào bạn học trên VLearn mà đọc/xem bài giảng rồi vẫn không hiểu một phần không?**

> **A (User — kể thật):** Có chứ. Tối thứ 5 vừa rồi em học bài *"Vòng lặp và Hàm trong Python"* trên VLearn. Em xem hết video 15 phút, đến đoạn làm bài Quiz kiểm tra kiến thức thì làm trượt 2 lần liền, đọc phần giải thích đáp án trong bài vẫn thấy mù mờ.

---

### **Q2. Kể mình nghe về lần gần nhất đó — bài gì, thuộc khóa nào trên VLearn, bạn học lúc nào?**

> **A:** Đó là Bài 4 trong Chương 2 của khóa *"Python & Data Analytics cơ bản"* trên VLearn. Em học lúc tầm 10h30 tối sau khi đi làm về. Đang hí hởn làm bài Quiz cuối bài thì bị tắc ở câu tính tổng danh sách dùng vòng lặp `for`.

---

### **Q3. Lúc đó bạn có biết mình đang thiếu kiến thức nền nào không? Bạn có nói được cụ thể không?** *(Phân biệt Pain A vs Pain B)*

> **A (Nghiêng A — Không gọi tên được chỗ hổng):**  
> *"Em chịu luôn. Em chỉ thấy nguyên cả câu Quiz với đoạn code mẫu nó cứ rối tung lên. Em không biết là mình đang hổng ở cú pháp `for`, cách khai báo biến đếm, hay do em chưa hiểu về `List`. Không biết phải bắt đầu hỏi từ đâu hay tra cái gì luôn."*  

> **A (Nghiêng B — Gọi tên được chỗ hổng nhưng ngại tốn chi phí ngắt mạch):**  
> *"Em biết rõ là em đang quên cách truy cập phần tử theo chỉ số index trong List mà bài trước ở Chương 1 có dạy. Nhưng lúc đó khuya rồi, nghĩ tới việc phải thoát bài hiện tại, mò lại danh sách bài giảng Chương 1 trên VLearn để tìm đúng cái video đó xem lại thì ngán quá, mất chắc phải 30–40 phút nên em thôi."*

---

### **Q4. Bạn đã tra từ khoá gì khi tìm kiếm? Vì sao chọn từ khoá đó?**

> **A:** Em mở tab mới ra Google gõ đại: `"tại sao vòng lặp for python bị lỗi out of range"`. Vì em đoán mang rợ là do cái đó. Kết quả ra toàn bài viết trên StackOverflow dùng thuật ngữ tiếng Anh rất khó hiểu, em đọc loay hoay 25 phút vẫn không áp dụng được vào bài Quiz trên VLearn.

---

### **Q5. Sau khi thấy không hiểu, bạn đã làm gì tiếp theo?**

> **A:** Em tua đi tua lại đoạn video trên VLearn 2 lần, rồi chụp màn hình câu Quiz quăng vào nhóm Discord/Zalo hỗ trợ của lớp VLearn. Nhưng vì lúc đó muộn rồi (11h đêm), không có trợ giảng nào trực cả. Có 1 bạn học cùng khoá bay vào trả lời nhưng giải thích qua loa làm em càng rối thêm.

---

### **Q6. Bạn mất bao lâu từ lúc thấy không hiểu đến khi xử lý xong (hoặc bỏ cuộc)?**

> **A:** Tổng cộng chắc phải gần 45 phút. Loay hoay từ 10h30 đến 11h15 đêm. Cuối cùng em tích chọn bừa một đáp án cho xong câu Quiz để hệ thống VLearn đánh dấu mở bài tiếp theo, chứ thực ra chưa hiểu bài đó.

---

### **Q7. Vì không hiểu hết đoạn đó, về sau (ở các bài tiếp theo trên VLearn) có chuyện gì xảy ra không?**

> **A:** Hậu quả thấy rõ luôn! Qua bài hôm sau học tới phần *"Xử lý dữ liệu với Pandas"*, code mẫu người ta dùng lại vòng lặp và hàm Python làm em hoàn toàn không theo kịp. Làm bài Lab thực hành bị lỗi liên tục, tốn thêm nguyên một buổi tối cuối tuần để ngồi vật lộn lại. Tuần đó em nản đến mức suýt thì bỏ khoá học luôn trên VLearn.

---

### **Q8. Tình trạng mắc kẹt kiểu này trên VLearn là một lần duy nhất hay bạn gặp thường xuyên?**

> **A:** Em gặp suốt luôn. Trung bình 1 tuần học 4 bài trên VLearn thì chắc phải 2–3 bài bị dính tình trạng này, đặc biệt là ở mấy bài giảng có nhiều bài tập code hoặc công thức tích luỹ.

---

### **Q9. Lúc đó cảm xúc của bạn thế nào? Hôm sau bạn còn nhớ hay bị ảnh hưởng gì không?**

> **A:** Nản và bực lắm chứ. Đi làm về mệt muốn học cho xong mà lại bị kẹt. Sáng hôm sau đi làm ngồi ở công ty trong đầu vẫn lấn cấn chuyện bài học tối qua chưa xong, cảm giác bị nợ kiến thức làm em rất áp lực.

---

## 4. Kịch bản phản xạ khi User nói lệch (Deflect / Anchor / Dig)

* **User khen khóa học / nền tảng:** *"Khóa này bài giảng hay, giao diện mượt."*  
  $\rightarrow$ **Interviewer:** *"Cảm ơn bạn. Cho mình quay lại lúc bạn bị kẹt ở bài đó nhé — lúc thấy bài lab/quiz làm không được thì bạn làm gì tiếp theo?"*

* **User hứa suông:** *"Chắc sau này mình sẽ thu xếp học sớm hơn để có gì hỏi trợ giảng."*  
  $\rightarrow$ **Interviewer:** *"Ừm. Vậy ở lần gần nhất đó, khi chưa có trợ giảng rep thì bạn đã xử lý ra sao?"*

* **User đòi tính năng:** *"Giá như VLearn có thêm nút bấm chat thẳng với AI để giải đáp ngay thì tốt."*  
  $\rightarrow$ **Interviewer:** *"Nếu có cái đó thì nó giúp bạn làm được gì? Còn ở thời điểm hiện tại khi chưa có, bạn đang chữa cháy bằng cách nào?"*

---

## 5. Kết thúc

> "Mình hiểu rồi. Còn điều gì về trải nghiệm học mà mình chưa hỏi tới mà bạn muốn chia sẻ thêm không?"  
> "Cảm ơn bạn nhiều. Những chia sẻ thật của bạn rất có giá trị với bọn mình!"