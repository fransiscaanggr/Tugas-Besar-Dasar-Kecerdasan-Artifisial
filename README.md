# Tugas-Besar-Dasar-Kecerdasan-Artifisial
Prediksi Hujan Menggunakan Fuzzy System (Mamdani &amp; Sugeno)

📌 Deskripsi Proyek
Proyek ini merupakan implementasi sistem prediksi hujan menggunakan Fuzzy Inference System (FIS) dengan dua metode utama:
- Metode Mamdani (output linguistik, mendekati penalaran manusia)
- Metode Sugeno (output linear, lebih efisien secara komputasi)
Sistem ini memprediksi kemungkinan hujan besok berdasarkan parameter cuaca hari ini seperti suhu, kelembaban, kecepatan angin, curah hujan, tutupan awan, dan tekanan atmosfer.

📊 Dataset
Dataset diambil dari Kaggle (usa_rain_prediction_dataset_2024_2025.csv) yang berisi data cuaca harian dari 20 kota besar di Amerika Serikat (2024-2025).
- Total data asli: 73.100
- Data sampel yang digunakan: 1.000 (diseimbangkan: 500 hujan / 500 tidak hujan)
- Variabel input:
  1. Suhu
  2. Kelembaban
  3. Kecepatan Angin
  4. Curah Hujan
  5. Tutupan Awan
  6. Tekanan
- Target: Rain Tomorrow (1 = Ya, 0 = Tidak)

🧠 Metodologi
- Preprocessing Data
  1. Pemilihan sampel acak
  2. Penyeimbangan kelas
  3. Eksplorasi statistik dan visualisasi
- Fuzzifikasi
  1. Mendefinisikan variabel linguistik (contoh: Suhu → Dingin, Sedang, Panas)
  2. Menetapkan fungsi keanggotaan (membership function)
- Inferensi Fuzzy
  1. Pembuatan aturan IF-THEN berdasarkan domain pengetahuan
  2. Penerapan metode Mamdani dan Sugeno
- Defuzzifikasi
  1. Mamdani: Metode centroid
  2. Sugeno: Weighted average
- Evaluasi Model
  1. Akurasi, Presisi, Recall, F1-Score
  2. Confusion Matrix

📈 Hasil
Kedua metode menunjukkan performa yang mirip dengan akurasi sekitar 74%. Metode Sugeno sedikit lebih unggul secara konsisten dalam semua metrik evaluasi.
- Mamdani: Output lebih interpretatif, mendekati logika manusia
- Sugeno: Lebih efisien secara komputasi, cocok untuk sistem real-time

🛠️ Teknologi yang Digunakan
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (untuk evaluasi)
- Fuzzy Logic (implementasi manual)
