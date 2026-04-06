# Phát hiện Fake News với Python

> Dự án Machine Learning sử dụng **TfidfVectorizer** và **PassiveAggressiveClassifier** để tự động phân loại tin tức thật/giả với độ chính xác cao (~97.86%).

## Tính năng

- Phân loại tin tức là **REAL** hay **FAKE** dựa trên nội dung, tiêu đề và tác giả.
- Sử dụng kỹ thuật **TF-IDF** để trích xuất đặc trưng văn bản.
- Mô hình **PassiveAggressiveClassifier** – thuật toán học máy trực tuyến hiệu quả.
- Trực quan hóa dữ liệu: biểu đồ phân bố tin thật/giả, ma trận nhầm lẫn (Confusion Matrix).
- Hỗ trợ test nhanh với bài báo bất kỳ (input thủ công qua notebook).
- Độ chính xác mô hình: **97.86%** trên tập test.

## Công nghệ sử dụng

- **Ngôn ngữ**: Python
- **Thư viện chính**:
  - `pandas` – Xử lý dữ liệu
  - `scikit-learn` – TfidfVectorizer, PassiveAggressiveClassifier, train_test_split, accuracy_score, confusion_matrix
  - `matplotlib` & `seaborn` – Trực quan hóa
- **Môi trường**: Jupyter Notebook

## Tập dữ liệu

- Nguồn: `news.csv` (dựa trên tập `train.csv` từ cuộc thi Fake News trên Kaggle)
- Số lượng: 20.800 bài báo (khoảng 50% thật – 50% giả)
- Các cột: `id`, `title`, `author`, `text`, `label` (0 = REAL, 1 = FAKE)

## Cài đặt

### Yêu cầu
- Python 3.8+
- Jupyter Notebook
