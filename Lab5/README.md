### BÀI TOÁN SVM SỬ DỤNG CVXOPT

### MỤC LỤC
[1. Công Nghệ Sử Dụng](#CongNgheSuDung)

[2. Thuật Toán](#ThuatToan)

[3. Hiển Thị Kết Quả](#HienThiKetQua)

---

<a name="CongNgheSuDung"></a>
## 1. Công Nghệ Sử Dụng
- **`Numpy`**: Thư viện cơ bản được sử dụng để tính toán trên mảng và ma trận, hỗ trợ thao tác dữ liệu hiệu quả và tối ưu cho tính toán khoa học trong Python.

- **`CVXOPT`**: Thư viện được sử dụng để giải các bài toán tối ưu lồi, trong trường hợp này được áp dụng để giải bài toán lập trình bậc hai nhằm tìm các giá trị tối ưu của λ, w, và b cho SVM. Đây là thành phần quan trọng để tối ưu hóa toán học trong SVM biên cứng và biên mềm.

- **`Matplotlib`**: Thư viện dùng để trực quan hóa dữ liệu, vẽ biểu đồ, đường biên quyết định, và các vector hỗ trợ. Nó giúp tạo ra các biểu diễn đồ họa của kết quả mô hình.

<a name="ThuatToan"></a>
## 2. Thuật Toán

### SVM Biên Cứng
- **Dữ liệu**: Một tập dữ liệu nhỏ với các điểm huấn luyện được phân loại vào hai lớp: +1 hoặc -1.
- **Mục tiêu**: Tìm đường phân chia tối ưu giữa hai lớp mà không cho phép lỗi phân loại, đảm bảo tất cả các điểm được phân loại chính xác.
- **Các bước**:
  - Tính ma trận `H` cho bài toán lập trình bậc hai.
  - Giải bài toán lập trình bậc hai bằng `CVXOPT` để tìm các giá trị λ.
  - Tính toán vector trọng số `w` và độ dời `b` dựa trên các vector hỗ trợ.
  - Trực quan hóa đường biên quyết định và biên.

### SVM Biên Mềm
- **Mục tiêu**: Cho phép một số điểm dữ liệu có thể nằm sai biên hoặc nằm trong biên, giới thiệu các biến slack. Điều này hữu ích khi dữ liệu không hoàn toàn phân chia được.
- **Các bước**:
  - Tương tự như biên cứng, nhưng có thêm tham số phạt `C` để cân bằng giữa việc tối đa hóa biên và giảm thiểu lỗi phân loại.
  - Giải bài toán lập trình bậc hai bằng `CVXOPT` để tìm các giá trị λ, w, và b.
  - Trực quan hóa đường biên quyết định và tính toán biên cùng với các biến slack cho các điểm bị phân loại sai.

<a name="HienThiKetQua"></a>
## 3. Hiển Thị Kết Quả

Kết quả bao gồm:
- **Các giá trị λ**: Được hiển thị bên cạnh từng điểm dữ liệu, thể hiện tầm quan trọng của các vector hỗ trợ.
- **Đường biên quyết định**: Một đường thẳng phân chia hai lớp, được tính từ `w` và `b`.
- **Biên**: Vùng giữa hai đường nét đứt, biểu diễn khoảng cách từ các điểm gần nhất của mỗi lớp đến đường phân chia.
- **Các vector hỗ trợ**: Các điểm nằm trên hoặc gần biên.
- **Các biến slack**: Hiển thị trong SVM biên mềm, đại diện cho mức độ sai số phân loại của từng điểm.

### Kết Quả Mẫu

#### Biên Cứng

![image](https://github.com/user-attachments/assets/6f18149e-af9a-469b-98b6-ac5d438dbf9e)

#### Biên Mềm

![image](https://github.com/user-attachments/assets/ebcf68ef-09fd-4932-9cbf-5ddbaae7bcd9)

---

