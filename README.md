# Klasifikasi Pelanggan untuk Churn pada Perusahaan XYZ

## Deskripsi Project
Project ini bertujuan untuk memprediksi pelanggan yang berpotensi melakukan **churn** (berhenti menggunakan layanan) dengan menggunakan algoritma klasifikasi biner. Analisis dilakukan untuk membantu perusahaan XYZ dalam memahami pola pelanggan churn dan mengambil langkah strategis untuk mengurangi churn.

## Dataset
Dataset yang digunakan dalam project ini tersedia di Google Drive. Dataset dapat diunduh melalui link berikut:
https://drive.google.com/uc?id=19IfOP0QmCHccMu8A6B2fCUpFqZwCxuzO
Dataset berisi data pelanggan dengan berbagai fitur, seperti informasi demografis dan penggunaan layanan, yang digunakan untuk membangun model klasifikasi.

## Algoritma yang Digunakan
Beberapa algoritma klasifikasi digunakan dalam project ini:
- **K-Nearest Neighbors (KNN)**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **Naive Bayes**

### Analisis Hasil
1. **Random Forest**
   - Memiliki **akurasi tertinggi** sebesar **86.95%**.
   - Precision yang baik (78.45%) menunjukkan kemampuannya untuk memprediksi pelanggan churn dengan benar.
   - F1-Score sebesar **58.24%** menunjukkan keseimbangan antara precision dan recall.
2. **Support Vector Machine (SVM)**
   - Precision tinggi (82.78%) tetapi recall rendah, menunjukkan model ini baik dalam memprediksi churn namun melewatkan banyak pelanggan yang benar-benar churn.
3. **K-Nearest Neighbors (KNN)**
   - Akurasi cukup baik (82.40%) namun recall rendah, artinya model sering gagal mendeteksi churn sebenarnya.
4. **Decision Tree dan Naive Bayes**
   - Kedua model memiliki akurasi dan performa yang lebih rendah dibandingkan dengan Random Forest.

Dari hasil evaluasi ini, **Random Forest** adalah model dengan performa terbaik dan direkomendasikan untuk implementasi lebih lanjut.

## Teknologi yang Digunakan
- Python
- Google Colab
- Scikit-learn (Machine Learning Library)
- Pandas dan NumPy (Data Manipulation)
- Matplotlib dan Seaborn (Visualisasi Data)

## Langkah Penggunaan
1. **Clone repository ini** ke lokal:
   ```bash
   git clone https://github.com/ngeaninurul/churn_binary_classification.git
   ```
2. **Buka project di Google Colab atau Jupyter Notebook**.
3. **Unduh dataset** dengan script yang disediakan di atas.
4. **Jalankan kode** untuk melatih model dan mengevaluasi hasil.

## Struktur Project
```
churn_binary_classification/
│
├── dataset/                             # Folder untuk dataset
├── churn_binary_classification.ipynb    # File notebook (.ipynb)
├── README.md                            # Dokumentasi project
└── requirements.txt                     # Dependencies
```

## Dependencies
Pastikan semua library dalam file requirements.txt sudah terinstal sebelum menjalankan project

## Penutup
Project ini memberikan pemahaman mendalam tentang implementasi algoritma klasifikasi untuk memprediksi pelanggan churn. Hasil menunjukkan bahwa **Random Forest** adalah model yang paling efektif untuk tugas ini. Project ini dapat dikembangkan lebih lanjut dengan mengoptimalkan hyperparameter atau mencoba teknik balancing data untuk meningkatkan performa.
