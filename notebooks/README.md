# Phân tích điểm thi tốt nghiệp THPT

---

### 📘 Giới thiệu dự án

Dự án này là một phân tích chuyên sâu về điểm thi tốt nghiệp THPT qua các năm từ 2022 đến 2025. Mục tiêu chính là khám phá các xu hướng, đánh giá hiệu suất của thí sinh, và so sánh kết quả giữa các tỉnh thành.

---

### 📊 Nguồn dữ liệu

Dữ liệu được sử dụng trong dự án là các tệp CSV chứa điểm thi tốt nghiệp THPT qua các năm từ 2022 đến 2025. Các tệp này được thu thập và tổng hợp từ dữ liệu công khai trên mạng, do những người thu thập dữ liệu (data crawlers) chia sẻ.
Dữ liệu được sử dụng trong dự án được lưu trữ dưới dạng các tệp CSV trong thư mục Google Drive `diemthi_thpt_2022_2025`. Các tệp bao gồm:
* `diem_thi_thpt_2022.csv`
* `diem_thi_thpt_2023.csv`
* `diem_thi_thpt_2024.csv`
* `20250715-ketquathi-ct2018b.csv`
* `20250715-ketquathi-ct2018a.csv`
* `diem_thi_2025_3.csv`
 
---

### 📈 Các bước phân tích

Quy trình phân tích dữ liệu được thực hiện theo các bước chính sau đây:
1.  **Tải dữ liệu**: Đọc các tệp CSV vào các DataFrame của pandas.
2.  **Làm sạch dữ liệu**: Kiểm tra và xử lý các giá trị null, các giá trị trùng lặp và chuyển đổi kiểu dữ liệu phù hợp.
3.  **Xử lý dữ liệu**: Kết hợp các bộ dữ liệu từ các năm khác nhau, tính toán các điểm tổng hợp và thứ hạng của thí sinh.
4.  **Trực quan hóa dữ liệu**: Tạo ra các biểu đồ và bản đồ để minh họa kết quả phân tích.

---

### 🔍 Kết quả chính và Insight

Dự án đã khám phá nhiều insight quan trọng, được thể hiện rõ qua các biểu đồ:
* **Bản đồ trung vị điểm Toán theo tỉnh**: Cho thấy sự chênh lệch về trình độ Toán học giữa các tỉnh thành trên cả nước.
* **Biểu đồ phân phối điểm thi từng môn học**: Giúp xác định mức độ khó dễ của từng môn và phân bố điểm của thí sinh.
* **Bản đồ số lượng thí sinh top 5% theo tỉnh**: Nổi bật các khu vực có số lượng học sinh xuất sắc cao, phản ánh chất lượng giáo dục tại các địa phương.

---

### ⚙️ Hướng dẫn chạy code

Để chạy code trong file `phan_tich_diem_thi_thpt.ipynb`, bạn cần thực hiện các bước sau:
1.  **Môi trường**: Sử dụng Google Colab để đảm bảo môi trường chạy code tương thích và dễ dàng truy cập.
2.  **Gắn Google Drive**: Chạy đoạn code để kết nối với Google Drive của bạn.
3.  **Thư viện**: Các thư viện cần thiết là `pandas`, `numpy`, `matplotlib`, và `seaborn`.
4.  **Thư mục dữ liệu**: Đặt tất cả các tệp CSV đã tải lên vào một thư mục có tên `diemthi_thpt_2022_2025` trong Google Drive của bạn.
5.  **Thực thi**: Chạy lần lượt các cell code từ trên xuống dưới.