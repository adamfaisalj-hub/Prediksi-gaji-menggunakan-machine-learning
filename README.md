# Prediksi-gaji-menggunakan-machine-learning
 # Deskripsi Proyek
Proyek ini merupakan analisis data lowongan pekerjaan Data Engineer menggunakan Python dan Jupyter Notebook. Proyek bertujuan untuk memahami karakteristik lowongan kerja Data Engineer melalui proses eksplorasi data, pembersihan data, penanganan missing values, deteksi outlier, transformasi data, serta analisis korelasi antarvariabel. 
Dataset yang digunakan berisi informasi mengenai lowongan pekerjaan Data Engineer, seperti jabatan, estimasi gaji, deskripsi pekerjaan, rating perusahaan, lokasi, industri, dan informasi perusahaan lainnya.
# Tujuan Proyek

Memahami struktur dan karakteristik dataset lowongan kerja Data Engineer.

Melakukan data cleaning untuk mempersiapkan data sebelum analisis.

Menangani missing values pada data numerik dan kategorikal.

Melakukan eksplorasi data menggunakan visualisasi.

Melakukan transformasi dan standarisasi data.

Menganalisis distribusi data dan korelasi antarvariabel, khususnya terhadap rating.

# Dataset

Dataset yang digunakan adalah DataEngineer.csv.

Dataset terdiri dari 2.528 baris dan 15 kolom, dengan beberapa atribut berikut:

Kolom

Deskripsi

Job Title

Jabatan pekerjaan

Salary Estimate

Estimasi gaji

Job Description

Deskripsi dan persyaratan pekerjaan

Rating

Rating perusahaan

Company Name

Nama perusahaan

Location

Lokasi pekerjaan

Headquarters

Lokasi kantor pusat perusahaan

Size

Ukuran perusahaan

Founded

Tahun perusahaan didirikan

Type of ownership

Jenis kepemilikan perusahaan

Industry

Industri perusahaan

Sector

Sektor bisnis perusahaan

Revenue

Pendapatan perusahaan

Competitors

Informasi perusahaan pesaing

Easy Apply

Informasi kemudahan melamar pekerjaan

# Tools dan Library

Proyek ini menggunakan beberapa library Python:

Pandas — untuk membaca, mengolah, dan membersihkan data.

Seaborn — untuk visualisasi dan eksplorasi data.

Matplotlib — untuk membuat grafik dan visualisasi.

Scikit-learn — untuk standarisasi data menggunakan StandardScaler serta encoding menggunakan LabelEncoder.

# Tahapan Analisis Data

1. Data Loading

Membaca dataset CSV menggunakan Pandas dan menampilkan beberapa baris pertama untuk memahami isi data.

2. Data Understanding

Memeriksa struktur dataset, tipe data, informasi kolom, dan statistik deskriptif menggunakan info() dan describe().

3. Missing Values Handling

Mengidentifikasi nilai yang hilang pada setiap kolom. Program menerapkan beberapa metode penanganan:

Kolom numerik diisi menggunakan nilai median.

Kolom kategorikal diisi menggunakan nilai modus.

Kolom dengan jumlah missing values mencapai 1.000 atau lebih dihapus dari dataset.

4. Outlier Analysis

Menggunakan box plot untuk mengamati distribusi data numerik dan metode Interquartile Range (IQR) untuk mengidentifikasi data yang berpotensi menjadi outlier.

5. Data Standardization

Menggunakan StandardScaler untuk melakukan standarisasi pada fitur numerik sehingga skala data dapat dibandingkan dengan lebih mudah.

6. Duplicate Data Handling

Memeriksa baris duplikat menggunakan duplicated() dan menghapus duplikasi menggunakan drop_duplicates().

7. Categorical Data Encoding

Mengubah data kategorikal menjadi format numerik menggunakan dua pendekatan:

One-Hot Encoding dengan pd.get_dummies().

Label Encoding dengan LabelEncoder.

8. Exploratory Data Analysis (EDA)

Melakukan eksplorasi data melalui beberapa visualisasi, antara lain:

Histogram untuk melihat distribusi variabel.

Box plot untuk memeriksa sebaran dan potensi outlier.

Heatmap untuk melihat korelasi antarvariabel.

Grafik korelasi untuk mengetahui hubungan variabel dengan rating perusahaan.

9. Correlation Analysis

Menghitung korelasi antarvariabel numerik dan mengurutkan nilai korelasi absolut terhadap kolom Rating untuk membantu mengidentifikasi variabel yang memiliki hubungan linear relatif kuat dengan rating perusahaan.

# Hasil yang Diharapkan

Melalui tahapan analisis tersebut, proyek ini diharapkan dapat menghasilkan pemahaman yang lebih baik mengenai:

Karakteristik dan distribusi data lowongan pekerjaan Data Engineer.

Kondisi kualitas data sebelum dan sesudah preprocessing.

Distribusi berbagai atribut pekerjaan dan perusahaan.

Hubungan linear antara atribut numerik dan rating perusahaan.

Data yang lebih terstruktur untuk digunakan pada analisis atau pengembangan model machine learning berikutnya.

# Cara Menjalankan Proyek

Clone repository GitHub:

git clone https://github.com/USERNAME/REPOSITORY.git

Masuk ke folder proyek:

cd REPOSITORY

Instal library yang dibutuhkan:

pip install pandas matplotlib seaborn scikit-learn jupyter

Pastikan file DataEngineer.csv berada di direktori yang sama dengan Laporan.ipynb.

Jalankan Jupyter Notebook:

jupyter notebook

Buka Laporan.ipynb dan jalankan setiap cell secara berurutan.

# Struktur Repository

DataEngineer-Analysis/
├── DataEngineer.csv
├── Laporan.ipynb
└── README.md

# Kesimpulan

Proyek ini menerapkan proses pengolahan dan eksplorasi data lowongan pekerjaan Data Engineer menggunakan Python. Proses meliputi pemeriksaan data, penanganan missing values, analisis outlier, standarisasi, encoding data kategorikal, visualisasi, serta analisis korelasi.

Hasil eksplorasi ini dapat menjadi dasar untuk pengembangan proyek machine learning selanjutnya, misalnya untuk memprediksi rating perusahaan atau melakukan analisis estimasi gaji, setelah menentukan target, fitur, dan metode evaluasi yang sesuai.

Author: [Adam Faisal Jabbar]

Project Type: Data Analysis / Data Preprocessing / Exploratory Data Analysis (EDA)

Language: Python
