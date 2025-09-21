# 💰 Medical Insurance Cost Prediction

## 📌 Deskripsi
Project ini bertujuan untuk melakukan **prediksi biaya asuransi medis** berdasarkan faktor-faktor demografis dan gaya hidup responden. Dengan memanfaatkan algoritma *machine learning* berbasis regresi, project ini berupaya menemukan model terbaik yang mampu memprediksi biaya asuransi dengan akurasi tinggi.

Beberapa algoritma yang digunakan:
- 👥 **K-Nearest Neighbors (KNN)**  
- 🌳 **Random Forest**  
- 🚀 **Gradient Boosting**  
- 🧠 **Neural Network (MLP)**  

---

## 📂 Dataset
### 📑 Sumber Data  
Dataset diperoleh dari **Kaggle**:  
🔗 [Medical Cost Personal Dataset – Kaggle](https://www.kaggle.com/datasets/mirichoi0218/insurance)  

### 📊 Keterangan Data  
Beberapa variabel utama yang digunakan:  
- **Age** → Usia tertanggung  
- **Sex** → Jenis kelamin  
- **BMI** → Indeks massa tubuh  
- **Children** → Jumlah anak yang ditanggung asuransi  
- **Smoker** → Status perokok  
- **Region** → Wilayah tempat tinggal  
- **Charges** → Biaya asuransi medis (variabel target)  

---

## 🧹 Tahapan Analisis
1. **Definisi Library** 📚  
   Mengimpor library Python seperti `pandas`, `numpy`, `matplotlib`, `seaborn`, dan `scikit-learn`.  
2. **Baca Dataset** 📂  
   Membaca data mentah dan memahami struktur dataset.  
3. **Pembersihan Data** 🧹  
   - Cek nilai kosong (missing values)  
   - Penghapusan data duplikat jika ada  
4. **EDA (Exploratory Data Analysis)** 🔎  
   - Distribusi biaya asuransi berdasarkan usia, BMI, status perokok, jumlah anak, dan region  
   - Analisis korelasi antar variabel numerik  
5. **Preprocessing Data** ⚙️  
   - Encoding variabel kategorikal (sex, smoker, region)  
   - Normalisasi data numerik jika diperlukan  
   - Split dataset menjadi data latih dan data uji  
6. **Implementasi Model** 🤖  
   Menerapkan empat algoritma utama:  
   - 👥 **K-Nearest Neighbors (KNN)**  
   - 🌳 **Random Forest**  
   - 🚀 **Gradient Boosting**  
   - 🧠 **Neural Network (MLP)**  
7. **Evaluasi Model** 📈  
   Menggunakan metrik evaluasi:  
   - **R² (Coefficient of Determination)**  
   - **MAE (Mean Absolute Error)**  
   - **MSE (Mean Squared Error)**  

---

## 📊 Hasil
Berikut hasil performa masing-masing model:

| Model                  | R² (%) | MAE     | MSE          |
|-------------------------|--------|---------|--------------|
| K-Nearest Neighbors     | 4.98   | 8896.22 | 174609724.58 |
| Random Forest           | 88.34  | 2555.93 | 21420846.46  |
| Gradient Boosting       | 90.11  | 2508.42 | 18170259.11  |
| Neural Network (MLP)    | 13.95  | 9604.94 | 158125880.36 |

---

## 🏆 Conclusion
### Alasan Pemilihan Model Terbaik
Berdasarkan hasil di atas, **Gradient Boosting** dipilih sebagai algoritma terbaik karena:  
- Memiliki **R² tertinggi (90.11%)**, menunjukkan kemampuan terbaik dalam menjelaskan variansi data.  
- Memberikan **error terkecil (MAE & MSE)**, sehingga prediksi lebih akurat dan stabil.  
- Lebih konsisten dibanding model lain, terutama dalam menangani kompleksitas data.  

Dengan demikian, Gradient Boosting menjadi model paling andal dalam kasus **prediksi biaya asuransi medis** pada dataset ini.
