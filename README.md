# 💬 Analisis Sentimen Aplikasi WhatsApp

## 📌 Deskripsi Proyek

Proyek ini bertujuan untuk melakukan analisis sentimen terhadap komentar pengguna **aplikasi WhatsApp** yang diambil dari **Google Play Store**. Analisis ini bertujuan untuk memahami persepsi, kepuasan, serta keluhan pengguna terhadap aplikasi, yang dapat digunakan untuk perbaikan fitur, strategi pemasaran, dan pengambilan keputusan produk.

---

## 👤 Informasi Kontributor

- **Nama**: Daffa Haidar Farras  
- **Email**: daffahaidarfarras@gmail.com  
- **ID Dicoding**: daffa_haidar  

---


---

## 🧾 Sumber Data

- Data diperoleh dari **komentar pengguna aplikasi WhatsApp di Google Play Store**.
- Format data berupa file teks atau CSV berisi:
  - `Komentar pengguna`
  - Label sentimen manual

---

## 🛠️ Teknologi dan Library

- Python
- Pandas
- NLTK / Sastrawi (untuk preprocessing teks bahasa Indonesia)
- Scikit-learn (untuk klasifikasi)
- WordCloud, Seaborn, Matplotlib (untuk visualisasi)

---

## 🔄 Alur Analisis

1. **Pengumpulan Data**  
   Scraping data ulasan dari Play Store (dapat dilakukan manual atau dengan tools seperti `google-play-scraper`).

2. **Preprocessing Teks**  
   - Case folding
   - Pembersihan simbol dan angka
   - Tokenisasi
   - Normalisasi (slang word -> kata baku)
   - Stopword removal
   - Stemming

3. **Pemberian Label Sentimen**  
   - Positif
   - Negatif
   - Netral  
   (bisa otomatis dengan lexicon-based atau manual)

4. **Ekstraksi Fitur dan Modeling**  
   - TF-IDF Vectorizer
   - Model: SVM

5. **Evaluasi Model**  
   - Akurasi
   - Precision, Recall, F1-Score
   - Confusion Matrix

6. **Visualisasi**  
   - Wordcloud komentar
   - Distribusi sentimen
   - Grafik performa model

---

## 📊 Hasil & Insight

- Mayoritas ulasan menunjukkan sentimen **positif**, namun terdapat sejumlah besar ulasan negatif terutama terkait:
  - Bug teknis
  - Privasi & keamanan
  - Update fitur yang tidak disukai
- WordCloud membantu mengidentifikasi kata kunci dominan dari masing-masing sentimen.

---

## ✅ Kesimpulan

Analisis sentimen ini menunjukkan pentingnya mendengarkan **suara pengguna** melalui ulasan publik. Dengan melakukan klasifikasi dan visualisasi data, tim pengembang bisa:
- Mengenali masalah utama pengguna
- Menentukan prioritas perbaikan fitur
- Meningkatkan kepuasan pelanggan secara data-driven

---

## 📌 Cara Menjalankan

1. Pastikan environment Python (versi 3.8+) telah terpasang.
2. Install dependensi:
   ```bash
   pip install -r requirements.txt


