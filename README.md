# Data-Cleansing-Pemegang-Saham
Deskripsi

Project ini merupakan penerapan Data Cleansing menggunakan Python dan Google Colab pada dataset Pemegang Saham di Atas 1% per 31 Juli 2026.

Dataset digunakan untuk mempraktikkan beberapa proses pengolahan data, mulai dari pemeriksaan kondisi awal hingga menghasilkan dataset yang lebih rapi, konsisten, dan siap digunakan untuk analisis selanjutnya.

Sumber Data

Dataset yang digunakan berasal dari Bursa Efek Indonesia (BEI) dengan periode data:

31 Juli 2026

Dataset awal memiliki:

50 baris data
12 kolom
Format Excel (.xlsx)
Proses Data Cleansing

Beberapa proses yang dilakukan dalam project ini meliputi:

1. Pemeriksaan Awal Dataset

Melakukan pemeriksaan terhadap:

Jumlah baris dan kolom
Nama kolom
Tipe data
Missing value
Data duplikat

2. Standarisasi Data

Melakukan penyamaan format pada beberapa kolom, meliputi:

SHARE_CODE
ISSUER_NAME
INVESTOR_NAME
INVESTOR_CLASSIFICATION
DATE
LOCAL_FOREIGN
Data numerik
PERCENTAGE

Contoh standarisasi LOCAL_FOREIGN:
L → LOCAL
F → FOREIGN

3. Penanganan Missing Value

Mengidentifikasi dan menangani nilai kosong pada dataset berdasarkan jenis kolomnya.

4. Deduplikasi Data

Mengidentifikasi dan menghapus data yang duplikat berdasarkan kombinasi:

DATE
SHARE_CODE
INVESTOR_NAME
5. Data Enrichment

Menambahkan informasi INVESTOR_TYPE menggunakan data lookup berdasarkan nilai pada kolom LOCAL_FOREIGN.

6. Pemeriksaan Dataset Setelah Cleansing

Melakukan pemeriksaan kembali terhadap:

Missing value
Data duplikat
Jumlah baris dan kolom
Tipe data
Hasil akhir dataset
Struktur Repository
Data-Cleansing-Pemegang-Saham/
│
├── 2418045dataCleansing.ipynb
├── data_pemegang_saham_1persen_31juli2026.xlsx
├── data_pemegang_saham_1persen_clean.xlsx
└── README.md
Keterangan File
File	Keterangan
2418045dataCleansing.ipynb	Notebook Google Colab yang berisi proses data cleansing menggunakan Python
data_pemegang_saham_1persen_31juli2026.xlsx	Dataset awal sebelum dilakukan cleansing
data_pemegang_saham_1persen_clean.xlsx	Dataset setelah proses cleansing
README.md	Dokumentasi project
Teknologi yang Digunakan
Python
Pandas
NumPy
Google Colab
Microsoft Excel
Link Project
Google Colab

Hasil

Setelah dilakukan proses data cleansing, dataset menjadi lebih:

Konsisten dalam format dan penulisan
Rapi dari sisi struktur data
Bersih dari data duplikat
Lebih lengkap setelah proses data enrichment
Siap digunakan untuk proses analisis selanjutnya
Identitas
