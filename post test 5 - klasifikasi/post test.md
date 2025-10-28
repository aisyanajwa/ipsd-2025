# Analisis Klasifikasi – Dataset Jamur (Mushroom Dataset)

## Tujuan
Tujuan dari analisis ini adalah **memprediksi apakah jamur dapat dimakan atau beracun** berdasarkan karakteristik fisik jamur seperti bentuk tudung, warna insang, permukaan batang, bau, dan lainnya.  
Model klasifikasi akan dibangun menggunakan **K-Nearest Neighbors (KNN)**, **Naive Bayes**, dan **Support Vector Machine (SVM)** untuk memprediksi kategori jamur sebagai variabel target.

---

## Ringkasan Dataset

**Variabel Target (Dependent Variable):**
- `class`: Menunjukkan apakah jamur dapat dimakan (`e`) atau beracun (`p`).

**Fitur Prediktor (Independent Variables):**
- `cap-shape`: Bentuk tudung (bell, convex, flat, dll.)
- `cap-surface`: Permukaan tudung (smooth, scaly, fibrous, dll.)
- `cap-color`: Warna tudung (brown, red, white, yellow, dll.)
- `odor`: Bau jamur (almond, foul, fishy, none, dll.)
- `gill-color`: Warna insang.
- `stalk-shape`, `stalk-color-above-ring`, `stalk-color-below-ring`
- `ring-type`, `spore-print-color`, `population`, `habitat`, dll.

Dataset ini berisi **8124 data jamur** dengan **22 fitur kategorikal** yang menggambarkan ciri fisik jamur dan satu kolom target (`class`).

---

## Tahapan Analisis Berdasarkan Siklus Hidup Data Science

### 1. Pemahaman Masalah (Problem Understanding)
- **Pertanyaan Kunci:**  
  Dapatkah kita memprediksi apakah jamur beracun atau tidak berdasarkan ciri-cirinya?
- **Metrik Utama:**  
  Akurasi, Precision, Recall, dan F1-score.

---

### 2. Pengumpulan Data (Data Collection)
- **Dataset:** `mushrooms.csv`  
  Berisi data jamur dari *UCI Machine Learning Repository*.

---

### 3. Eksplorasi Data (Data Exploration)
Langkah-langkah:
- Memeriksa jumlah data per kelas (edible vs poisonous).
- Melihat distribusi fitur seperti `odor`, `cap-color`, dan `habitat`.
- Membuat visualisasi sederhana seperti:
  - Barplot distribusi kelas (`class`)

---

### 4. Persiapan Data (Data Preparation)
- Mengubah data kategorikal menjadi numerik menggunakan **LabelEncoder**.
- Memisahkan dataset menjadi `X` (fitur) dan `y` (target).
- Membagi data menjadi **training set** dan **testing set**.
- Lakukan standarisasi jika diperlukan.

---

### 5. Pemodelan (Modeling)
Bangun tiga model klasifikasi:
1. **K-Nearest Neighbors (KNN)**
2. **Naive Bayes**
3. **Support Vector Machine (SVM)**

**Langkah-langkah:**
- Latih model pada data training.
- Lakukan prediksi pada data testing.
- Evaluasi hasilnya menggunakan metrik evaluasi.

---

### 6. Evaluasi Model (Model Evaluation)
Gunakan metrik berikut:
- **Akurasi (Accuracy)**
- **Presisi (Precision)**
- **Recall**
- **F1-score**
- **Confusion Matrix**

Bandingkan hasil ketiga model dan analisis mana yang paling baik dalam mendeteksi jamur beracun.
---

## Output yang Diharapkan
- Tabel perbandingan metrik evaluasi dari ketiga model (KNN, Naive Bayes, SVM).  
- Visualisasi confusion matrix.  
- Interpretasi hasil model: fitur mana yang paling berpengaruh terhadap prediksi jamur beracun

---
- Dijelaskan ya dari awal codenya.
---

### Bonus (Nilai Tambah)
Bandingkan hasil akurasi model pada data yang telah **distandarisasi** dan yang **belum distandarisasi**.  
Bagaimana pengaruh standarisasi terhadap performa setiap model (**KNN**, **Naive Bayes**, dan **SVM**)?
Jelaskan alasannya.



