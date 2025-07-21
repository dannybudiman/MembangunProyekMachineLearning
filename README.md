# Proyek Akhir Belajar Machine Learning untuk Pemula - Dicoding

## Deskripsi Proyek

Proyek ini merupakan bagian dari tugas akhir kelas Machine Learning Pemula di Dicoding. Proyek ini bertujuan untuk melakukan analisis dan pemodelan machine learning menggunakan dataset Bank Transaction dari Dicoding.
Proyek ini terdiri dari dua bagian utama: clustering dan klasifikasi.


## Struktur Proyek

1. **Clustering**
    - Notebook: `[Clustering]_Submission_Akhir_BMLP.ipynb`
    - Deskripsi: Pada bagian ini, dilakukan analisis eksplorasi data (EDA) dan clustering menggunakan algoritma K-Means dan DBSCAN untuk mengelompokkan data pesawat berdasarkan harga dan kategori.
    - Hasil Silhouette Score: X.XX (K-Means) dan X.XX (DBSCAN)

2. **Klasifikasi**
    - Notebook: `[Klasifikasi]_Submission_Akhir_BMLP.ipynb`
    - Deskripsi: Pada bagian ini, dilakukan pemodelan klasifikasi menggunakan algoritma Random Forest untuk memprediksi cluster dari dataset yang telah dikelompokkan pada tahap clustering.
    - Hasil Accuracy: XX.X%


## Persyaratan

- Python 3.12 atau lebih tinggi
- Jupyter Notebook
- Menginstall seluruh dependency dari `requirements.txt`
> `pip install -r requirements.txt`


## Cara Menjalankan

1. Pastikan Anda memiliki Python 3.12 atau lebih tinggi dan Jupyter Notebook terinstal di sistem Anda.
2. Buka Jupyter Notebook.
3. Jalankan notebook `[Clustering]_Submission_Akhir_BMLP.ipynb` untuk melakukan clustering.
4. Jalankan notebook `[Klasifikasi]_Submission_Akhir_BMLP.ipynb` untuk melakukan klasifikasi.


## Dataset
Dataset yang digunakan dalam project ini sudah disediakan oleh Dicoding:
https://drive.google.com/drive/folders/1Zs7VmPZ-jNwsRlMKH65Ea-LApSwx6lKx?hl=ID


## Kriteria Penilaian

Kriteria 1: Memuat Dataset dan Melakukan Exploratory Data Analysis (EDA)
- Menampilkan dataset menggunakan function head().
- Menampilkan informasi dataset dengan info().
- Menampilkan statistik deskriptif dataset dengan menjalankan describe() untuk mendapatkan ringkasan data.

Kriteria 2: Pembersihan dan Pra Pemrosesan Data
- Mengecek dataset menggunakan isnull().sum() dan duplicated().sum().
- Melakukan feature scaling menggunakan MinMaxScaler() atau StandardScalar() untuk fitur numerik.
- Melakukan feature encoding menggunakan LabelEncoder() untuk fitur kategorikal.
- Melakukan drop pada kolom yang memiliki keterangan ID seperti TransactionID, AccountID, DeviceID,  IPAddress, MerchantID 

Kriteria 3: Membangun Model Clustering
- Menggunakan dataset yang sudah dilakukan preprocessing.
- Melakukan visualisasi Elbow Method untuk menentukan jumlah cluster terbaik menggunakan KElbowVisualizer().
- Menggunakan algoritma K-Means Clustering dengan sklearn.cluster.KMeans().
- Menjalankan cell code joblib.dump() dengan nama model_clustering agar reviewer dapat secara otomatis menilai evaluasi model anda.

Kriteria 4: Interpretasi Hasil Clustering
- Menampilkan hasil clustering dalam bentuk visualisasi.
- Menjelaskan karakteristik tiap cluster berdasarkan rentangnya.
- Mengekspor data training dari proses preprocessing beserta data hasil clustering dan berikan nama untuk kolom tersebut yaitu Target.

Kriteria 5: Membangun Model Klasifikasi
- Menggunakan train_test_split() untuk melakukan pembagian dataset.
- Membangun model dengan algoritma Decision Tree.
- Menjalankan cell code joblib.dump() dengan nama decision_tree_model.h5 agar reviewer dapat secara otomatis menilai evaluasi model anda.

