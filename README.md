# Analyzing-eCommerce-Business-Performance-with-SQL

**Tool** : PostgreSQL & Google Data Studio

**Programing Languange** : SQL 

# Problem Statement #

Dalam suatu perusahaan mengukur performa bisnis sangatlah penting untuk melacak, memantau, dan menilai keberhasilan atau kegagalan dari berbagai proses bisnis. Oleh karena itu, dalam paper ini akan menganalisa performa bisnis untuk sebuah perusahan eCommerce,  dengan memperhitungkan beberapa metrik bisnis yaitu pertumbuhan pelanggan, kualitas produk, dan tipe pembayaran.

# Objective #

Membuat quey untuk menampilkan beberapa analisis diantaranya adalah : 

1. Annual Customer Activity Growth
2. Annual Product Category Quality
3. Annual Payment Type Usage

# Stage 0 - Data Preparation #

Dataset ini merupakan dataset dari perusahaan E-Commerce Brazil dengan jumlah data 99441 dari Tahun 2016 - 2018. Dataset ini berisikan fitur dengan beberapa informasi seperti lokasi , rincian item, jenis pembayaran dan ulasan.

Adapun ERD dari dataset ini adalah sebagai berikut 

<img src="Stage 0/ERD Picture.PNG" />

# Stage 1 - Exploratory Data Analysis #

## 1. Annual Customer Activity Growth ##

Pada tahap ini , aktivitas pola pertumbuhan pelanggan tahunan dapat dianalisis dengan tabel dengan beberapa fitur atau kolom diantaranya adalah total customer baru, total customer yang melakukan repeat order dan rata rata order yang di lakukan oleh pelanggan

### Tabel Pertumbuhan Pelanggan Per Tahun ###

<img src="Stage 1/Table Annual Growth Customer Activity.PNG" />

### Perbandingan Rata Rata User Aktif dan User Baru  ###

<img src="Stage 1/Average Active User vs New Customer.PNG" />

### Insight ###

1. Terjadi peningkatan pada rata – rata user yang aktif  dan customer atau pelanggan baru secara signifikan untuk setiap tahunnya.
2. Peningkatan tertinggi untuk jumlah customer baru terjadi pada periode tahun 2016 ke 2017.
3. Total user yang aktif adalah sebanyak 9142 user selama periode 2016 – 2018 dan total customer baru adalah sebanyak 96.096 user selama periode 2016 – 2018.
4. Total aktif user saat ini adalah sebanyak 5338 user.

### Perbandingan Pelanggan Repeat Order dan Rata Rata Frekuensi Order  ###

<img src="Stage 1/Repeat Order vs Average Frequency Order.PNG" />

### Insight ###

1. Repeat order terbanyak terjadi pada periode tahun 2017 sebanyak 1256 order, dan terjadi penurunan pada periode 2018.
2. Total repeat order selama periode 2016 – 2018 adalah sebanyak 2426 order.
3. Untuk rata rata frekuensi order per tahunnya tidak mengalami kenaikan secara signifikan .


## Stage 2 - Annual Customer Activity Growth ##

Tabel ini merupakan hasil query untuk menentukan analisis terhadap produk dengan kategori penjualan terbaik, jumlah pendapatan dan kategori produk yang sering mengalami pembatalan order.

<img src="Stage 2/table.PNG" />

### Total Pendapatan Produk Terbaik   ###

<img src="Stage 2/Total Revenue.PNG" />

### Insight ###

1. Dari analisis ini , terlihat bahwa pendapatan perusahaan untuk tiap tahunnya mengalami peningkatan.

2. Tiap tahunnya tiap kategori yang menyumbang pendapatan tertinggi mengalami perubahan.

### Perbandingan Produk Terbaik dan Produk Gagal Beli ###

<img src="Stage 2/top product vs most cance product.PNG" />

### Insight ###

Dari analisis ini , kategori produk yang mengalami cancel terbanyak mengalami perubahan tiap tahunnya. 

Untuk kategori health beauty merupakan kategori yang menyumbang pendapatan terbanyak sekaligus cancel order terbanyak juga, dikarenakan produk health beauty ini mendominasi transaksi selama periode 2018

## Stage 3 - Annual Payment Analysis ##

Tabel ini berisikan informasi mengenai jumlah user yang melakukan pembayaran dari berbagai platform. 

<img src="Stage 3/Table.PNG" />

### Perbandingan Platfom Pembayaran Paling Diminati ###

<img src="Stage 3/annual payment.PNG" />

### Insight ###

1. Secara keseluruhan metode pembayaran yang paling banyak diminati adalah jenis kartu kredit.

2. Namun kenaikan secara signifikan juga terjadi pada metode pembayaran kartu debit pada periode 2017 - 2018, sebaliknya untuk voucher yang mengalami penurunan.

3. Hal ini bisa terjadi karena adanya bisnis kerja antara ecommerce dengan lembaga bank yang bersangkutan.

## Summary ##

1. Berdasarkan aspek pertumbuhan customer , peningkatan customer baru terbanyak terjadi pada periode 2016 - 2017 dari 326 customer menjadi 43.708 customer

2. Seiring pertambahan customer dari tahun ke tahun , namun penurunan repeat order juga terjadi di periode 2018 dilihat berdasarkan indicator frekuensi rata rata order

3. Berdasarkan aspek kategori kualitas produk, total pendapatan perusahaan terjadi peningkatan setiap tahunnya, dan produk yang paling banyak diminati adalah kategori beauty health.

4. Berdasarkan aspek kategori pembayaran, kartu kredit merupakan tipe pembayaran yang paling banyak digunakan oleh customer dalam membeli barang. 
















