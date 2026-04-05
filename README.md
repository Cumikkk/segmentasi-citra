# Implementasi Metode Segmentasi Citra Digital pada Gambar Tomat

> Mata Kuliah: Visi Komputer

## Deskripsi

Proyek ini mengimplementasikan empat metode segmentasi citra digital menggunakan Python di Google Colab, dengan objek studi berupa citra buah tomat. Segmentasi citra adalah proses memisahkan region-region bermakna dalam sebuah gambar — dalam konteks ini digunakan untuk membedakan tomat matang, tomat mentah, dan latar belakang, serta menghitung jumlah tomat yang sudah matang secara otomatis.

Keempat metode yang diimplementasikan:

1. **Thresholding (Otsu)** — Memisahkan area tomat dari background berdasarkan nilai intensitas piksel secara otomatis.
2. **Active Contour (Snake)** — Mendeteksi kontur presisi satu tomat menggunakan kurva yang berevolusi mengikuti tepi objek. Ditampilkan dalam tiga tahap: inisial masking, citra biner, dan citra RGB hasil segmentasi.
3. **Segmentasi Warna (HSV)** — Membedakan tomat merah (matang) dari tomat hijau (mentah) dan background menggunakan ruang warna HSV.
4. **Deteksi Tepi Canny** — Menemukan batas kontur seluruh tomat sekaligus menggunakan algoritma Canny edge detection.

Sebagai bonus, terdapat metode kelima berupa **deteksi dan penghitungan otomatis tomat matang** menggunakan kombinasi morphological operations dan watershed algorithm.

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

- Syafi'i, S. I., Wahyuningrum, R. T., & Muntasa, A. (2016). **Segmentasi Obyek pada Citra Digital Menggunakan Metode Otsu Thresholding**. *Jurnal Informatika*, 13(1), 1–8. https://doi.org/10.9744/informatika.13.1.1-8

- Firdaus, H., Farizi, F., Syakur, R. A., Ramadhan, A. T., & Rosyani, P. (2024). **Deteksi Tingkat Kematangan Buah Tomat Menggunakan Pengolahan Citra dengan OpenCV dan Python**. *BIN: Bulletin of Informatics*, 2(1), 130–136. https://ojs.jurnalmahasiswa.com/index.php/bin/article/view/342

### 2. Active Contour (Snake)

- Fadillah, N., & Gunawan, C. R. (2019). **Segmentasi Citra CT Scan Paru-Paru dengan Menggunakan Metode Active Contour**. *JURIKOM (Jurnal Riset Komputer)*, 6(2), 126–132. https://doi.org/10.30865/jurikom.v6i2.1166

- Mawarni, S. S., Murinto, M., & Sunardi, S. (2023). **Segmentasi Citra Luka Luar Berbasis Warna Menggunakan Teknik Active Contour**. *Kesatria: Jurnal Penerapan Sistem Informasi (Komputer dan Manajemen)*, 4(2). https://doi.org/10.30645/kesatria.v4i2.175

### 3. Segmentasi Warna (HSV)

- Pratama, R., Assagaf, A. F., & Tempola, F. (2019). **Deteksi Kematangan Buah Tomat Berdasarkan Fitur Warna Menggunakan Metode Transformasi Ruang Warna HIS**. *JIKO (Jurnal Informatika dan Komputer)*, 2(2). https://doi.org/10.33387/jiko.v2i2.1318

- Firdaus, H., Farizi, F., Syakur, R. A., Ramadhan, A. T., & Rosyani, P. (2024). **Deteksi Tingkat Kematangan Buah Tomat Menggunakan Pengolahan Citra dengan OpenCV dan Python**. *BIN: Bulletin of Informatics*, 2(1), 130–136. https://ojs.jurnalmahasiswa.com/ojs/index.php/bin/article/view/342

### 4. Deteksi Tepi Canny

- Mustafid, A., & 'Uyun, S. (2017). **Segmentasi Citra Sapi Berbasis Deteksi Tepi Menggunakan Algoritma Canny Edge Detection**. *Jurnal Buana Informatika*, 8(1), 27–36. https://doi.org/10.24002/jbi.v8i1.1074

- Rahayu, S., Ridwansyah, & Purnama, J. J. (2025). **Analisis Pengaruh Threshold pada Metode Canny dan Sobel dalam Deteksi Tepi Citra Cabai**. *Jurnal Teknoinfo*, 19(2), 118–127. https://doi.org/10.33365/teknoinfo.v19i2.162
