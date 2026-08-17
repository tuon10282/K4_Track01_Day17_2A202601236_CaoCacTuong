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

### **Q1. Trong khoảng 7 ngày gần đây, có lần nào bạn học mà đọc/xem lại bài giảng vẫn thấy không hiểu một phần không?**

> **A (User — kể thật):** Có. Tối thứ 6 em học bài lab `Controlled Agent Security` thì làm bước dựng `egress policy` chạy test trượt 2 lần, xem lại đoạn video hướng dẫn vẫn không hiểu tại sao bị chặn.

---

### **Q2. Kể mình nghe về lần gần nhất đó — bài học đó là bài gì và bạn học vào lúc nào vậy?**

> **A:** Bài `Guardrails, HITL & Red Teaming` của khoá `AI Agent Security`. Em học khoảng 10h tối, đang code theo starter repo thì bước `HITL approve` không chạy như hướng dẫn.

---

### **Q3. Lúc đó bạn có biết mình đang thiếu kiến thức nền nào không? Nói được cụ thể không?** *(Phân biệt Pain A vs Pain B)*

> **A (Nghiêng A — Không gọi tên được):** Em không biết nữa. Em chỉ thấy test fail, log đầy lỗi lạ. Không biết nên hỏi hay tìm từ khoá gì.  

> **A (Nghiêng B — Gọi tên được):** Em biết là em thiếu khái niệm `correlation ID` và luồng `audit trail` trong HITL. Nhưng tối rồi, mở lại bài cũ ra đọc thì mất cả tiếng, em thôi làm tiếp cho xong.

---

### **Q4. Bạn đã tra từ khoá gì khi tìm kiếm? Vì sao chọn từ khoá đó?**

> **A:** Em gõ `"pytest HITL fail"` trên Google. Vì em đoán là do cấu hình, nhưng kết quả ra toàn đủ thứ kiểu `"mock"`, `"async timeout"`, `"fixture"` — mỗi bài một khác, em phải tự dịch lại. Loay hoay 30 phút vẫn không hiểu.

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

### **Q1. Trong 7 ngày qua, có buổi nào bạn ngồi học mà bị "nghẽn" lại ở một đoạn khó, xem đi xem lại bài giảng vẫn không thể làm tiếp được không?**

> **A (User — kể thật):** Có chứ. Tối thứ 4 vừa rồi em làm bài lab RAG Pipeline v2, bị kẹt ở đoạn cấu hình `Vectorless Fallback` dùng BM25 khi vector database bị timeout. Chạy suite test case fallback toàn báo lỗi, xem lại slide với video hướng dẫn 3 lần vẫn không hiểu nguyên do.

---

### **Q2. Bạn nhớ lại lần gần nhất đó xem — lúc đó bạn đang học bài gì và học vào lúc nào vậy?**

> **A:** Bài lab *"RAG Pipeline v2: Retrieval Hybrid, Vectorless Fallback & Generation có Citation"* thuộc khoá AI Engineering. Em học lúc tầm 10h tối thứ 4, đang gộp kết quả tìm kiếm giữa BM25 với Dense Vector để sinh Citation metadata thì unit test bị trượt ngay dòng tính điểm fusion.

---

### **Q3. Lúc thấy test trượt dính lỗi đó, bạn có tự gọi tên được chính xác mình đang bị hổng kiến thức hay thuật toán nền nào không?** *(Phân biệt Pain A vs Pain B)*

> **A (Nghiêng A — Diagnosis Gap / Không gọi tên được chỗ hổng):**  
> *"Thực sự là em mù tịt luôn. Terminal chỉ hiện một dòng `KeyError: citation_score` ngắn tủn. Em không phân biệt nổi là do em hổng kiến thức toán Reciprocal Rank Fusion (RRF), chưa nắm Pydantic Schema của LangChain, hay do hiểu sai luồng BM25 Fallback. Chẳng biết phải gõ từ nào lên mạng để tìm cách sửa."*  

> **A (Nghiêng B — Momentum Gap / Gọi tên được nhưng ngại ngắt mạch):**  
> *"Em biết tống táng là em quên công thức tính weight của Reciprocal Rank Fusion (RRF) đã dạy ở bài lab tuần trước. Nhưng lúc đó 10h30 tối rồi, nghĩ tới chuyện ngắt mạch bài v2 này để lội lại bài đọc RRF cũ thì ngán quá, mất cả 45 phút nên em nản, đành gõ bừa một con số cố định vào code cho qua."*

---

### **Q4. Lúc không biết làm sao, bạn đã thử gõ từ khóa gì lên Google để tra cứu?**

> **A:** Em gõ đại `langchain RAG hybrid search citation error`. Vì em cứ nghĩ lỗi tại thư viện. Nó nhảy ra toàn bài hướng dẫn dùng LlamaIndex hoặc bản LangChain v0.1 cũ không xài được cho v2. Ngồi lướt lướt mất 30 phút mà chả giải quyết được gì.

---

### **Q5. Tra Google không ăn thua thì bạn xử lý tiếp thế nào?**

> **A:** Em chụp nguyên cái màn hình lỗi gửi vào kênh Zalo/Discord hỗ trợ của lớp VLearn. Mà lúc đó 11h đêm rồi nên không có trợ giảng nào reply. Có một bạn học cùng khóa vào nhắn *"xem lại API Key Embedding xem"*, nghe xong em càng rối thêm vì lỗi này đâu liên quan tới API key.

---

### **Q6. Tính từ lúc bị kẹt tới lúc bạn bỏ cuộc tắt máy thì mất bao nhiêu thời gian? Bạn đã nộp bài thế nào?**

> **A:** Tốn nguyên 45 phút cuống cuồng. Cuối cùng em comment tạm dòng `assert citation_score` trong file test cho test nó xanh để kịp bấm nộp bài trước 12h đêm, chứ thực sự đoạn Fallback với Citation đó em nộp đối phó chứ chưa hiểu.

---

### **Q7. Việc nộp đối phó đoạn đó có kéo theo rắc rối gì cho bạn ở các bài lab phía sau không?**

> **A:** Rắc rối to luôn! Qua bài lab tuần này làm về `Evaluations & Hallucination Guardrails`, bài tập yêu cầu đo đạc độ chính xác của Citation dựa trên Hybrid Retrieval. Vì bài trước em làm lấp liếm nên qua bài này em hoàn toàn bị mất gốc, chạy test trượt hàng loạt, phải bỏ ra nguyên cả ngày Chủ nhật ngồi làm lại từ đầu.

---

### **Q8. Tình trạng bị nghẽn bài lab vì hổng kiến thức tích lũy này có lặp lại thường xuyên với bạn không?**

> **A:** Tuần nào cũng bị dính 2–3 lần luôn anh/chị. Mấy bài lab kiến trúc nâng cao như Router, Hybrid Search, Multi-query toàn bài dài, cứ hổng một khái niệm nhỏ là bị đứng hình ngay.

---

### **Q9. Tối hôm đó nằm xuống ngủ bạn thấy thế nào? Hôm sau đi làm có bị ảnh hưởng gì không?**

> **A:** Bực và áp lực lắm. Đi làm về đã mệt mà học không thông. Sáng hôm sau lên công ty ngồi làm việc mà trong đầu vẫn lấn cấn cảm giác nợ bài, cứ lo lắng không biết cuối tuần có kịp trả nợ kiến thức không.

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