### BASIC MACHINELEARNING
### MỤC LỤC 

[1. Công Nghệ Sử Dụng](#CongNgheSuDung)

[2. Thuật Toán](#ThuatToan)

[3. Hiển Thị Kết Quả](#hienthiketqua)
<a name ="CongNgheSuDung"></a>
## 1. [Công Nghệ sữ dụng]
- **`Numpy`**: Thư viện này được sử dụng để thực hiện các phép toán trên mảng `(arrays)` và là một trong những thư viện cơ bản cho khoa học dữ liệu và tính toán số. Nó cung cấp nhiều hàm và công cụ để xử lý dữ liệu một cách hiệu quả.

- **`Pandas`**: Thư viện mạnh mẽ này cho phép người dùng thao tác và phân tích dữ liệu một cách dễ dàng. Pandas có khả năng đọc và ghi nhiều định dạng file khác nhau (như `.csv`, `.xls`, `.xlsx`), giúp quản lý và phân tích dữ liệu trở nên thuận tiện hơn.

- **`Scikit-learn (sklearn)`**: Thư viện cung cấp các thuật toán học máy, công cụ cho việc chia dữ liệu (`train-test split`), và đánh giá mô hình. Trong đoạn mã, `train_test_split` được sử dụng để chia tập dữ liệu thành tập huấn luyện và tập kiểm tra. Ngoài ra, thư viện còn cung cấp các mô hình như `DecisionTreeClassifier` và `RandomForestClassifier` để xây dựng và huấn luyện mô hình học máy.

<a name ="ThuatToan"></a>
## 2. [Thuật Toán]

### Tải dữ liệu
- Dữ liệu được tải vào sử dụng `Pandas` với hàm `read_csv`. Kết quả là một DataFrame chứa thông tin về các thuộc tính và mục tiêu (loại thuốc) cho mô hình.

### Huấn luyện và Kiểm tra
- Sử dụng hàm `train_test_split` để chia dữ liệu thành tập huấn luyện (`train`) và tập kiểm tra (`test`). Tập huấn luyện được sử dụng để huấn luyện mô hình, trong khi tập kiểm tra sẽ đánh giá hiệu suất của mô hình.

### Cây quyết định (Decision Tree)
- Mô hình Decision Tree sử dụng các tham số như `min_samples_split`, `max_depth`, và `min_samples_leaf` để kiểm soát quá trình phân nhánh, tránh overfitting và đạt được dự đoán chính xác nhất.

### Rừng ngẫu nhiên (Random Forest)
- Random Forest là tập hợp của nhiều cây quyết định, giúp cải thiện độ chính xác và tính ổn định. Mô hình này sử dụng tham số `n_estimators` để xác định số lượng cây và `max_features` để chọn đặc trưng ngẫu nhiên tại mỗi nút phân chia.

<a name ="hienthiketqua"></a>
 ## 3. [Hiển Thị Kết Quả]

 *kết quả*
 
 ![image](https://github.com/user-attachments/assets/f178b749-2fa6-48bd-9daa-ad12d53ccf31)


 
