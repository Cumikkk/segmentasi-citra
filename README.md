# Implementasi Metode Segmentasi Citra Digital pada Gambar Tomat

## Deskripsi

Proyek ini merupakan tugas mata kuliah **Visi Komputer** yang mengimplementasikan empat metode segmentasi citra digital menggunakan Python di Google Colab, dengan objek studi berupa citra buah tomat. Segmentasi citra adalah proses memisahkan region-region bermakna dalam sebuah gambar dan dalam konteks ini digunakan untuk membedakan tomat matang, tomat mentah, dan latar belakang, serta menghitung jumlah tomat yang sudah matang secara otomatis.

Keempat metode yang diimplementasikan:

1. **Thresholding (Otsu)** — Memisahkan area tomat dari background berdasarkan nilai intensitas piksel secara otomatis.
2. **Active Contour (Snake)** — Mendeteksi kontur presisi satu tomat menggunakan kurva yang berevolusi mengikuti tepi objek. Ditampilkan dalam tiga tahap: inisial masking, citra biner, dan citra RGB hasil segmentasi.
3. **Segmentasi Warna (HSV)** — Membedakan tomat merah (matang) dari tomat hijau (mentah) dan background menggunakan ruang warna HSV.
4. **Deteksi Tepi Canny** — Menemukan batas kontur seluruh tomat sekaligus menggunakan algoritma Canny edge detection.

Terdapat juga metode kelima berupa **deteksi dan penghitungan otomatis tomat matang** menggunakan kombinasi morphological operations dan watershed algorithm.

## Cara Pakai

**Prasyarat:** Google Colab (direkomendasikan) atau lingkungan Python lokal dengan library berikut terpasang:
```
numpy, matplotlib, scikit-image, opencv-python, scipy, Pillow
```

**Langkah-langkah:**

1. Buka notebook `.ipynb` di Google Colab.
2. Jalankan **Cell 1** — sistem akan meminta upload gambar dari komputer. Pilih foto tomat yang ingin dianalisis.
3. Jalankan **Cell 2 sampai Cell 5** secara berurutan untuk melihat hasil masing-masing metode.
4. Jalankan **Cell 6** untuk melihat perbandingan semua metode dalam satu tampilan.
5. Jalankan **Cell 7** untuk melihat hasil deteksi dan penghitungan tomat matang secara otomatis.

> Catatan: Setiap cell harus dijalankan berurutan karena variabel antar cell saling bergantung. Jika runtime di-reset, mulai ulang dari Cell 1.

## Referensi Jurnal

### 1. Thresholding (Otsu)

- **Segmentasi Obyek pada Citra Digital Menggunakan Metode Otsu Thresholding**
  https://media.neliti.com/media/publications/107084-ID-none.pdf

- **Deteksi Tingkat Kematangan Buah Tomat Menggunakan Pengolahan Citra dengan OpenCV dan Python**
  https://ojs.jurnalmahasiswa.com/index.php/bin/article/view/342/105

### 2. Active Contour (Snake)

- **Segmentasi Citra Luka Luar Berbasis Warna Menggunakan Teknik Active Contour**
  https://mti.uad.ac.id/download/segmentasi-citra-luka-luar-berbasis-warna-menggunakan-teknik-active-contour/

- **Segmentasi Dengan Metode Active Contour Untuk Peningkatan Akurasi Klasifikasi Citra USG Kanker Payudara Menggunakan K-Nearest Neighbor (KNN)**

  https://www.researchgate.net/publication/389897141

### 3. Segmentasi Warna (HSV)

- **Deteksi Kematangan Buah Tomat Berdasarkan Fitur Warna Menggunakan Metode Transformasi Ruang Warna HIS**

  https://ejournal.unkhair.ac.id/index.php/jiko/article/view/1318/1058

- **Klasifikasi Kematangan Buah Tomat dengan Variasi Model Warna Menggunakan Support Vector Machine**
  http://ojs.aknacehbarat.ac.id/index.php/vocatech/article/view/27

### 4. Deteksi Tepi Canny

- **Segmentasi Citra Sapi Berbasis Deteksi Tepi Menggunakan Algoritma Canny Edge Detection**
  https://doi.org/10.24002/jbi.v8i1.1074

- **Analisis Pengaruh Threshold pada Metode Canny dan Sobel dalam Deteksi Tepi Citra Cabai**
  https://publikasi.teknokrat.ac.id/index.php/teknoinfo/article/view/162/63
