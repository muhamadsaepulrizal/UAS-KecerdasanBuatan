# UAS-KecerdasanBuatan

🩺 Prediksi Penyakit Jantung Menggunakan Random Forest
Proyek ini merupakan tugas akhir mata kuliah Kecerdasan Buatan di Institut Teknologi Garut. Tujuannya adalah membangun model prediksi penyakit jantung berdasarkan data medis menggunakan algoritma Random Forest pada dataset UCI Cleveland.

📊 Dataset
Sumber: Heart Disease UCI - Kaggle

Dataset yang digunakan: heart_disease_data.csv

Jumlah data: 606 baris × 14 kolom

Fitur yang tersedia meliputi: usia, jenis kelamin, tekanan darah istirahat, kolesterol, detak jantung maksimal, dan lain-lain

🎯 Tujuan Proyek
Memprediksi apakah seorang pasien berisiko mengidap penyakit jantung berdasarkan data klinis.

Membantu memberikan insight awal untuk proses skrining medis dengan model machine learning.

🔍 Tahapan Proyek
Exploratory Data Analysis (EDA)

Visualisasi histogram usia dan kolesterol

Bar chart distribusi kelas target

Heatmap korelasi antar fitur

Data Preparation

Pemeriksaan nilai kosong

One-hot encoding

Normalisasi menggunakan MinMaxScaler

Split data train-test (80:20)

Modeling

Algoritma: Random Forest Classifier

Hyperparameter tuning dengan GridSearchCV

Visualisasi feature importance

Evaluation

Confusion matrix

Classification report (accuracy, precision, recall, f1-score)

Accuracy akhir model: 98.36%

🧠 Algoritma
Model: RandomForestClassifier

Library utama: scikit-learn

Parameter terbaik:

n_estimators = 100

max_depth = 5 atau None

min_samples_split = 2

🖼️ Visualisasi
📌 Histogram: Distribusi usia & kolesterol pasien

📌 Bar chart: Distribusi target (0 = sehat, 1 = sakit)

📌 Heatmap korelasi antar fitur

📌 Confusion matrix & feature importance

🗂️ Struktur Folder

UAS-KecerdasanBuatan/
├── README.md                      # Deskripsi proyek (file ini)
├── notebook_model.ipynb           # Notebook utama untuk analisis dan modeling
├── uas_ai.pdf                     # File laporan
├── data/                        
│   ├── jurnal.pdf                 # 5 jurnal yang digunakan sebagai referensi
│   └── heart_disease_data.csv     # dataset yang digunakan


🧾 Hasil Evaluasi
Accuracy: 98.36%

Precision: 1.00 (positif), 0.97 (negatif)

Recall: 0.97 (positif), 1.00 (negatif)

F1-Score: 0.98


