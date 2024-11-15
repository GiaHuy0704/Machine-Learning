## Basic Machinelearning 
### MỤC LỤC 

[1. Công Nghệ Sử Dụng](#CongNgheSuDung)

[2. Thuật Toán](#ThuatToan)

[3. Hiển Thị Kết Quả](#hienthiketqua)


<a name ="CongNgheSuDung"></a>
## 1. [Công Nghệ sữ dụng]
**`Numpy`**: Thư viện này được sử dụng để thực hiện các phép toán trên mảng `(arrays)` và là một trong những thư viện cơ bản cho khoa học dữ liệu và tính toán số. Cung cấp nhiều hàm và công cụ để xử lý dữ liệu.

**`Pandas`**: Thư viện mạnh mẽ này cho phép người dùng thao tác và phân tích dữ liệu một cách dễ dàng. Với khả năng đọc và ghi nhiều định dạng file khác nhau `(như .csv, .xls, .xlsx)`, **Pandas** là công cụ chủ chốt việc quản lý và phân tích dữ liệu.

**`Scikit-learn (sklearn)`**: Thư viện này cung cấp nhiều thuật toán học máy, công cụ cho việc chia dữ liệu `(train-test split)`, và đánh giá mô hình. Trong đoạn mã trên, `train_test_split` được sử dụng để chia tập dữ liệu thành tập huấn luyện `(train)` và tập kiểm tra `(test)`.

<a name ="ThuatToan"></a>
## 2. [Thuật Toán]
**[Tải dữ liệu]**: Hàm `loadCsv` trả về một Dataframe Pandas chứa dữ liệu

**[Huấn luyện và kiểm tra]**: Với hàm `splitTrainTest` thực hiện xáo trộn ngẫu nhiên chỉ mục của dữ liệu và chia thành hai phần: 
- Một phần cho huấn luyện (train)
- Một phần cho kiểm tra (test). 
- Tập huấn luyện được sử dụng để huấn luyện mô hình, trong khi tập kiểm tra dùng để đánh giá hiệu suất của mô hình.

**[Chia tập dữ liệu]**: Dữ liệu được chia ra và tìm kiếm nhờ hàm `splitTrainTest`. Trong đó, biến `target` là tên cột mà ta muốn dự đoán, với tham số `ratio` dùng để xác định tỉ lệ dữ liệu dùng cho tập kiểm tra.

**[Tính trung bình lớp]**: Hàm `mean_class` sử dụng phương pháp nhóm `(groupby)` tính toán trung bình của từng lớp trong biến mục tiêu. Có nghĩa là đối với mỗi lớp (chẳng hạn như các loại hoa trong tập dữ liệu Iris), hàm sẽ tính toán trung bình của các đặc trưng `(features)` khác.

**[Dự đoán bằng khoảng cách `Euclid`]**: Hàm `target_pred` sử dụng khoảng cách **Euclid** so sánh điểm dữ liệu trong tập kiểm tra với các trung bình lớp đã được tính toán. Khoảng cách Euclid giữa hai điểm trong không gian nhiều chiều một cách hiệu quả để đo độ tương đồng.

**[kết quả]**: Cuối cùng, các kết quả được dự đoán sẽ so sánh với các giá trị thực tế trong tập kiểm tra. Để dễ dàng thấy được độ chính xác của mô hình thông qua việc so sánh. 

<a name ="hienthiketqua"></a>
 ## 3. [Hiển Thị Kết Quả]

*Kết quả*
- Chạy thử code [centroid_pratice](https://github.com/DucThanh21/Machinelearning/blob/main/MachinelearningLab3/Centroid_practice.ipynb)

data = loadExcel('Iris.xls')

data

data_train, X_test, y_test = splitTrainTest(data, 'iris', ratio = 0.3)

print(data_train)

print(X_test)

print(y_test)


**Hàm bao gồm:** 
- Tải dữ liệu Iris và chia thành tập huấn luyện và kiểm tra.
- Tính toán giá trị trung bình cho mỗi lớp trong tập huấn luyện.
- Dự đoán lớp cho các mẫu trong tập kiểm tra.

![image](https://github.com/user-attachments/assets/e558cf5c-4847-4021-b698-708d5ee1776d)

![image](https://github.com/user-attachments/assets/bea3fdb7-f2cb-48d2-8094-136bd2e341fa)

- bài tập [KNN_BT1](https://github.com/DucThanh21/Machinelearning/blob/main/week_4/lab3/KNN_BT1-practice.ipynb)

- ![image](https://github.com/user-attachments/assets/e9bc78cc-e369-4567-bc29-1c4c2751a9fa)

![image](https://github.com/user-attachments/assets/bc770bcf-0c4f-4941-804b-1b4a33fa6c13)


- ![image](https://github.com/user-attachments/assets/25ff90aa-8505-419b-ba91-cf4ed2d89286)

![image](https://github.com/user-attachments/assets/2b7e4659-939a-4deb-9ae6-683950a0fc8e)

- ![image](https://github.com/user-attachments/assets/13576a33-c4d1-417a-a12a-13032fd30464)

![image](https://github.com/user-attachments/assets/351d6c9b-127e-4173-b584-188920cef4bc)

- ![image](https://github.com/user-attachments/assets/d83b4f91-ff0a-460b-9347-bf355df3544c)

![image](https://github.com/user-attachments/assets/90065e74-34d2-4a70-91cf-081603381822)

- ![image](https://github.com/user-attachments/assets/51f4069e-8e37-4e1a-b305-e7e6bd561b0b)

![image](https://github.com/user-attachments/assets/5dd56e48-7a22-4b3a-9cd0-e51b186af941)

- Bài tập [KNN_BT2](https://github.com/DucThanh21/Machinelearning/blob/main/MachinelearningLab3/KNN_BT2-practice.ipynb).

-![image](https://github.com/user-attachments/assets/76d9ed6d-ff89-432c-b9df-df34976e256b)

![image](https://github.com/user-attachments/assets/5cd02494-67e3-43b1-9d15-6c1a425e74ef)


- ![image](https://github.com/user-attachments/assets/6d0da2d6-a289-4c56-9e75-dae3e5721a61)

![image](https://github.com/user-attachments/assets/ccbb5278-6202-4c53-9ea9-5694ab3bc06c)


- ![image](https://github.com/user-attachments/assets/948ffecc-bb61-45a3-9113-6185c86a3451)

![image](https://github.com/user-attachments/assets/720a904f-9511-4231-8d81-5100cea487ef)


- ![image](https://github.com/user-attachments/assets/26b4fe50-2356-4786-b4b6-8abb03fa442b)

![image](https://github.com/user-attachments/assets/4940e6d6-e2ab-4624-bbb2-c9d20ec520c8)


- ![image](https://github.com/user-attachments/assets/e5bbcfef-baeb-477a-adfd-b1e20dc0ac39)

![image](https://github.com/user-attachments/assets/5996652e-dcd5-410e-ba6d-be80a65bef46)


- ![image](https://github.com/user-attachments/assets/e7f7a8e2-2de8-4f01-a833-8aa6ae0e443d)

![image](https://github.com/user-attachments/assets/50bf6381-7982-4924-8d71-1a7e509bbd21)


