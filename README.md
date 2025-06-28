# 🚗 Used Car Price Regression

Proyek ini bertujuan untuk memprediksi harga mobil bekas berdasarkan fitur-fitur kendaraan. Proyek ini menggunakan pendekatan regresi dan beberapa algoritma machine learning, serta melakukan feature engineering dan EDA untuk mendapatkan performa terbaik.

## 📌 Informasi Umum

- **Nama Proyek:** Used Car Price Regression
- **Nama Pembuat:** Masmur Toloni Harefa
- **Dataset:** [Kaggle - Playground Series S4E9](https://www.kaggle.com/competitions/playground-series-s4e9/)

---

## 🗂️ Dataset Overview

Dataset terdiri dari data kendaraan bekas dengan fitur-fitur seperti:

- `brand`: Merek mobil
- `model`: Model kendaraan
- `fuel_type`: Jenis bahan bakar
- `engine`: Kapasitas/jenis mesin
- `transmission`: Jenis transmisi
- `ext_color`: Warna luar kendaraan
- `int_color`: Warna dalam kendaraan
- `accident`: Riwayat kecelakaan (biner)
- `clean_title`: Status legalitas kendaraan (biner)
- `price`: Harga kendaraan (target regresi)

---

## 🔍 Exploratory Data Analysis (EDA)

Beberapa hasil dari analisis data:

- Jumlah merek (`brand`): 57
- Jumlah model unik (`model`): 1.897
- `fuel_type`: 7 jenis unik, namun banyak data hilang
- `engine`: 1.117 nilai unik dalam format teks (perlu rekayasa fitur)
- `transmission`: 52 jenis (perlu disederhanakan, misalnya 'A/T' dan '7-Speed A/T')
- `ext_color`: 319 warna unik
- `int_color`: 156 warna unik
- `accident`: Banyak missing values
- `clean_title`: Bernilai biner

---

## ⚙️ Feature Engineering

- **Fuel Type:** Normalisasi nama bahan bakar
- **Engine:** Ekstraksi kapasitas mesin jika memungkinkan
- **Transmission:** Penyederhanaan jenis transmisi
- **Missing Value Handling:** Imputasi untuk kolom `accident`, dll
- **Encoding:** Label encoding atau freq encoding untuk fitur kategorikal

---

## 🤖 Model yang Digunakan

| Model               | Deskripsi                          |
|---------------------|------------------------------------|
| Random Forest       | Model ensemble berbasis decision tree |
| XGBoost             | ✅ **Model terbaik** berdasarkan evaluasi |
| CatBoost            | Cocok untuk fitur kategorikal, namun performa sedikit di bawah XGBoost |

---

## ✅ Kesimpulan

- Model **XGBoost** memberikan performa terbaik dalam prediksi harga mobil bekas.
- Feature engineering memainkan peran penting dalam peningkatan akurasi model.
- Proyek ini cocok untuk dijadikan portofolio bagi praktisi pemula di bidang Data Science khususnya regresi.

---

## 🧪 Cara Menjalankan

1. Clone repo ini
2. Pastikan dependensi seperti `pandas`, `xgboost`, `catboost`, `matplotlib`, dll sudah terinstal
3. Jalankan notebook `UsedCarPriceRegression.ipynb` di Jupyter Notebook atau Google Colab

---

---

## 🏆 Kompetisi & Pencapaian

Proyek ini diikutsertakan dalam kompetisi **[Kaggle Playground Series - Season 4, Episode 9](https://www.kaggle.com/competitions/playground-series-s4e9/)**.
![image](https://github.com/user-attachments/assets/98a4453b-b498-4c47-9173-0cdd37ce7a9a)


- 📈 **Score (RMSE):** `63650.27387`
- 🏅 **Peringkat:** Top 50 secara global (Late Submission)
- 👥 **Statistik Peserta:**
  - 9,606 Total Entrants
  - 3,306 Active Participants
  - 3,066 Teams
- ⏱️ Kompetisi telah **berakhir**, namun skor didapat melalui **pengumpulan terlambat (late submission)** yang tetap dievaluasi oleh sistem leaderboard Kaggle.

Meskipun bukan submission resmi kompetisi, hasil ini menunjukkan bahwa model ini sangat kompetitif dan mampu bersaing di level global.


## 📧 Kontak

Untuk pertanyaan atau kolaborasi, silakan hubungi:

**Masmur Toloni Harefa**  
Email: masmurharefa03@gmail.com  

---

