## Basic Machinelearning 

# Lab2 _  Phân phối VBernoulli, Gaussian và Multinomial
### MỤC LỤC 

[1. Công Nghệ Sử Dụng](#CongNgheSuDung)

[2. Thuật Toán](#ThuatToan)

[3. Hiển Thị Kết Quả](#hienthiketqua)

<a name ="CongNgheSuDung"></a>
## 1. [Công Nghệ sữ dụng]

## Thư viện python: 
-`pandas`, `sklearn` (scikit-learn)

## Các công cụ chính:
- `CountVectorizer`: Để chuyển đổi văn bản thành các đặc trưng số.
-  `BernoulliNB` và `MultinomialNB`: Áp dụng các phân phối Naive Bayes khác nhau.
-  `train_test_split`: Chia dữ liệu thành tập huấn luyện và kiểm tra.
- `GaussianNB`: Mô hình Naive Bayes với phân phối Gaussian.
- `train_test_split`: Chia dữ liệu thành tập huấn luyện và kiểm tra.
- `LabelEncoder`: Mã hóa các giá trị phân loại thành số.

<a name ="ThuatToan"></a>
[2. Thuật Toán](#ThuatToan)

## Thuật toán sử dụng:
- Phân phối Bernoulli Naive Bayes: Áp dụng cho dữ liệu `hị phân (binary)`. Phù hợp khi các đặc trưng chỉ có hai giá trị (0 hoặc 1).
  
- Phân phối Multinomial Naive Bayes: Áp dụng cho `dữ liệu rời rạc (discrete)`, đặc biệt là trong bài toán phân loại văn bản. Phù hợp khi đặc trưng là tần suất xuất hiện từ trong văn bản.
  
- Phân phối Gaussian Naive Bayes: Áp dụng cho dữ liệu liên tục. Phân phối này phù hợp cho các bài toán mà đặc trưng đầu vào là các biến số liên tục như tuổi, tỷ lệ Natri/Kali.

<a name ="hienthiketqua"></a>
[3. Hiển Thị Kết Quả](#hienthiketqua)

**kết quả của thực hiện**

![image](https://github.com/user-attachments/assets/f071a20a-cdcd-48c9-ad18-fafdc63dfe60)

![image](https://github.com/user-attachments/assets/0c17e85b-7404-4e6e-8d3a-484165fc94df)

[ Áp dụng thuật toán Naive Bayes (phân phối bernoulli và phân phối Multinomial) để dự đoán cảm xúc của văn bản là tích cực hay tiêu cực và so sánh kết quả của hai phân phối đó.]


[ Yêu cầu: Áp dụng thuật toán Naive Bayes (phân phối Gaussian) để dự đoán kết quả loại thuốc phù hợp với bệnh nhân.]

![image](https://github.com/user-attachments/assets/b3a98f44-a387-43b2-9461-6a0e69020de5)





