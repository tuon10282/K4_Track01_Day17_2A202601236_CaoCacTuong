# 🎭 Kịch bản phỏng vấn — Q&A mẫu (Chặng 3)

**Chặng 3 · Track 1 Day 17 · Case A — AI Tutor: Diagnostic Refresher**  
**Nhóm:** Cao Các Tường (2A202601236) · Đinh Lê Quỳnh Phương (2A202601865)

| Lượt | Interviewer | Đóng vai User | Kịch bản áp dụng |
|---|---|---|---|
| 1 | Tường | Phương | **Kịch bản số 1** (Khoá Controlled Agent Security) |
| 2 | Phương | Tường | **Kịch bản số 2** (Khoá RAG Pipeline v2: Hybrid & Citation) |

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

## 3. Kịch bản số 2: Khoá RAG Pipeline v2 (Retrieval Hybrid, Vectorless Fallback & Generation có Citation)

> **Bối cảnh:** Learner đang học khoá *AI Engineering*, làm bài lab *"RAG Pipeline v2: Retrieval Hybrid, Vectorless Fallback & Generation có Citation"*. Learner mắc kẹt ở bước cấu hình cơ chế Vectorless Fallback kết hợp BM25 và trích xuất Citation metadata khi sinh câu trả lời.

### **Q1. Trong 7 ngày gần đây, có lần nào bạn học mà xem lại video/code bài lab vẫn không hiểu một phần không?**

> **A (User — kể thật):** Có chứ. Tối thứ 4 vừa rồi em học bài lab *RAG Pipeline v2* thì mắc ở đoạn làm cơ chế `Vectorless Fallback` kết hợp BM25 khi vector DB bị timeout. Chạy test case fallback cứ bị fail, đọc lại tài liệu hướng dẫn bài lab 3 lần vẫn không hiểu tại sao.

---

### **Q2. Kể mình nghe về lần gần nhất đó — bài gì, học lúc nào?**

> **A:** Bài lab *"RAG Pipeline v2: Retrieval Hybrid, Vectorless Fallback & Generation có Citation"* thuộc khoá AI Engineering. Em học lúc tầm 10h tối, đang làm phần ghép kết quả BM25 với Dense Vector rồi sinh Citation metadata thì test fail ở câu lệnh gộp score.

---

### **Q3. Lúc đó bạn có biết mình đang thiếu kiến thức nền nào không? Bạn có nói được cụ thể không?** *(Phân biệt Pain A vs Pain B)*

> **A (Nghiêng A — Không gọi tên được chỗ hổng):**  
> *"Em chịu luôn. Em chỉ thấy test báo error log `KeyError: citation_score` và kết quả RAG không kèm được nguồn tham chiếu. Em không biết mình đang hổng kiến thức về Reciprocal Rank Fusion (RRF), cú pháp Pydantic Schema của LangChain, hay do em chưa hiểu luồng Fallback của BM25. Không biết nên gõ từ khoá gì để tìm luôn."*  

> **A (Nghiêng B — Gọi tên được chỗ hổng nhưng ngại tốn chi phí ngắt mạch):**  
> *"Em biết rõ là em đang hổng công thức tính trọng số Reciprocal Rank Fusion (RRF) ở bài lab tuần trước. Nhưng lúc đó khuya rồi, nghĩ tới việc phải tạm dừng bài v2 này, lội lại video và bài đọc RRF cũ thì mất chắc phải 40–50 phút nên em nản, thôi cứ sửa đại code cho xong."*

---

### **Q4. Bạn đã tra từ khoá gì khi tìm kiếm? Vì sao chọn từ khoá đó?**

> **A:** Em mở tab mới ra Google gõ đại: `"langchain RAG hybrid search citation error"`. Vì em đoán do thư viện. Kết quả ra toàn bài hướng dẫn dùng LlamaIndex hoặc bản LangChain v0.1 cũ rích không dùng được cho v2, em loay hoay đọc 30 phút vẫn không giải quyết được.

---

### **Q5. Sau khi thấy không hiểu, bạn đã làm gì tiếp theo?**

> **A:** Em tua lại video bài giảng 2 lần, rồi chụp log lỗi quăng vào nhóm Discord/Zalo hỗ trợ của lớp. Nhưng lúc đó 11h đêm rồi không có trợ giảng trực, có 1 bạn học cùng khoá vào rep nhưng khuyên câu chung chung *"xem lại API key Embeddings"* — không đúng chỗ em bị kẹt.

---

### **Q6. Bạn mất bao lâu từ lúc thấy không hiểu đến khi xử lý xong (hoặc bỏ cuộc)?**

> **A:** Tầm 45 phút. Cuối cùng em comment tạm đoạn `assert citation_score` trong unit test cho nó xanh test để nộp bài, chứ thực ra đoạn Fallback và Citation đó em chưa hiểu vì sao code chạy.

---

### **Q7. Vì không hiểu hết đoạn đó, về sau (ở các bài tiếp theo) có chuyện gì xảy ra không?**

> **A:** Có chứ. Qua bài lab tuần này làm về *"Evaluations & Hallucination Guardrails cho RAG"*, bài mới yêu cầu đánh giá độ chính xác của Citation dựa trên Hybrid Retrieval. Vì bài trước em làm đối phó nên qua bài này em hoàn toàn bị mất gốc, làm lại trượt test liên tục, tốn nguyên cả ngày chủ nhật ngồi vật lộn lại từ đầu.

---

### **Q8. Tình trạng mắc kẹt kiểu này là một lần duy nhất hay bạn gặp thường xuyên?**

> **A:** Em gặp hoài. Mấy bài lab về kiến trúc nâng cao (Router, Hybrid Search, Multi-query) bài nào bài nấy đều dài, tuần nào em cũng bị vướng 2–3 lần ở các khái niệm tích luỹ nền tảng.

---

### **Q9. Lúc đó cảm xúc của bạn thế nào? Hôm sau bạn còn nhớ hay bị ảnh hưởng gì không?**

> **A:** Rất áp lực và bực mình. Đi làm cả ngày mệt, tối về học lại bị kẹt ở đoạn thuật toán nền. Sáng hôm sau đi làm ngồi ở công ty vẫn chưa nguôi cảm giác bất an vì bài lab chưa xong hoàn chỉnh.

---

## 4. Kịch bản phản xạ khi User nói lệch (Deflect / Anchor / Dig)

* **User khen khóa học / bài lab:** *"Bài lab RAG này viết kịch bản test hay ghê."*  
  $\rightarrow$ **Interviewer:** *"Cảm ơn bạn. Cho mình quay lại lúc bạn bị kẹt ở bài RAG v2 đó nhé — lúc thấy test Hybrid & Citation fail thì bạn làm gì tiếp theo?"*

* **User hứa suông:** *"Chắc sau này mình sẽ thu xếp học sớm hơn để có gì hỏi trợ giảng."*  
  $\rightarrow$ **Interviewer:** *"Ừm. Vậy ở lần gần nhất đó lúc 11h đêm, khi chưa có trợ giảng rep thì bạn đã xử lý ra sao?"*

* **User đòi tính năng:** *"Giá như có nút bấm chat AI giải thích nguyên nhân fail test ngay bài lab thì tốt."*  
  $\rightarrow$ **Interviewer:** *"Nếu có cái đó thì nó giúp bạn làm được gì? Còn ở thời điểm hiện tại khi chưa có, bạn đang chữa cháy bằng cách nào?"*

---

## 5. Kết thúc

> "Mình hiểu rồi. Còn điều gì về trải nghiệm học mà mình chưa hỏi tới mà bạn muốn chia sẻ thêm không?"  
> "Cảm ơn bạn nhiều. Những chia sẻ thật của bạn rất có giá trị với bọn mình!"