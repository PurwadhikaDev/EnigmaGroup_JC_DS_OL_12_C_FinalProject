# Olist Brazilian E-Commerce Analysis by Enigma 📊🛍

## Enigma - JCDSOL – 012 (C) 👩‍💻🧑‍💻
- Teguh Saputra
- Benazheer Salsabila
- Masta Siahaan
- Abyatar Fanuel Lantera


## Latar Belakang 🛒
Olist, sebuah platform e-commerce terkemuka di Brasil, telah menjadi wahana bagi ribuan merchant untuk menjual produk mereka secara online. Namun, untuk tetap bersaing di pasar yang semakin kompetitif, para merchant membutuhkan wawasan yang mendalam tentang perilaku konsumen, tren penjualan, dan faktor-faktor lain yang mempengaruhi pendapatan mereka. Inilah mengapa tim Data Analyst/Scientist Olist hadir: untuk menggali potensi data dan menerjemahkannya menjadi strategi bisnis yang cerdas dan efektif.

## Konteks 💰
Dalam konteks bisnis e-commerce yang dinamis, peningkatan revenue bukan hanya tentang menghasilkan keuntungan bagi para merchant, tetapi juga tentang meningkatkan reputasi dan daya saing platform secara keseluruhan. Dengan pemahaman yang lebih baik tentang perilaku konsumen dan preferensi mereka, Merchant Olist dapat menyediakan pengalaman berbelanja yang lebih personal dan memuaskan, yang pada gilirannya akan meningkatkan loyalitas pelanggan dan menggerakkan pertumbuhan bisnis.

## Problem 📉❗️
![image](https://github.com/PurwadhikaDev/EnigmaGroup_JC_DS_OL_12_C_FinalProject/assets/109770559/a953e807-5acf-4ca2-aefe-08abc6527205)
Jumlah order dan pendapatan mengalami peningkatan dari tahun 2017 ke 2018, namun terjadi stagnasi bahkan penurunan pada tahun 2018, khususnya sejak November. Faktor utama yang mempengaruhi revenue penjualan adalah perilaku konsumen, harga jual, dan kuantitas penjualan. Penetapan harga yang tepat penting untuk menghindari kehilangan minat pelanggan atau kerugian bagi penjual. Demikian pula, manajemen persediaan yang baik diperlukan agar tidak terjadi kelebihan atau kekurangan stok. Oleh karena itu, memahami perilaku konsumen dan menerapkan strategi kampanye yang efektif, serta menetapkan harga dan kuantitas penjualan secara optimal, merupakan langkah kunci dalam meningkatkan kembali pendapatan penjualan.

## Tujuan Utama 📈
![image](https://github.com/PurwadhikaDev/EnigmaGroup_JC_DS_OL_12_C_FinalProject/assets/109770559/73d5bfce-6c29-4f2d-8793-abc28f8fb3e4)
1. **Meneliti Perilaku Konsumen**: Memahami bagaimana konsumen berinteraksi dengan platform, produk, dan layanan Olist.
2. **Penerapan Machine Learning (ML)**: Pembangunan model ML untuk memprediksi pendapatan merchant berdasarkan data historis dan variabel-variabel lainnya.
3. **Peningkatan Revenue Merchant**: Rekomendasi yang actionable berdasarkan hasil analisis data untuk meningkatkan kinerja dan pendapatan mereka.
4. **Menaikkan Traffic Olist**: Mengembangkan strategi untuk meningkatkan jumlah pengunjung dan aktivitas pengguna di platform Olist.

## Business Questions 💬❓
- Bagaimana perilaku pembelian dari customer (Preferensi Produk, Waktu Pembelian, Jumlah Transaksi, Rata - Rata Pengeluaran, dll)?
- Bagaimana Karakteristik dari setiap prtoduk yang terjual?
- Bagaimana keragaman produk yang terjual di setiap lokasi yang berbeda?
- Faktor - Faktor apa saja yang berpengaruh terhadap revenue penjualan?

## Gambaran Data 📑
Data yang dianalisis mencakup berbagai aspek, mulai dari jumlah order, revenue, hingga detail produk dan pelanggan. Faktor-faktor seperti harga produk, biaya pengiriman, lokasi geografis, rating produk, dan lainnya diperhatikan. Data historis dari tahun 2016-2018 menjadi dasar untuk mengidentifikasi pola-pola yang berguna dan menerapkan strategi yang relevan. Data yang digunakan untuk membangun model Machine Learning:

| Attribute | Data Type | Description |
| --- | --- | --- |
| customer_city | object | customer city name |
| customer_state | object | customer state |
| product_category_name_english | object | category name in English |
| product_name_lenght | float64 | number of characters extracted from the product name |
| product_description_lenght | float64 | number of characters extracted from the product description |
| product_photos_qty | float64 | number of product published photos |
| product_weight_g | float64 | product weight measured in grams |
| product_length_cm | float64 | product length measured in centimeters |
| product_height_cm | float64 | product height measured in centimeters |
| product_width_cm | float64 | product width measured in centimeters |
| price | float64 | item price |
| order_quantity | int64 | sequential number identifying number of items included in the same order |
| freight_value | float64 | item freight value |
| delivery_duration | int64 | duration (days) from customer checkout until the product arrives at the customer's location |
| review_score | int64 | Note ranging from 1 to 5 given by the customer on a satisfaction survey |
| payment_value | float64 | transaction value |

## Pendekatan Analitis 📝
Berbagai teknik analisis data digunakan, termasuk eksplorasi data, segmentasi pelanggan berbasis RFM (Recency, Frequency, Monetary) & analisis regresi dalam pembangunan model ML. Pendekatan ini bertujuan untuk memberikan wawasan yang actionable kepada para stakeholder dan memberikan solusi yang praktis untuk meningkatkan kinerja bisnis.

## Hasil dan Rekomendasi ✅💹

Dalam analisis dataset Olist, ditemukan bahwa São Paulo merupakan state dengan pembelanjaan online tertinggi, diikuti oleh Rio de Janeiro. Produk yang laris di São Paulo meliputi Bed Bath Table, Health & Beauty, dan lainnya. Harga dan berat produk memiliki dampak positif pada pendapatan, sementara review negatif memiliki dampak sebaliknya. Puncak musim belanja terjadi dari Mei hingga Agustus dengan Black Friday menonjol. Mayoritas pembayaran dilakukan dengan kartu kredit atau Boleto. Waktu pengiriman rata-rata adalah 5-10 hari, dengan yang terlama terjadi di utara Brasil. Analisis RFM mengidentifikasi pelanggan yang berpotensi untuk loyalitas dan churn. Strategi pemasaran termasuk pemberian promo khusus untuk mengurangi churn dan implementasi program loyalitas untuk meningkatkan kesetiaan pelanggan. Diketahui juga bahwa penetapan harga serta jumlah kuantitas produk yang terjual menjadi salah satu faktor penting dalam mengoptimalkan revenue yang didapatkan oleh para Merchant.

**`Model Overview:`** Setelah melalui Cross Validation dan Hyperparameter Tuning, model Random Forest terpilih sebagai model terbaik untuk memprediksi Revenue Merchant Olist. Model ini memiliki nilai R-Squared sebesar 86.1%, menunjukkan bahwa sekitar 86% variabilitas revenue dapat dijelaskan oleh fitur-fitur yang ada. Median Absolute Error yang rendah (8.4) juga menandakan ketepatan prediksi model.

![image](https://github.com/PurwadhikaDev/EnigmaGroup_JC_DS_OL_12_C_FinalProject/assets/109770559/82cb5082-92b4-446f-aa9c-82c23665ff3b)

| Metrics | Random Forest Tuned |
|:-----:|:-----:|
| R^2 |0.861012|
| MedAE |8.400692|

**`Faktor Pengaruh Revenue:`** Harga barang dan kuantitas penjualan menjadi faktor utama yang memengaruhi revenue. Penamaan judul dan deskripsi produk, biaya dan lama pengiriman, serta review score juga berperan penting dalam menentukan jumlah revenue. Faktor-faktor yang dapat mempengaruhi pelanggan untuk memberikan ulasan yang baik:

- Fast transactions.
- Convenient payment methods.
- Price and value.
- Customer service.
- Product quality.
- Information quality.
- Delivery quality.

**`Catatan untuk Analisis Lanjutan:`** Untuk meningkatkan akurasi prediksi, dianjurkan untuk menambahkan data dengan fitur tambahan seperti sub kategori barang dan jenis ekspedisi. Model ML perlu disempurnakan terus-menerus melalui penyetelan hyperparameter dan eksperimen dengan algoritma alternatif.

**`Sebelum & Setelah Implementasi ML:`** Sebelum implementasi ML, merchant mengalami kesulitan dalam mengoptimalkan stok barang dan merencanakan keuntungan. Setelah implementasi ML, merchant dapat mengevaluasi data penjualan masa lampau, melakukan simulasi penjualan, dan mengoptimalkan stok barang untuk memaksimalkan revenue.

## Tableau Dashboard 📊
Kami Juga menyediakan dashboard interaktif menggunakan Tableau untuk memudahkan melihat data secara visual. untuk dapat mengaksesnya dapat membuka link dibawah ini:

[Tableau Link](https://public.tableau.com/app/profile/teguh.saputra4922/viz/Olist_update_cs_17114927683690/RevR)

# References (Daftar Pustaka)

- https://www.statista.com/forecasts/289746/e-commerce-revenue-forecast-in-brazil
- https://www.linkedin.com/advice/1/how-do-you-use-customer-behavior-increase#:~:text=Customer%20behavior%20is%20a%20key%20factor%20in,strategies%20to%20increase%20your%20revenue%20and%20profitability.
- https://www.kimkim.com/c/brazil-in-august-travel-tips-weather-and-more
- https://www.brazileducation.info/education-system/academic-year-and-language-of-instruction-in-brazil.html
- https://documentation.bloomreach.com/engagement/docs/rfm-segmentation
- https://www.sciencedirect.com/science/article/pii/S1877050910004229
- https://ejournals.ph/article.php?id=16559#:~:text=Five%20factors%20contributed%20to%20this,distributing%20questionnaires%20to%20393%20respondents.
- https://www.shopify.com/id/retail/inventory-shortages
- https://finance.cornell.edu/accounting/topics/inventories
- https://www.symson.com/pricing-studies/price-optimisation-guide
- https://www.oreilly.com/library/view/machine-learning-for/9781786469878/9f44e711-deb6-42de-abbd-524832ad32cc.xhtml
