# 📈 Ứng Dụng Machine Learning Dự Đoán Giá Cổ Phiếu Các Công Ty Chứng Khoán Việt Nam  

## 📌 Tổng Quan Dự Án  
Dự án này nhằm nghiên cứu và so sánh độ chính xác của các mô hình **CNN, BiLSTM, LSTM, Hồi quy tuyến tính (Linear Regression) và XGBoost** khi áp dụng vào dữ liệu thị trường chứng khoán Việt Nam. Mục tiêu là tìm ra mô hình tối ưu nhất để dự đoán biến động giá cổ phiếu.  

---

## 📂 Cấu Trúc Thư Mục  
```plaintext
📦 stock-price-prediction
👉 📂 data                # Thư mục chứa dữ liệu
   ┗📄 HCM.csv
   ┗📄 SSI.csv
   ┗📄 VCI.csv
   ┗📄 VND.csv
👉 📂 main code           # Thư mục chứa các mô hình Machine Learning
   ┗📁 CNN_.ipynb
   ┗📁 CNN_BiLSTM.ipynb
   ┗📁 LN_LSTM.ipynb
   ┗📁 LSTM.ipynb
   ┗📁 Linear_Regression.ipynb
   ┗📁 XgBoost.ipynb
   ┗📁 Tổng quan giới thiệu các công ty...
👉 README.md              # File mô tả dự án
👉 requirements.txt       # Các thư viện cần cài đặt
🔹 ## Tính Năng Chính
✅ ## Dữ liệu
Sử dụng dữ liệu giá cổ phiếu lịch sử của các công ty chứng khoán Việt Nam: HCM, SSI, VCI, VND.

Các đặc trưng chính: Giá mở cửa, Giá đóng cửa, Giá cao nhất, Giá thấp nhất.

✅ ## Mô hình Machine Learning
CNN.ipynb: Mô hình Convolutional Neural Network.

CNN_BiLSTM.ipynb: Kết hợp CNN và BiLSTM để phân tích chuỗi thời gian.

LN_LSTM.ipynb: Kết hợp Linear Regression và LSTM để dự đoán giá cổ phiếu.

LSTM.ipynb: Mô hình LSTM truyền thống cho dự đoán chuỗi thời gian.

Linear_Regression.ipynb: Hồi quy tuyến tính đơn giản để tạo baseline.

XgBoost.ipynb: Mô hình XGBoost để dự đoán giá cổ phiếu.

✅ ## Kỹ thuật tối ưu hóa mô hình
K-Fold Cross Validation để đánh giá độ chính xác.

EarlyStopping và ModelCheckpoint để cải thiện hiệu suất.

Đánh giá bằng các chỉ số: MAE, MSE, RMSE, R².

##🔧  **Cài Đặt & Sử Dụng**
1.**Clone repository từ GitHub về máy**

bash
git clone https://github.com/yourusername/stock-price-prediction.git
cd stock-price-prediction

2.**Cài đặt thư viện cần thiết**

bash
pip install -r requirements.txt

3.**Chạy Jupyter Notebook và mở các file trong thư mục main code**

bash
jupyter notebook

4.**Hoặc chạy trực tiếp bằng Python (nếu có file .py)**

bash
python main.py

##📊**Kết Quả & Nhận Định**
**LSTM và XGBoost** là hai mô hình có hiệu suất tốt nhất khi dự đoán xu hướng giá cổ phiếu.

**Hồi quy tuyến tính** hoạt động kém hơn do không xử lý tốt quan hệ phi tuyến tính.

**CNN_BiLSTM** có tiềm năng nhưng yêu cầu tài nguyên tính toán lớn hơn.

##🏆 **Kết Luận & Hướng Phát Triển**
📌**Kết quả đạt được**
Nghiên cứu đã áp dụng và tối ưu các mô hình học máy (LSTM, CNN, XGBoost, Linear Regression) cũng như các mô hình kết hợp (Linear Regression + LSTM, CNN + BiLSTM) để dự đoán giá cổ phiếu. Mô hình kết hợp Linear Regression + LSTM và CNN + BiLSTM cho kết quả dự đoán tốt nhất.

📌 **Hạn chế của nghiên cứu**
Dữ liệu: Chỉ giới hạn trong các công ty lớn trên sàn HOSE, thiếu dữ liệu từ các công ty nhỏ hoặc quốc tế.

Mô hình: Chưa xử lý tốt các tình huống thị trường biến động mạnh.

Tài nguyên tính toán: Hạn chế trong việc triển khai các mô hình sâu trên tập dữ liệu lớn.

📌 **Định hướng phát triển**
Áp dụng mô hình tiên tiến như Transformer và Attention Mechanism để cải thiện khả năng xử lý chuỗi thời gian.

Mở rộng dữ liệu từ nhiều thị trường khác nhau để kiểm chứng tính tổng quát của mô hình.

Tích hợp dữ liệu từ AI, IoT, phân tích mạng xã hội để nâng cao độ chính xác.

Sử dụng kỹ thuật Time Series Split để đảm bảo mô hình học được xu hướng dài hạn và giảm thiểu lỗi dự đoán.

📌 **Ứng dụng thực tiễn**
Hỗ trợ công ty chứng khoán và quỹ đầu tư trong việc ra quyết định tối ưu hóa danh mục đầu tư.

Ngân hàng và tổ chức tài chính có thể áp dụng để quản lý rủi ro và nâng cao hiệu quả đầu tư.

Nghiên cứu có thể mở rộng để tích hợp machine learning với các yếu tố kinh tế vĩ mô nhằm cung cấp cái nhìn toàn diện hơn về thị trường tài chính.
