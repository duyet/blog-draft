Trong Machine Learning và NLP, phân lớp văn bản là một bài toán xử lí văn bản cổ điển,
gán các nhãn phân loại lên một văn bản mới dựa trên mức độ tương tự của văn bản đó so với các văn bản đã được gán nhãn trong tập huấn luyện.

Các ứng dụng của phân lớp văn bản thường rất đa dạng như: lọc email spam, phân tích cảm xúc (sentiment analysis), phân loại tin tức, ...

Mình sẽ giới thiệu vài nét rất tổng quát các bước để có thể phân lớp văn bản, một số kỹ thuật thường sử dụng và đưa ra từ khóa để tự tìm hiểu thêm.

-----
# Pipeline
Việc phân lớp về cơ bản có thể có nhiều kỹ thuật, tổng quát đều thực hiện các bước sau:

1. Tiền xử lý văn bản: lọc bỏ dấu câu, chính tả, kĩ tự lỗi, ...
2. Biểu diễn văn bản dưới dạng vector (thường gọi là mô hình hóa văn bản), thường phải làm các công việc như sau:
  * Lọc bỏ stopwords.
  * Tách từ: 
