
### BÀI TOÁN MLP SỬ DỤNG TẬP DỮ LIỆU CIFAR-10

### MỤC LỤC
[1. Công Nghệ Sử Dụng](#CongNgheSuDung)

[2. Thuật Toán](#ThuatToan)

[3. Hiển Thị Kết Quả](#HienThiKetQua)

---

<a name="CongNgheSuDung"></a>
## 1. Công Nghệ Sử Dụng
- **`Pytorch`**: Thư viện học sâu mạnh mẽ giúp xây dựng và huấn luyện các mô hình học máy, cung cấp các lớp và hàm để dễ dàng phát triển mạng nơ-ron.

- **`Numpy`**: Thư viện cơ bản hỗ trợ tính toán ma trận và mảng, hữu ích cho các phép toán số học và thống kê trong quá trình xử lý dữ liệu.

- **`Matplotlib`**: Thư viện dùng để trực quan hóa kết quả, bao gồm biểu đồ mất mát và độ chính xác của mô hình qua các epoch.

- **`Torchvision`**: Thư viện cung cấp các bộ dữ liệu chuẩn và các công cụ biến đổi dữ liệu hình ảnh, hỗ trợ tải và xử lý các tập dữ liệu hình ảnh như CIFAR-10.

<a name="ThuatToan"></a>
## 2. Thuật Toán

### MLP (Multi-Layer Perceptron)
- **Dữ liệu**: Tập dữ liệu CIFAR-10 gồm 60,000 hình ảnh màu 32x32 pixels thuộc 10 lớp khác nhau (chó, mèo, xe hơi, v.v.), với 50,000 ảnh dùng cho huấn luyện và 10,000 ảnh cho kiểm tra.

- **Mục tiêu**: Xây dựng một mô hình MLP để phân loại hình ảnh trong tập dữ liệu CIFAR-10, nhận diện chính xác từng loại hình ảnh.

- **Các bước**:
  - Tiền xử lý dữ liệu: Tải và chuẩn hóa dữ liệu về khoảng từ 0 đến 1 để phù hợp với mô hình.
  - Xây dựng mô hình MLP: Sử dụng các lớp Linear, hàm kích hoạt ReLU, và lớp đầu ra với 10 nút cho các lớp phân loại.
  - Huấn luyện mô hình: Sử dụng phương pháp tối ưu SGD và hàm mất mát CrossEntropy.
  - Đánh giá mô hình: Kiểm tra độ chính xác và mất mát trên tập dữ liệu kiểm tra sau mỗi epoch.

<a name="HienThiKetQua"></a>
## 3. Hiển Thị Kết Quả

Kết quả bao gồm:
- **Đồ thị Mất mát**: Hiển thị sự thay đổi của mất mát huấn luyện và kiểm tra qua các epoch, cho thấy mô hình đang học tốt hay không.
- **Đồ thị Độ chính xác**: Theo dõi độ chính xác của mô hình trên tập kiểm tra qua các epoch.
- **Trọng số Mô hình**: Trọng số của mô hình được lưu trữ để có thể sử dụng lại mà không cần huấn luyện lại.

### Kết Quả Mẫu

#### Đồ Thị Mất Mát

![image](https://github.com/user-attachments/assets/b9344ae8-45a2-4d03-bade-63bc5cbf553f)

#### Đồ Thị Độ Chính Xác

![image](https://github.com/user-attachments/assets/25d9a9ab-2db1-4ff8-8833-5bfe41710980)

---
