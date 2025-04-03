# 📈 Ứng Dụng Machine Learning Dự Đoán Giá Cổ Phiếu Các Công Ty Chứng Khoán Việt Nam  

## 📌 **Tổng Quan Dự Án**  
Dự án này nhằm nghiên cứu và so sánh độ chính xác của các mô hình **CNN, BiLSTM, LSTM, Hồi quy tuyến tính (Linear Regression) và XGBoost** khi áp dụng vào dữ liệu thị trường chứng khoán Việt Nam. Mục tiêu là tìm ra mô hình tối ưu nhất để dự đoán biến động giá cổ phiếu.  

---

## 📂 **Cấu Trúc Thư Mục**  
```
📦 stock-price-prediction
├── 📂 data                # Thư mục chứa dữ liệu
│   ├── HCM.csv
│   ├── SSI.csv
│   ├── VCI.csv
│   ├── VND.csv
├── 📂 models              # Thư mục chứa các mô hình Machine Learning
│   ├── CNN.ipynb
│   ├── CNN_BiLSTM.ipynb
│   ├── LN_LSTM.ipynb
│   ├── LSTM.ipynb
│   ├── Linear_Regression.ipynb
│   ├── XgBoost.ipynb
├── 📂 reports             # Thư mục chứa báo cáo, kết quả phân tích
│   ├── Tổng quan giới thiệu các công ty.md
│   ├── Đánh giá mô hình.md
├── README.md              # File mô tả dự án
├── requirements.txt       # Các thư viện cần cài đặt
└── main.py                # File chạy chính của dự án (nếu có)
```

---

## 🔹 **Tính Năng Chính**
- Dự báo giá cổ phiếu dựa trên dữ liệu lịch sử.
- So sánh hiệu suất giữa các mô hình khác nhau.
- Đánh giá kết quả dự đoán bằng các chỉ số: MAE, MSE, RMSE, R².
- Visualization dữ liệu bằng biểu đồ trực quan.

---

## 🔧 **Cài Đặt & Sử Dụng**
### 1️⃣ Clone repository từ GitHub về máy
```bash
git clone https://github.com/yourusername/stock-price-prediction.git
cd stock-price-prediction
```
### 2️⃣ Cài đặt thư viện cần thiết
```bash
pip install -r requirements.txt
```
### 3️⃣ Chạy Jupyter Notebook và mở các file trong thư mục models
```bash
jupyter notebook
```
### 4️⃣ Hoặc chạy trực tiếp bằng Python (nếu có file `.py`)
```bash
python main.py
```

---

## 📊 **Kết Quả & Nhận Định**
- **LSTM và XGBoost** là hai mô hình có hiệu suất tốt nhất khi dự đoán xu hướng giá cổ phiếu.
- **Hồi quy tuyến tính** hoạt động kém hơn do không xử lý tốt quan hệ phi tuyến tính.
- **CNN_BiLSTM** có tiềm năng nhưng yêu cầu tài nguyên tính toán lớn hơn.

---

## 🏆 **Kết Luận & Hướng Phát Triển**
📌 **Kết quả đạt được**
- Ứng dụng thành công Machine Learning để dự đoán giá cổ phiếu của các công ty lớn trên sàn HOSE.
- So sánh hiệu suất của các mô hình và tìm ra phương pháp tối ưu.

📌 **Hạn chế của nghiên cứu**
- Chỉ sử dụng dữ liệu từ một số công ty lớn, chưa mở rộng sang các thị trường khác.
- Các mô hình vẫn gặp khó khăn trong việc dự đoán các biến động mạnh của thị trường.

📌 **Định hướng phát triển**
- Nâng cấp mô hình bằng các phương pháp tiên tiến như Transformer và Attention Mechanism.
- Mở rộng tập dữ liệu để tăng tính chính xác và khả năng tổng quát.
- Kết hợp phân tích dữ liệu từ mạng xã hội, AI để cải thiện dự đoán.

📌 **Ứng dụng thực tiễn**
- Hỗ trợ công ty chứng khoán và quỹ đầu tư trong việc tối ưu hóa danh mục đầu tư.
- Ứng dụng trong ngân hàng để quản lý rủi ro tài chính.
- Có thể mở rộng để tích hợp Machine Learning với các yếu tố kinh tế vĩ mô nhằm đưa ra các dự đoán chính xác hơn về thị trường tài chính.

