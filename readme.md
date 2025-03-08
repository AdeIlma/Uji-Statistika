# Uji Statistika - Analisis Data TikTok Mahasiswa

## Sumber Data
- Data yang digunakan dalam analisis ini adalah data generate (simulasi) yang dibuat menggunakan Python dengan library numpy dan pandas. Data ini dirancang untuk meniru pola dan hubungan yang mungkin terjadi dalam kehidupan nyata, khususnya terkait penggunaan TikTok oleh mahasiswa.
- Dataset terdiri dari 100 entri yang mewakili mahasiswa dengan berbagai karakteristik seperti jurusan, tahun angkatan, dan kebiasaan penggunaan TikTok.
- Meskipun bersifat simulasi, pola hubungan dalam data ini dibuat berdasarkan hipotesis yang masuk akal mengenai bagaimana penggunaan media sosial dapat mempengaruhi aspek kehidupan mahasiswa.
## Deskripsi Proyek

Proyek ini bertujuan untuk melakukan analisis statistik terhadap dataset yang berisi data penggunaan TikTok oleh mahasiswa. Dataset ini mencakup berbagai variabel numerik dan kategorik yang berkaitan dengan waktu penggunaan TikTok, IPK, persentase tugas yang diselesaikan, kesulitan tidur, jenis kelamin, jurusan, tahun angkatan, waktu akses, tipe konten, dan tempat tinggal.

## Struktur File

- **`uji_statistika.ipynb`**: File Jupyter Notebook yang berisi kode Python untuk analisis data.
- **`dataset_tiktok_mahasiswa.csv`**: Dataset yang digunakan dalam analisis.

## Variabel dalam Dataset

1. **Variabel Numerik**:
   - `waktu_tiktok`: Waktu penggunaan TikTok dalam menit per hari (rentang 0-300 menit).
   - `ipk`: Indeks Prestasi Kumulatif (IPK) mahasiswa (rentang 1.0-4.0).
   - `tugas_selesai`: Persentase tugas mahasiswa yang berhasil diselesaikan (rentang 0-100%).

2. **Variabel Kategorik**:
   - `kesulitan_tidur`: Tingkat kesulitan tidur (Tidak, Ringan, Sedang, Parah).
   - `jenis_kelamin`: Jenis kelamin mahasiswa (Laki-laki, Perempuan).
   - `jurusan`: Jurusan mahasiswa (Teknik Informatika, Ekonomi, Psikologi, Kedokteran, Hukum).
   - `tahun_angkatan`: Tahun angkatan mahasiswa (2022, 2023, 2024).
   - `waktu_akses`: Waktu akses TikTok (Pagi, Siang, Malam).
   - `tipe_konten`: Tipe konten yang ditonton (Edukatif, Hiburan, Entertainment).
   - `tempat_tinggal`: Tempat tinggal mahasiswa (Asrama, Kost, Rumah).

## Analisis yang Dilakukan

1. **Statistik Deskriptif**:
   - Menghitung statistik deskriptif untuk variabel numerik seperti mean, median, standar deviasi, minimum, dan maksimum.
   - Menampilkan distribusi variabel kategorik.

2. **Uji Normalitas**:
   - Melakukan uji normalitas pada variabel numerik menggunakan beberapa metode seperti Kolmogorov-Smirnov (KS), Shapiro-Wilk, Pearson, dan Lilliefors.
   - Menentukan apakah data berdistribusi normal atau tidak.

3. **Visualisasi Data**:
   - Membuat histogram untuk variabel numerik untuk melihat distribusi data.
   - Menampilkan visualisasi hubungan antara waktu penggunaan TikTok dan kesulitan tidur.

## Hasil Analisis

- **Statistik Deskriptif**:
  - Rata-rata waktu penggunaan TikTok adalah 115.33 menit per hari.
  - Rata-rata IPK mahasiswa adalah 3.21.
  - Rata-rata persentase tugas yang diselesaikan adalah 77.41%.

- **Uji Normalitas**:
  - Variabel `waktu_tiktok` tidak berdistribusi normal berdasarkan uji Kolmogorov-Smirnov, tetapi berdistribusi normal berdasarkan uji Shapiro-Wilk, Pearson, dan Lilliefors.
  - Variabel `ipk` dan `tugas_selesai` berdistribusi normal berdasarkan semua uji yang dilakukan.

- **Visualisasi Data**:
  - Histogram menunjukkan distribusi data untuk variabel numerik.
  - Visualisasi hubungan antara waktu penggunaan TikTok dan kesulitan tidur menunjukkan adanya korelasi negatif.

## Cara Menjalankan Proyek

1. **Persiapan Lingkungan**:
   - Pastikan Anda telah menginstal Python dan Jupyter Notebook.
   - Instal library yang diperlukan dengan menjalankan perintah berikut:
     ```bash
     pip install numpy pandas matplotlib seaborn scipy
     ```

2. **Menjalankan Notebook**:
   - Buka file `uji_statistika.ipynb` di Jupyter Notebook.
   - Jalankan setiap sel secara berurutan untuk melihat hasil analisis.

3. **Menggunakan Dataset**:
   - Dataset `dataset_tiktok_mahasiswa.csv` akan otomatis dibaca oleh notebook. Pastikan file tersebut berada di direktori yang sama dengan notebook.

## Kontribusi

Jika Anda ingin berkontribusi pada proyek ini, silakan fork repository ini dan buat pull request dengan perubahan yang Anda usulkan.


Dengan mengikuti panduan ini, Anda dapat dengan mudah menjalankan dan memahami analisis data yang dilakukan dalam proyek ini. Selamat mencoba!