# KELOMPOK 5_KLASIFIKASI
## Latar Belakang
Depresi di kalangan siswa telah menjadi isu kesehatan mental yang mendesak dan kompleks, terutama pada kelompok usia 15–24 tahun. Menurut WHO, depresi adalah penyebab utama disabilitas global untuk kelompok usia ini. Berbagai faktor seperti tekanan akademik, penggunaan media sosial yang berlebihan, kurangnya dukungan emosional, hingga kondisi ekonomi keluarga turut berperan dalam meningkatnya prevalensi depresi.

**Dataset** yang digunakan dalam proyek ini terdiri dari 27.901 baris data siswa dengan 18 fitur. Variabel target **Depression_Status** bersifat biner (0 atau 1), menunjukkan apakah seorang siswa mengalami depresi atau tidak.

## Struktur Dataset
Beberapa variabel dalam dataset ini meliputi:
- ID
- Demografi: Usia, jenis kelamin, kota tinggal
- Akademik: CGPA, tekanan akademik, kepuasan studi
- Gaya Hidup & Kesejahteraan: durasi tidur, pola makan,tekanan kerja, kepuasan Kerja, jam belajar/kerja
- Faktor Lainnya: profesi, jenjang pendidikan, stres keuangan, riwayat keluarga, pikiran bunuh diri
- Variabel Target: Depression_Status

## Tahapan Preprocessing
1. Cek Missing Values
- Dataset sudah bersih dari missing values.
2. Pembersihan Data
- Menghapus kolom id
- Menghapus spasi berlebih pada data kategorikal
- Menghapus data duplikat
3. Encoding
- Durasi tidur dikonversi ke nilai numerik (contoh: “5-6 hours” → 5.5)
- Label Encoding untuk seluruh kolom kategorikal
4. Split Dataset
- Dataset dibagi 80% training dan 20% testing
- X: 16 fitur utama, y: variabel target Depression_Status
5. Normalisasi
- Menggunakan StandardScaler dari sklearn agar semua fitur memiliki skala yang seragam

## Model dan Evaluasi
Dua model digunakan untuk klasifikasi:
- Random Forest Classifier
- Support Vector Machine (SVM)

Model Random Forest memiliki akurasi sebesar 0,83, dengan precision, recall, dan f1-score tertinggi pada kelas 1, menunjukkan kemampuan yang lebih baik dalam mengenali korban. Sementara itu, model Support Vector Machine (SVM) sedikit lebih unggul dengan akurasi 0,84, serta performa keseluruhan yang lebih seimbang dan konsisten dalam mengklasifikasikan kedua kelas.

## Kesimpulan
Proyek ini menunjukkan potensi pemanfaatan machine learning untuk membantu memahami dan mengidentifikasi siswa yang berisiko mengalami depresi. Dengan pendekatan klasifikasi dan preprocessing yang tepat, kita dapat memperoleh wawasan penting dari data untuk mendukung intervensi yang lebih efektif di masa depan.

## Kontributor
- Kinanti Anggraeni (4112322010)
- Sekar Ayun Cahyani (4112322003)
- Mega Deazzahra (4112322016)
- Puput Nur Ramadhany (4112322017)
- Bintang Pamungkas (4112322024)
