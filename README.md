# 🚦 Prediksi Risiko Kecelakaan Menggunakan Algoritma Random Forest

Proyek ini merupakan notebook machine learning yang bertujuan untuk memprediksi tingkat risiko kecelakaan berdasarkan data kecelakaan lalu lintas global. Algoritma utama yang digunakan adalah **Random Forest Classifier**, dengan fokus pada preprocessing, evaluasi model, dan optimasi hyperparameter.

---

## 📁 Dataset

Dataset yang digunakan berasal dari Kaggle:

[`adilshamim8/global-traffic-accidents-dataset`](https://www.kaggle.com/datasets/adilshamim8/global-traffic-accidents-dataset)

Dataset ini diunduh otomatis melalui library **kagglehub** dan dimuat dalam format `.csv`.

---

## 🧹 Preprocessing Data

Langkah-langkah preprocessing yang dilakukan meliputi:

- Pengecekan tipe data dan informasi dasar menggunakan `df.info()`
- Identifikasi dan penanganan missing values
- Encoding kolom kategorikal dengan `LabelEncoder`
- Penyesuaian class imbalance menggunakan `compute_class_weight` dari `sklearn.utils`

---

## ⚙️ Model Machine Learning

- **Model**: `RandomForestClassifier` dari `scikit-learn`
- **Validasi**: `StratifiedKFold` untuk memastikan distribusi kelas tetap seimbang di setiap fold
- **Optimasi Hyperparameter**: `RandomizedSearchCV` untuk mempercepat pencarian parameter terbaik

---

## 📊 Evaluasi Model

Model dievaluasi menggunakan metrik-metrik berikut:

- `Accuracy Score`
- `F1 Score`
- `ROC AUC Score`
- `Confusion Matrix`
- Visualisasi menggunakan `ConfusionMatrixDisplay` dan `seaborn`

---

## 🛠️ Tools dan Library

Library utama yang digunakan antara lain:

- `pandas`, `numpy`
- `matplotlib.pyplot`, `seaborn`
- `sklearn` (scikit-learn)
- `kagglehub` (untuk pengambilan dataset)
- `joblib` (untuk menyimpan model)
- `warnings` (untuk suppress warning output)

---

## 🚀 Cara Menjalankan

1. Buka file `.ipynb` ini di Google Colab atau Jupyter Notebook.
2. Pastikan semua dependensi telah diinstal.
3. Jalankan setiap sel secara berurutan.
4. File CSV akan otomatis diunduh dari Kaggle saat sel pertama dijalankan.
5. Hasil akhir akan menampilkan skor model dan visualisasi evaluasi.

---

## 📦 Output

- Hasil evaluasi model
- Grafik confusion matrix dan ROC curve
- Model tersimpan dalam format `.pkl` (via `joblib`)

---

## 🔗 Open in Colab

Kamu bisa langsung membuka dan menjalankan notebook ini di Google Colab dengan mengklik badge berikut:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Nizaru-gpt/Natashop/blob/main/Prediksi_Risiko_Kecelakaan_Menggunakan_Algoritma_Random_Forest.ipynb)

---

## 📝 Catatan Tambahan

- Dataset besar: disarankan menjalankan notebook di **Google Colab** dengan koneksi internet stabil.
- Jika menggunakan notebook lokal, pastikan kamu memiliki **Kaggle API key** dan library `kagglehub` sudah terpasang.

---

## 📬 Kontak

Jika ada pertanyaan atau masukan, silakan hubungi melalui [GitHub Issues](https://github.com/Nizaru-gpt/Natashop/issues).

