# Clustering

## Problem Background
Pelanggan kredit merupakan aset penting bagi bank karena berkontribusi langsung terhadap pendapatan dan stabilitas keuangan melalui bunga dan penggunaan produk kredit. Namun, setiap pelanggan memiliki karakteristik dan tingkat risiko yang berbeda, sehingga pengelolaan kredit tanpa pemahaman yang baik dapat meningkatkan risiko gagal bayar dan strategi bisnis yang tidak optimal. Oleh karena itu, clustering data pelanggan kredit diperlukan untuk mengelompokkan nasabah berdasarkan perilaku dan profil kreditnya, sehingga bank dapat menyusun strategi manajemen risiko, penentuan limit, serta pemasaran yang lebih tepat dan berbasis data.
## Problem
Untuk mengelompokkan pelanggan kredit berdasarkan kemiripan perilaku dan risiko, sehingga bank dapat mengambil keputusan kredit, manajemen risiko, dan strategi layanan secara lebih tepat dan efisien.
## Project Output

| **Kluster** | **Karakteristik Utama**                           | **Profil Pelanggan**                                                                                      | **Rekomendasi Bisnis**                                                                              |
| ----------- | ------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **0**       | Balance tinggi, limit tinggi, purchases rendah    | **Pengguna Saldo Besar** — saldo dan limit tinggi, jarang bertransaksi, tetapi rutin melakukan pembayaran | Sediakan program pengurangan saldo dan insentif agar lebih sering bertransaksi (reward/poin ekstra) |
| **1**       | Balance rendah, limit rendah, purchases sedang    | **Pembeli Moderat** — menggunakan kartu secara hati-hati dengan pembelian stabil                          | Tawarkan peningkatan limit bertahap untuk mendorong transaksi lebih besar                           |
| **2**       | Purchases, limit, dan payments sangat tinggi      | **Pengguna Aktif Premium** — pelanggan paling aktif dan paling menguntungkan                              | Prioritaskan loyalitas dengan penawaran premium dan program reward eksklusif                        |
| **3**       | Balance, limit, payments, purchases sangat rendah | **Pengguna Minimalis** — menggunakan kartu sangat sedikit                                                 | Berikan insentif awal (diskon/bonus) untuk meningkatkan aktivitas penggunaan kartu                  |


## Data

Dataset: `P1G6_haafizhhamda.csv`

**Dataset Information**:


- **CUST_ID**: ID unik yang digunakan untuk mengidentifikasi setiap pelanggan.
- **BALANCE**: Saldo rata-rata yang dimiliki pelanggan pada kartu kredit.
- **BALANCE_FREQUENCY**: Frekuensi pembaruan saldo kartu kredit (nilai mendekati 1 menunjukkan saldo sering diperbarui).
- **PURCHASES**: Total nilai pembelian yang dilakukan pelanggan.
- **ONEOFF_PURCHASES**: Total nilai pembelian satu kali (non-cicilan).
- **INSTALLMENTS_PURCHASES**: Total nilai pembelian yang dilakukan dengan sistem cicilan.
- **CASH_ADVANCE**: Total dana tunai yang ditarik pelanggan dari kartu kredit.
- **PURCHASES_FREQUENCY**: Frekuensi pelanggan melakukan transaksi pembelian.
- **ONEOFF_PURCHASES_FREQUENCY**: Frekuensi pembelian satu kali.
- **PURCHASES_INSTALLMENTS_FREQUENCY**:  Frekuensi pembelian dengan sistem cicilan.
- **CASH_ADVANCE_FREQUENCY**:  Frekuensi pelanggan melakukan penarikan dana tunai.
- **CASH_ADVANCE_TRX**:  Jumlah transaksi penarikan dana tunai.
- **PURCHASES_TRX**:  Jumlah transaksi pembelian.
- **CREDIT_LIMIT**:  Batas maksimum kredit yang dimiliki pelanggan.
-  **PAYMENTS**:  Total pembayaran yang dilakukan pelanggan.
- **MINIMUM_PAYMENTS**:  Total pembayaran minimum yang harus dibayarkan pelanggan.
- **PRC_FULL_PAYMENT**:  Persentase pembayaran penuh (full payment) yang dilakukan pelanggan.
- **TENURE**:  Lama waktu pelanggan menggunakan kartu kredit (dalam bulan).



## Method

## Alur Pengerjaan Project

- **Data Loading**
- **Exploratory Data Analysis (EDA)**

- **Feature Engineering**
   - Define Numeric
   - Check Cardinality
   - Handling Outlier
   - Missing Value
   - Scaling

- **Dimensionality Reduction**
- **Find the Optimal Number of Clusters**
- **Train with the Optimal Number of Clusters**

- **EDA After Clustering**

- **Saving**

- **Kesimpulan**


## Stacks

- Python:

  - **Data Processing**: pandas, numpy
  - **Visualization**: matplotlib, seaborn
  - **Preprocessing & Feature Engineering**:
    - Scaling: StandardScaler
    - Outlier Handling: Winsorizer
  - **Dimensionality Reduction**: PCA
  - **Clustering Model**: KMeans
  - **Evaluation**:
    - Silhouette Score: silhouette_score, silhouette_samples
    - Visualization: SilhouetteVisualizer
  - **Utilities & Saving**: pickle, json

- GitHub

## Reference

- Laporan analisis model data berupa notebook `P1G6_haafizhhamda` dan visualisasi
- `model_kmean.pkl` berupa hasil model
- `P1G6_haafizhhamda.csv` berupa dataset

---