# 📦 Exploring Olist E-Commerce Data: Uncovering Significant Trends and Patterns

Capstone project for the Data Analyst program — an end-to-end Exploratory Data Analysis (EDA) on Olist Store's e-commerce transaction data to uncover business insights and provide actionable recommendations.

**Author:** Fariz Agyan

---

## 📖 Project Background

Olist Store is an e-commerce marketplace based in São Paulo, Brazil. This project analyzes a public dataset shared by Olist containing information on roughly 100,000 transactions between 2016 and 2018, covering order status, pricing, customer location, payment methods, product categories, and customer reviews.

## ❓ Problem Statement

1. Bagaimana pola transaksi, metode pembayaran, dan produk yang dijual di platform Olist?
2. Apakah terdapat pertumbuhan *new customer* pada rentang waktu tersebut?
3. Bagaimana tingkat kepuasan pelanggan terhadap produk dan layanan yang diberikan oleh penjual?
4. Bagaimana tingkat pembelian dari masing-masing pelanggan — apakah mereka pelanggan aktif, jarang membeli, atau hanya membeli sekali?

## 🗂️ Dataset

Dataset asli terdiri dari beberapa tabel (orders, products, customers, sellers, reviews, geolocation, dll). Analisis ini berfokus pada 5 tabel utama:

| Tabel | Deskripsi |
|---|---|
| **Orders** | Data pesanan: id pesanan, id pelanggan, tanggal, total harga, status |
| **Products** | Data produk: id, nama, deskripsi, harga, kategori |
| **Customers** | Data pelanggan: id, zip code, kota |
| **Sellers** | Data penjual: id, domisili |
| **Geolocation** | Data lokasi: kode pos, latitude, longitude |

Source: [Kaggle — Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/olistbr/brazilian-ecommerce)

## 🛠️ Method & Workflow

- **Framework:** CRISP-DM
- **Workflow:**
  1. Define stakeholder & analytics objectives
  2. Define problem statement
  3. Exploratory Data Analysis (EDA)
  4. Problem discovery
  5. Insight & recommendation

## 🔍 Key Findings

- Nilai transaksi (revenue) cenderung naik tiap bulan, namun **jumlah transaksi menurun drastis di akhir tahun**.
- **São Paulo (SP), Minas Gerais (MG), dan Rio de Janeiro (RJ)** adalah top 3 negara bagian dengan total transaksi dan nilai tertinggi.
- **Credit card** adalah metode pembayaran paling dominan, diikuti **Boleto** (metode pembayaran khas Brazil) — keduanya mencakup 90–95% dari seluruh transaksi.
- Jam sibuk transaksi berada di sekitar **pukul 11.00 dan 15.00–16.00**.
- Kategori produk dengan penjualan tertinggi: **bed_bath_table, computers_accessories, furniture_decor**.
- Terjadi penurunan tajam pada jumlah *new customer* di periode **November–Desember 2017**.
- **76% review positif** vs **~15% review negatif** dari seluruh transaksi.
- Pelanggan dikelompokkan berdasarkan **Recency & Monetary Value** untuk memahami segmentasi pelanggan aktif, jarang membeli, dan sekali beli (pendekatan mirip RFM).

## 💡 Recommendations

- Tingkatkan promosi dan kapasitas ekspedisi menjelang akhir tahun untuk mencegah penurunan transaksi saat *high-season*.
- Perluas promosi ke kota-kota dengan nilai transaksi rendah untuk meratakan persebaran penjualan.
- Optimalkan waktu tayang promosi di aplikasi pada jam-jam puncak transaksi harian.
- Tingkatkan kualitas kategori produk unggulan (bed & bath, computer accessories, furniture) agar semakin menjadi pilihan utama pelanggan.
- Analisis lebih lanjut penyebab penurunan *new customer* di akhir 2017 dan siapkan promosi khusus pelanggan baru pada periode rawan tersebut.
- Analisis review negatif secara mendalam untuk menurunkan tingkat ketidakpuasan pelanggan.
- Bangun program loyalitas (poin/reward) untuk mendorong repeat purchase dari pelanggan yang baru bertransaksi sekali.
- Sasar promosi berdasarkan segmentasi cluster pelanggan agar biaya marketing lebih efisien dan tepat sasaran.

## 🧰 Tools

`Python` (Pandas, EDA) · `Jupyter Notebook` · `Tableau` (dashboard & visualisasi)

## 📁 Repository Contents

- `Capstone_FARIZ_AGYAN_V1.ipynb` — Notebook analisis data (data cleaning & EDA)
- `Capstone_FARIZ_AGYAN_V1.twb` — File dashboard Tableau
- `Capstone_FARIZ_AGYAN_V1.pptx` — Slide presentasi hasil analisis
- `Olist_Data_Final_V1.csv` — Dataset yang digunakan

---

*Project ini merupakan bagian dari program Data Analyst #CDANarasioData.*
