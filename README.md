# Customer-Personality-Analysis

## Latar Belakang
Sebuah perusahaan retail ingin mengetahui apakah perusahaan mereka mengalami peningkatan jumlah pelanggan atau mengalami penurunan jumlah pelanggan. Perusahaan kemudian mencoba mencari tahu kondisi mana yang menggambarkan perusahaan mereka saat ini dan menganalisa untuk segera membuat keputusan bisnis agar tetap berkelanjutan.

## Goals
Tujuan dilakukan Exploratory Data Analysis ini adalah untuk mengetahui dan mempertahankan pelanggan potensial

## Business Question
- Apakah perusahaan mengalami churn?
- Apakah tingkat pengeluaran pelanggan mempengaruhi churn rate?
- Apakah tingkat pendapatan pelanggan mempengaruhi churn rate?
- Apakah promosi yang ditawarkan perusahaan ke pelanggan mempengaruhi churn rate?
- Apakah tingkat pendidikan pelanggan mempengaruhi churn rate?
- Apakah status pernikahan pelanggan mempengaruhi churn rate?
- Apakah keluhan dari pelanggan mempengaruhi churn rate?
- Apakah tempat belanja mempengaruhi churn rate?

## Content
### Attributes
**People**

- ID: primary key
- Year_Birth: Tahun lahir pelanggan
- Education: Tingkat pendidikan pelanggan
- Marital_Status: Status pernikahan pelanggan
- Income: Pendapatan pelanggan tahunan
- Kidhome: Jumlah anak-anak dalam rumah tangga
- Teenhome: Jumlah remaja dalam rumah tangga
- Dt_Customer: Tanggal berlangganan seorang pelanggan dengan perusahaan
- Recency: Jumlah hari sejak pembelian terakhir pelanggan
- Complain: 1 apabila customer pernah memberi keluhan selama 2 tahun terakhir, 0 bila tidak ada keluhan

**Products**

- MntWines: Jumlah pengeluaran untuk membeli wine selama 2 tahun terakhir
- MntFruits: Jumlah pengeluaran untuk membeli buah selama 2 tahun terakhir
- MntMeatProducts: Jumlah pengeluaran untuk membeli produk daging selama 2 tahun terakhir
- MntFishProducts: Jumlah pengeluaran untuk membeli produk ikan selama 2 tahun terakhir
- MntSweetProducts: Jumlah pengeluaran untuk membeli permen selama 2 tahun terakhir
- MntGoldProds: Jumlah pengeluaran untuk membeli emas selama 2 tahun terakhir

**Promotion**

- NumDealsPurchases: Jumlah pembelian yang dilakukan menggunakan diskon
- AcceptedCmp1: 1 apabila pelanggan belanja dari campaign pertama
- AcceptedCmp2: 1 apabila pelanggan belanja dari campaign kedua
- AcceptedCmp3: 1 apabila pelanggan belanja dari campaign ketiga
- AcceptedCmp4: 1 apabila pelanggan belanja dari campaign keempat
- AcceptedCmp5: 1 apabila pelanggan belanja dari campaign kelima
- Response: 1 apabila pelanggan belanja dari campaign terakhir

**Place**

- NumWebPurchases: Jumlah pembelian yang dilakukan dari website perusahaan
- NumCatalogPurchases: Jumlah pembelian yang dilakukan dari katalog
- NumStorePurchases: Jumlah pembelian yang dilakukan dari toko offline
- NumWebVisitsMonth: Jumlah visit ke website perusahaan selama 1 bulan terakhir

#Analisa
## Apakah perusahaan mengalami churn?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q1.png)

Dilansir dari investopedia, churn rate adalah tingkat pelanggan berhenti melakukan hubungan bisnis dengan lembaga/perusahaan. Biasanya, churn rate dijelaskan sebagai persentase dari pelanggan yang memberhentikan layanan langganannya dengan periode waktu yang di tentukan.

Grafik di atas menjelaskan mengenai customer yang churned dan not churned. Data tersebut di atas didapat dari jumlah recency yang menjelaskan waktu terakhir kali customer belanja dari perusahaan, dengan periode waktu yang ditentukan adalah 1 bulan (30 hari). 

Dari grafik di atas menunjukkan bahwa perusahaan mengalami **churn**.

## Apakah tingkat pendapatan pelanggan mempengaruhi churn rate?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q2.png)

Terlihat bahwa barchart dari ke-4 kelompok tersebut identik, hampir tidak terlihat ada perbedaan. Hal ini menunjukkan bahwa perusahaan mengalami churn, tapi **BUKAN** dari kelompok pendapatan pelanggan. Sehingga, dapat disimpulkan bahwa pendapatan pelanggan **tidak mempengaruhi** terjadinya churn.

## Apakah tingkat pengeluaran pelanggan mempengaruhi churn rate?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q3.png)

Terlihat bahwa barchart dari ke-2 kelompok pengeluaran tersebut identik, hampir tidak terlihat ada perbedaan. Hal ini menunjukkan bahwa perusahaan mengalami churn, tapi **BUKAN** dari kelompok pengeluaran pelanggan. Sehingga, dapat disimpulkan bahwa pendapatan pelanggan **tidak mempengaruhi** terjadinya churn.

## Apakah promosi yang ditawarkan perusahaan ke pelanggan mempengaruhi churn rate?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q4_1.png)

Pada barchart di atas menampilkan mengenai promosi yang ditawarkan perusahaan pertama kali ke pelanggan. Dari grafik tersebut, dapat disimpulkan bahwa promosi yang ditawarkan perusahaan pertama kali ke pelanggan **mempengaruhi** terjadinya churn, dengan selisih antara pelanggan yang churn dan yang tidak sebesar **34,76%**.

![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q4_2.png)

Pada barchart di atas menampilkan mengenai promosi yang ditawarkan perusahaan kedua kali ke pelanggan. Dari grafik tersebut, dapat disimpulkan bahwa promosi yang ditawarkan perusahaan kedua kali ke pelanggan **mempengaruhi** terjadinya churn, dengan selisih antara pelanggan yang churn dan yang tidak sebesar **26,66%**.

![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q4_3.png)

Pada barchart di atas menampilkan mengenai promosi yang ditawarkan perusahaan ketiga kali ke pelanggan. Dari grafik tersebut, dapat disimpulkan bahwa promosi yang ditawarkan perusahaan ketiga kali ke pelanggan **mempengaruhi** terjadinya churn, dengan selisih antara pelanggan yang churn dan yang tidak sebesar **31,28%**.

![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q4_4.png)

Pada barchart di atas menampilkan mengenai promosi yang ditawarkan perusahaan keempat kali ke pelanggan. Dari grafik tersebut, dapat disimpulkan bahwa promosi yang ditawarkan perusahaan keempat kali ke pelanggan **mempengaruhi** terjadinya churn, dengan selisih antara pelanggan yang churn dan yang tidak sebesar **39,02%**.

![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q4_5.png)

Pada barchart di atas menampilkan mengenai promosi yang ditawarkan perusahaan kelima kali ke pelanggan. Dari grafik tersebut, dapat disimpulkan bahwa promosi yang ditawarkan perusahaan keempat kali ke pelanggan **mempengaruhi** terjadinya churn, dengan selisih antara pelanggan yang churn dan yang tidak sebesar **35%**.

![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q4_6.png)

Pada barchart di atas menampilkan mengenai promosi yang ditawarkan perusahaan terakhir kali ke pelanggan. Dari grafik tersebut, dapat disimpulkan bahwa promosi yang ditawarkan perusahaan terakhir kali ke pelanggan **mempengaruhi** terjadinya churn, dengan selisih antara pelanggan yang churn dan yang tidak sebesar **0,6%**.

Selisih terbesar terjadi pada promosi keempat sebesar 39,02%. Hal ini menunjukkan bahwa pada pelanggan memutuskan untuk menjadi churn paling banyak pada saat dilakukan promosi keempat dibandingkan promosi yang lainnya. Salah satu alasan mengapa terjadi churn adalah taktik komunikasi yang tidak menarik dan cenderung mengganggu menyebabkan pelanggan menarik diri mereka (retentionscience). Mengirim informasi yang sama sekali tidak relevan kepada pelanggan hanya akan membuat perusahaan tampak mengganggu dalam jangka pendek dan tidak mengerti apa-apa dalam jangka panjang. 

Untuk langkah selanjutnya, untuk metode promosi dapat diganti menggunakan email. Email promosi yang dikirimkan dibuat tanpa harus mengganggu pelanggan dengan spam. Selain itu, promosi ini juga dilakukan sebagai jawaban dari permasalahan pelanggan. Salah satu cara adalah menggunakan Machine Learning untuk melakukan prediksi produk apa yang kemungkinan besar akan dibutuhkan oleh pelanggan.

## Apakah tingkat pendidikan pelanggan mempengaruhi churn rate?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q5.png)

Terlihat bahwa barchart dari ke-2 kelompok pendidikan tersebut identik, hampir tidak terlihat ada perbedaan. Hal ini menunjukkan bahwa perusahaan mengalami churn, tapi **BUKAN** dari pengaruh tingkat pendidikan. Sehingga, dapat disimpulkan bahwa tingkat pendidikan pelanggan **tidak mempengaruhi** terjadinya churn.

## Apakah status pernikahan pelanggan mempengaruhi churn rate?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q6.png)

Terlihat bahwa barchart dari ke-2 kelompok status pernikahan tersebut identik, hampir tidak terlihat ada perbedaan. Hal ini menunjukkan bahwa perusahaan mengalami churn, tapi **BUKAN** dari pengaruh status pernikahan. Sehingga, dapat disimpulkan bahwa status pernikahan pelanggan **tidak mempengaruhi** terjadinya churn.

## Apakah keluhan dari pelanggan mempengaruhi churn rate?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q7.png)

Pada barchart di atas menampilkan mengenai pengaruh keluhan pelanggan terhadap churn. Dari grafik tersebut, dapat disimpulkan bahwa keluhan pelanggan terhadap perusahaan **mempengaruhi** terjadinya churn, dengan selisih antara pelanggan yang churn dan yang tidak sebesar **50,0%**. Hal ini menunjukkan bahwa pelanggan memutuskan untuk churn pada saat pelanggan mengajukan keluhan. 

Layanan pelanggan yang buruk sering kali dapat menyebabkan churn yang tinggi (profitwell). Solusi yang dapat diberikan untuk mengurangi angka churn akibat dari banyaknya keluhan pelanggan adalah dengan cara membuat customer support secara real-time, baik secara online maupun offline. Melakukan interaksi dengan pelanggan dalam membantu memecahkan masalah yang dihadapi oleh pelanggan. (Entrepreneur Asia Pacific)

## Apakah tempat belanja mempengaruhi churn rate?
![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q8_1.png)

Terlihat bahwa barchart dari ke-2 kelompok tersebut identik, hampir tidak terlihat ada perbedaan. Hal ini menunjukkan bahwa perusahaan mengalami churn, tapi **BUKAN** akibat dari pembelian melalui website. Sehingga, dapat disimpulkan bahwa kelompok pembelian melalui website **tidak mempengaruhi** terjadinya churn.

![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q8_2.png)

Terlihat bahwa barchart dari ke-2 kelompok tersebut identik, hampir tidak terlihat ada perbedaan. Hal ini menunjukkan bahwa perusahaan mengalami churn, tapi **BUKAN** akibat dari pembelian catalog. Sehingga, dapat disimpulkan bahwa kelompok pembelian melalui catalog **tidak mempengaruhi** terjadinya churn.

![](https://github.com/baressiym/Customer-Personality-Analysis/blob/main/Gambar_Chart/Biz_Q8_3.png)

Terlihat bahwa barchart dari ke-2 kelompok tersebut identik, hampir tidak terlihat ada perbedaan. Hal ini menunjukkan bahwa perusahaan mengalami churn, tapi **BUKAN** akibat dari pembelian on-site. Sehingga, dapat disimpulkan bahwa kelompok pembelian melalui on-site **tidak mempengaruhi** terjadinya churn.
