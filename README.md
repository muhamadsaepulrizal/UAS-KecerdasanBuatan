# UAS-KecerdasanBuatan

# 🩺 Prediksi Penyakit Jantung Menggunakan Random Forest

Proyek ini merupakan tugas akhir mata kuliah Kecerdasan Buatan di Institut Teknologi Garut. Tujuan utama dari proyek ini adalah membangun model klasifikasi untuk memprediksi potensi penyakit jantung pada pasien berdasarkan data klinis, menggunakan algoritma Random Forest pada dataset UCI Cleveland.

---

## 📊 Dataset

- Sumber: [Heart Disease UCI – Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- Dataset yang digunakan: `heart_disease_data.csv`
- Jumlah data: 606 baris × 14 kolom
- Fitur yang tersedia meliputi:
  - Usia (`age`)
  - Jenis kelamin (`sex`)
  - Tekanan darah istirahat (`trestbps`)
  - Kolesterol (`chol`)
  - Detak jantung maksimal (`thalach`)
  - Nyeri dada (`cp`)
  - dan fitur lainnya

---

## 🎯 Tujuan Proyek

- Memprediksi apakah seorang pasien berisiko mengidap penyakit jantung berdasarkan data klinis.
- Memberikan insight awal untuk skrining penyakit jantung dengan bantuan model machine learning yang dapat diandalkan.

---

## 🔍 Tahapan Proyek

### 🧪 Exploratory Data Analysis (EDA)
- Histogram: Distribusi usia pasien
- Histogram: Distribusi kolesterol pasien
- Bar chart: Distribusi kelas target (sehat vs sakit)
- Heatmap korelasi antar fitur

### 🧹 Data Preparation
- Pemeriksaan nilai kosong (missing values)
- One-hot encoding untuk fitur kategorikal
- Normalisasi data numerik menggunakan MinMaxScaler
- Split data menjadi train-test (80% : 20%)

### ⚙️ Modeling
- Algoritma: Random Forest Classifier
- Hyperparameter tuning menggunakan GridSearchCV
- Visualisasi feature importance

### 📈 Evaluation
- Confusion matrix
- Classification report:
  - Accuracy
  - Precision
  - Recall
  - F1-Score

---

## 🧠 Algoritma

- Model: RandomForestClassifier
- Library utama: scikit-learn
- Parameter terbaik hasil tuning:
  - n_estimators = 100
  - max_depth = 5 atau None
  - min_samples_split = 2

---

## 🖼️ Visualisasi

- 📊 Histogram: Distribusi usia & kolesterol
- 📊 Bar chart: Distribusi target (0 = sehat, 1 = sakit)
- 🔥 Heatmap: Korelasi antar fitur
- ✅ Confusion matrix
- 🌿 Feature importance (kontribusi tiap fitur)

---

## 🗂️ Struktur Folder

UAS-KecerdasanBuatan/
├── README.md # Deskripsi proyek (file ini)
├── notebook_model.ipynb # Notebook utama untuk analisis dan modeling
├── uas_ai.pdf # File laporan akhir
├── data/
│ ├── jurnal.pdf # Kumpulan 5 jurnal pendukung
│ └── heart_disease_data.csv # Dataset utama
""

---

## 🧾 Hasil Evaluasi Model

| Metrik        | Kelas 0 (Sehat) | Kelas 1 (Sakit) |
|---------------|------------------|------------------|
| Precision     | 0.97             | 1.00             |
| Recall        | 1.00             | 0.97             |
| F1-Score      | 0.98             | 0.98             |
| Accuracy      | ✅ 98.36%         |
