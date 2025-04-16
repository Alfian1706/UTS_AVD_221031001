# 📊 Consumer Complaints Analysis

Proyek ini bertujuan untuk menganalisis data pengaduan konsumen dan membangun model prediktif untuk mengidentifikasi kemungkinan terjadinya dispute (perselisihan) berdasarkan data laporan yang masuk. Dengan memahami pola-pola ini, perusahaan dapat merespons lebih cepat dan meningkatkan kualitas layanan pelanggan.

---

## 📁 Dataset
Dataset yang digunakan berasal dari sumber terbuka, yaitu **Consumer Complaints**, yang memuat data keluhan pelanggan terkait layanan finansial. Kolom-kolom penting dalam dataset antara lain:
- `product`, `sub_product`
- `issue`, `sub_issue`
- `company`, `state`
- `submitted_via`, `date_received`, `company_response_to_consumer`
- `consumer_disputed?` *(variabel target)*

---

## ⚙️ Metodologi
### 1. Data Preparation
- Menghapus kolom dengan nilai kosong berlebihan (>20% missing values)
- Menghapus baris yang masih memiliki missing value
- Encoding untuk data kategorikal
- Normalisasi menggunakan `StandardScaler`

### 2. Modeling
Beberapa model supervised learning digunakan untuk membangun sistem prediktif terhadap kemungkinan terjadinya dispute:
- Logistic Regression
- Decision Tree
- Naive Bayes
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)

### 3. Evaluasi Model
Evaluasi dilakukan menggunakan metrik:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Model terbaik dipilih berdasarkan performa evaluasi terhadap data uji.

---

## 📈 Hasil
- Setiap model menunjukkan performa yang berbeda terhadap data uji.
- Model terbaik menunjukkan akurasi yang tinggi dan distribusi prediksi yang seimbang.
- Fitur-fitur tertentu seperti jenis produk, metode pengajuan, dan perusahaan memiliki korelasi yang signifikan terhadap kemungkinan dispute.

---

## ✅ Kesimpulan
Proyek ini berhasil menunjukkan bahwa data pengaduan konsumen dapat dianalisis untuk membangun sistem prediktif yang membantu dalam mengantisipasi potensi dispute. Model yang dibangun dapat digunakan untuk meningkatkan kualitas layanan, pengambilan keputusan yang lebih cepat, dan efisiensi penanganan keluhan.

---

## 🚀 Pengembangan Selanjutnya
- Menambahkan NLP untuk menganalisis narasi keluhan konsumen
- Menggunakan teknik balancing untuk menangani dataset yang tidak seimbang
- Menerapkan pendekatan ensemble seperti Random Forest atau XGBoost
- Membuat dashboard interaktif untuk visualisasi hasil

---

## 📚 Library yang Digunakan
- `pandas`, `numpy`
- `matplotlib`, `seaborn`
- `scikit-learn`

---

## ✍️ Author
Proyek ini dikembangkan sebagai bagian dari tugas analisis data menggunakan metode supervised learning.

