﻿# NLP_email_spam_or_ham
## Giới thiệu
Trong thời đại số, email là phương tiện trao đổi thông tin phổ biến, tuy nhiên, thư rác (spam) đang trở thành vấn đề đáng lo ngại với số lượng lớn, nội dung phiền nhiễu và tiềm ẩn nguy cơ bảo mật. Việc phân loại thư rác giúp bảo vệ người dùng, tiết kiệm tài nguyên và tăng cường an ninh mạng. Nhằm giải quyết bài toán này, nhóm nghiên cứu xây dựng mô hình học máy kết hợp xử lý ngôn ngữ tự nhiên (NLP) để tự động nhận diện và phân loại email spam, góp phần nâng cao trải nghiệm và hiệu quả sử dụng hệ thống thư điện tử.

## Mục tiêu đề tài
* Nghiên cứu này nhằm xây dựng một mô hình phát hiện email spam hiệu quả, áp dụng các kỹ thuật NLP và học máy tiên tiến.

## Thành viên nhóm 
* A46350 Trần Huyền Trang
* A46483 Nguyễn Thị Thùy Trang
* A45510 Phạm Thanh Mai
* A39948 Phạm Tiến Đạt

## Công nghệ sử dụng
* Ngôn ngữ lập trình: Python
* Thư viện chính: Pandas, Scikit-learning, Tensorflow, Tokenization
* Mô hình: Naive Bayes, Random Forest, LSTM

## Bộ dữ liệu sử dụng
Bộ dữ liệu Email Spam Classification Dataset, được cung cấp trên Kaggle bởi người dùng purusinghvi, là một tập dữ liệu tổng hợp từ hai nguồn lớn: TREC 2007 Public Spam Corpus và Enron-Spam Dataset. Mục tiêu của bộ dữ liệu này là cung cấp một tập hợp các email đã được gán nhãn rõ ràng (spam hoặc không spam), phục vụ cho các nghiên cứu và ứng dụng liên quan đến lọc và phân loại thư rác bằng kỹ thuật học máy.
(https://www.kaggle.com/datasets/purusinghvi/email-spam-classification-dataset?select=combined_data.csv)

## Demo
https://github.com/Kannee37/demo_NLP

## Kết quả và Đánh giá

| Mô hình        | Accuracy | Precision | Recall   | F1-Score | AUC ROC  | Thời gian huấn luyện |
|----------------|----------|-----------|----------|----------|----------|------------------------|
| Naïve Bayes    | 0.963990 | 0.972836  | 0.958324 | 0.965525 | 0.993704 | 0.0074 giây            |
| Random Forest  | 0.984182 | 0.984748  | 0.985197 | 0.984973 | 0.998017 | 0.8639 giây            |
| LSTM           | 0.984602 | 0.984761  | 0.985994 | 0.985377 | 0.997116 | 2.6525 giây            |

* LSTM cho thấy hiệu suất vượt trội so với Naive Bayes và Random 
Forest, đặc biệt trong việc dự đoán chính xác. Điều này cho thấy LSTM 
có khả năng nắm bắt các mẫu phức tạp trong dữ liệu tốt hơn so với hai 
mô hình còn lại.
   Random Forest tốt hơn Naïve Bayes: Random Forest cho thấy hiệu suất 
đáng kể so với Naïve Bayes, với số lượng dự đoán đúng cao hơn và số 
lượng dự đoán sai thấp hơn ở cả hai lớp.

