# IoV-Intelligent-IDS-Tree-Based

[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Machine Learning](https://img.shields.io/badge/Machine-Learning-orange.svg)](https://scikit-learn.org/)
[![Cybersecurity](https://img.shields.io/badge/Cybersecurity-IoV-red.svg)](https://arxiv.org/abs/1910.08635)

Hệ thống phát hiện xâm nhập (IDS) thông minh cho mạng xe tự hành (IoV) dựa trên các mô hình học máy cấu trúc cây. Dự án được triển khai, kế thừa và cải tiến từ bài báo khoa học: **"Tree-based Intelligent Intrusion Detection System in Internet of Vehicles"** (IEEE GlobeCom 2019).



---

## 📑 Mục lục
1. [Giới thiệu chung](#-giới-thiệu-chung)
2. [Cấu trúc thư mục](#-cấu-trúc-thư-mục)
3. [Dòng chảy hệ thống & Phân công (Mapping)](#-dòng-chảy-hệ-thống--phân-công-mapping)
4. [Tập dữ liệu sử dụng](#-tập-dữ-liệu-sử-dụng)
5. [Hướng dẫn cài đặt](#-hướng-dẫn-cài-đặt)
6. [Các điểm cải tiến so với Paper gốc](#-các-điểm-cải-tiến-so-với-paper-gốc)

---

## 📝 Giới thiệu chung
Dự án giải quyết bài toán an ninh mạng cho xe thông minh ở hai cấp độ: mạng nội bộ (**CAN bus**) và mạng bên ngoài (**V2X**). Chúng tôi sử dụng các thuật toán Ensemble Learning (XGBoost, Random Forest, Extra Trees) kết hợp cơ chế **Stacking** để tối ưu hóa khả năng phát hiện các cuộc tấn công như DoS, Spoofing và Fuzzy với độ chính xác tiệm cận 100%.



---

## 📁 Cấu trúc thư mục
```text
/IoV-Intelligent-IDS-Tree-Based
│
├── /data               # Chứa CICIDS2017 và Car-Hacking Dataset
├── /notebooks          # Luồng xử lý chi tiết theo từng giai đoạn
│   ├── 01_Preprocessing_Dang.ipynb
│   ├── 02_Feature_Engineering_Khoa.ipynb
│   ├── 03_Modeling_Tuning_Hung.ipynb
│   └── 04_Evaluation_Minh.ipynb
├── /src                # Các script Python hỗ trợ xử lý đặc thù
├── README.md           # Tài liệu hướng dẫn này
└── requirements.txt    # Danh sách thư viện cần thiết
