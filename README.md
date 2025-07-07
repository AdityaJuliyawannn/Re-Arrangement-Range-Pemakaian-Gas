# 🔄 Re-Arrangement Range Pemakaian Gas Pelanggan Industri PGN

Repositori ini berisi kode dan dokumentasi untuk proyek analisis data pemakaian gas pelanggan industri **PT Perusahaan Gas Negara Tbk (PGN)**. Proyek ini bertujuan untuk menyusun ulang rentang pemakaian gas (range) pada sub-produk **Bronze 1** dan **Bronze 2** secara lebih proporsional, akurat, dan efisien berdasarkan data historis dan metode unsupervised learning.

---

## 🏢 Latar Belakang

PT Perusahaan Gas Negara Tbk (PGN) adalah perusahaan nasional terbesar di bidang transmisi dan distribusi gas bumi di Indonesia. Dalam operasionalnya, PGN mengklasifikasikan pelanggan industri ke dalam produk berdasarkan rata-rata pemakaian gas, salah satunya adalah produk **Bronze**.

Namun, saat ini rentang pemakaian pada sub-produk:
- **Bronze 1**: 1.001 – 10.000 m³/bulan
- **Bronze 2**: 350 – 1.750 MMBtu/bulan  
dinilai **terlalu luas**, sehingga kurang mencerminkan kebutuhan serta karakteristik pelanggan secara proporsional dan efisien. Efisiensi pemakaian berdasarkan data historis hanya tercapai sebesar:
- **31%** (Bronze 1)
- **47%** (Bronze 2)

---

## 🎯 Tujuan Proyek

Menyusun ulang (re-arrange) range pemakaian pada sub-produk Bronze 1 dan 2 dengan metode berbasis data untuk:
- Meningkatkan efisiensi distribusi gas bumi
- Mewakili pola pemakaian pelanggan secara lebih akurat
- Memberikan dasar klasifikasi dan harga yang lebih adil
- Menyediakan acuan pengambilan keputusan strategis di internal PGN

---

## 🧪 Metodologi

Proyek ini menggunakan pendekatan **unsupervised learning** dan **statistik eksploratif** dengan membandingkan 3 algoritma clustering:

| Algoritma                  | Tipe Pendekatan     | Kelebihan                                                                 |
|---------------------------|---------------------|--------------------------------------------------------------------------|
| K-Means                   | Partisi             | Mengelompokkan berdasarkan kemiripan jarak (centroid)                   |
| Gaussian Mixture Model    | Probabilistik       | Cocok untuk data overlap dan distribusi non-linear                      |
| Jenks Natural Breaks (JNB)| Distribusi alami    | Meminimalkan variasi dalam kelompok, cocok untuk data tidak merata      |

---

## 📦 Struktur Proyek
📁 Re-Arrangement-Range-Pemakaian-Gas
│
├── 📁 data/ # Dataset pemakaian gas pelanggan (dihilangkan)
├── 📁 ipnyb/ # Notebook eksplorasi, pemodelan, dan visualisasi
├── 📁 PDF/ 
└── 📄 README.md # Dokumentasi proyek


---

## 📈 Hasil & Analisis

- Ketiga metode memberikan hasil segmentasi yang berbeda, dengan:
  - **K-Means** efektif untuk cluster simetris
  - **GMM** menangkap pola overlap & varian tinggi
  - **JNB** memberikan klasifikasi berbasis distribusi aktual

- **Hasil akhir** menunjukkan bahwa pendekatan **multimetode** menghasilkan range pemakaian yang **lebih adil dan operasional**, serta meningkatkan proporsi pemakaian aktual terhadap batas kontrak pelanggan.



