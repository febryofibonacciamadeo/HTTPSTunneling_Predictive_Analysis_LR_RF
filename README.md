# HTTPS Tunneling Predictive Analysis (LR & RF)

Analisis prediktif untuk mendeteksi/mengklasifikasikan trafik **HTTPS Tunneling** menggunakan algoritma **Logistic Regression (LR)** dan **Random Forest (RF)**.

## Deskripsi

HTTPS Tunneling adalah teknik yang dapat digunakan untuk menyembunyikan trafik jaringan (termasuk aktivitas mencurigakan) di dalam koneksi HTTPS yang terenkripsi, sehingga sulit dideteksi oleh sistem keamanan konvensional. Proyek ini membangun model *machine learning* untuk melakukan analisis prediktif terhadap data trafik jaringan guna mengidentifikasi indikasi HTTPS tunneling, dengan membandingkan performa dua algoritma klasifikasi:

- **Logistic Regression (LR)**
- **Random Forest (RF)**

## Struktur Repository

```
HTTPSTunneling_Predictive_Analysis_LR_RF/
└── code.ipynb   # Notebook utama: preprocessing data trafik, training, evaluasi model
```

## Alur Kerja (Workflow)

1. **Data Loading:** memuat data trafik jaringan/fitur koneksi HTTPS.
2. **Data Preprocessing:** pembersihan data, encoding fitur kategorikal, normalisasi/standardisasi fitur numerik.
3. **Exploratory Data Analysis (EDA):** eksplorasi pola/fitur yang membedakan trafik normal vs. tunneling.
4. **Model Training:** melatih model Logistic Regression dan Random Forest pada data yang telah diproses.
5. **Evaluation:** membandingkan performa kedua model menggunakan metrik seperti accuracy, precision, recall, F1-score, dan confusion matrix.
6. **Analisis Hasil:** interpretasi fitur penting (feature importance) yang berkontribusi pada deteksi HTTPS tunneling, khususnya dari model Random Forest.

## Library yang Digunakan

- Python
- Jupyter Notebook
- scikit-learn (Logistic Regression, Random Forest, metrik evaluasi)
- pandas & numpy
- matplotlib/seaborn (visualisasi data & hasil)

## Cara Menjalankan

1. Clone repository ini:
   ```bash
   git clone https://github.com/febryofibonacciamadeo/HTTPSTunneling_Predictive_Analysis_LR_RF.git
   cd HTTPSTunneling_Predictive_Analysis_LR_RF
   ```
2. Install dependensi:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn jupyter
   ```
3. Jalankan notebook:
   ```bash
   jupyter notebook code.ipynb
   ```

## Hasil

Perbandingan performa model Logistic Regression vs Random Forest dalam mendeteksi HTTPS tunneling, lengkap dengan metrik evaluasi dan visualisasi. Lihat `code.ipynb` untuk detail lengkap.
