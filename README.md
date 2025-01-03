# Optimasi-SVM-untuk-Klasifikasi-Kanker-Payudara-dengan-Particle-Swarm-Optimization
Penelitian ini bertujuan meningkatkan klasifikasi kanker payudara dengan mengoptimalkan parameter Support Vector Machine (SVM) menggunakan Particle Swarm Optimization (PSO). Data Breast Cancer Wisconsin (Prognostic) dengan 198 observasi dan 35 atribut digunakan untuk menguji metode ini. Hasil menunjukkan PSO berhasil meningkatkan kinerja SVM dengan akurasi **85%**, presisi **83,8%**, dan recall **100%**, menunjukkan kemampuan deteksi kasus positif yang optimal. PSO memungkinkan eksplorasi parameter secara efisien, mengurangi risiko overfitting dan underfitting. Metode ini berpotensi mendukung deteksi dini kanker payudara, membantu profesional medis dalam pengambilan keputusan klinis, serta berkontribusi pada pengembangan teknologi prediksi medis yang lebih andal.

## Pendahuluan
Proyek ini bertujuan untuk mengoptimalkan klasifikasi kanker payudara menggunakan Support Vector Machine (SVM) dengan algoritma Particle Swarm Optimization (PSO) untuk memilih parameter terbaik (C dan gamma). Dataset yang digunakan adalah Breast Cancer Wisconsin (Prognostic) dari UCI Machine Learning Repository.

## Instalasi
Pastikan Anda sudah menginstal Python dan pip. Instal library yang diperlukan dengan perintah berikut:

```bash
pip install pyswarms ucimlrepo numpy pandas scikit-learn matplotlib seaborn
```

## Langkah-Langkah

### 1. Import Dataset
Dataset diambil langsung dari UCI Machine Learning Repository menggunakan library `ucimlrepo`.
link : https://archive.ics.uci.edu/dataset/16/breast+cancer+wisconsin+prognostic
### 2. Data Cleaning
- Mengisi nilai yang hilang dengan rata-rata.
- Melakukan label encoding untuk kolom kategori.

### 3. Data Analysis / Preprocessing
- Menampilkan statistik deskriptif.
- Membuat heatmap korelasi.
- Membagi data menjadi set pelatihan dan pengujian.

### 4. Optimasi Parameter dengan PSO
Algoritma PSO digunakan untuk mencari parameter optimal (C dan gamma) dengan fungsi fitness berbasis akurasi klasifikasi.

### 5. Pelatihan Model
Model SVM dilatih menggunakan parameter terbaik yang diperoleh dari PSO.

### 6. Evaluasi Model
- Akurasi
- Classification Report
- Confusion Matrix
- Precision-Recall Curve
- ROC Curve

### 7. Visualisasi Prediksi
Membuat plot untuk batas keputusan pada set pelatihan dan pengujian.

### 8. Contoh Prediksi
Melakukan prediksi kelas untuk data baru.

## Struktur Program
1. **Import Library**: Semua library penting diimpor di awal.
2. **Preprocessing**: Menangani nilai hilang, encoding, dan standarisasi.
3. **PSO Optimization**: Algoritma PSO untuk mencari parameter optimal.
4. **Model Training**: SVM dilatih dengan parameter optimal.
5. **Evaluation**: Evaluasi model menggunakan berbagai metrik.
6. **Visualization**: Menampilkan hasil prediksi secara grafis.

## Cara Penggunaan
1. Jalankan script di lingkungan Python seperti Jupyter Notebook atau IDE.
2. Pastikan semua dependensi sudah terinstal.
3. Ikuti langkah-langkah sesuai urutan untuk mengoptimalkan parameter dan mengevaluasi model.

## Hasil
Setelah melakukan optimasi, parameter terbaik (C dan gamma) diperoleh menggunakan PSO. Model SVM memberikan hasil akurasi tinggi pada dataset pengujian. Visualisasi seperti Precision-Recall Curve dan ROC Curve disediakan untuk analisis lebih lanjut.

## Catatan Tambahan
- Dataset harus diperiksa secara manual untuk menangani outlier atau anomali.
- Algoritma PSO memerlukan waktu yang bervariasi tergantung pada ukuran dataset dan jumlah iterasi.
---
