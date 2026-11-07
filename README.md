# BRImo Digital Banking Customer Reviews & Sentiment Analysis

Dashboard Power BI untuk menganalisis ulasan pengguna aplikasi mobile banking BRImo (Bank BRI) dari Google Play dan App Store.

![Dashboard](BRImo%20Analysis_page-0001.jpg)

## Latar Belakang
Ulasan pengguna adalah sumber umpan balik langsung untuk produk digital. Project ini mengolah ulasan BRImo menjadi insight yang bisa dipakai untuk menemukan masalah utama pengguna dan memprioritaskan perbaikan.

## Dataset
- Google Play: 17.219 review (brimo_googleplaystore_review.csv)
- App Store: 466 review (brimo_appstore_reviews.csv)
- Total: 17.685 review
- Periode: Januari 2023

## Langkah Analisis
1. Data preparation (Power Query): menggabungkan dua file CSV, menyeragamkan kolom (Platform, Rating, ReviewDate, ReviewText), dan mengatur tipe data.
2. Label sentimen (DAX): Rating 4-5 = Positif, 3 = Netral, 1-2 = Negatif.
3. Visualisasi: kartu ringkasan, tren review harian, distribusi rating, donut sentimen dan platform, rata-rata rating per platform, tabel keluhan pengguna, dan slicer platform.
4. Insight dan rekomendasi berdasarkan hasil analisis.

## Key Insight
- 79% review positif (13.968), 18% negatif (3.197), 3% netral (520). Rating rata-rata 4,2.
- Rating Google Play dan App Store hampir sama (sekitar 4,18).
- Keluhan terbanyak pada review negatif: gagal/error/tidak bisa/susah (sekitar 45%), lalu daftar, verifikasi, login, dan OTP (sekitar 32%).
- Semua review negatif sudah dibalas BRI, tetapi secara keseluruhan App Store baru 24% dibalas, Google Play 85%.

## Rekomendasi
1. Sederhanakan alur pendaftaran, verifikasi wajah, dan OTP.
2. Kurangi error saat transaksi dan uji stabilitas sebelum rilis update.
3. Samakan tingkat balasan di App Store dengan Google Play.
4. Pantau sentimen secara rutin setiap rilis.

## Keterbatasan
- Data hanya mencakup Januari 2023, sehingga tidak bisa melihat tren jangka panjang.
- Data App Store hanya 466 review, sehingga perbandingan antar platform perlu dibaca hati-hati.
- Label sentimen berasal dari rating, bukan analisis teks (NLP).
- Persentase jenis keluhan dihitung dari kata kunci pada review negatif, sehingga satu review bisa masuk lebih dari satu kategori.

## Tools
Power BI Desktop, Power Query, DAX

## Isi Repository
- BRImo Analysis.pbix: file dashboard Power BI
- BRImo Analysis.pdf: hasil export dashboard
- brimo_googleplaystore_review.csv dan brimo_appstore_reviews.csv: dataset
- dashboard.png: screenshot dashboard

## Penulis
Medina Fikanti, Teknik Informatika, Universitas Pamulang
