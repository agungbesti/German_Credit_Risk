# Klasifikasi Risiko Kredit Bank di Jerman   - Agung Besti
---
# Domain Proyek
---
Bank merupakan lembaga keuangan yang berpengaruh dalam bidang perekonomian suatu negara serta menghimpun dana dari masyarakat dalam bentuk simpanan maupun menyalurkan kembali kepada masyarakat dalam bentuk pinjaman. Kegiatan umum bank pada dasarnya merupakan memobalisasi dana dari masyarakat untuk disalurkan kepada perorangan atau suatu lembaga yang membutuhkan dana pinjaman. Pinjaman pada bank merupakan salah satu bagian pembentukan modal yang dilakukan oleh lembaga keuangan, pada hal ini pihak perbankan dapat mendorong masyarakat dalam menyalurkan kinerja usaha, sehingga dapat dimanfaatkan untuk meningkatkan produktivitas yang dilakukan oleh masyarakat individu maupun suatu lembaga. Sebagai industri yang bergerak pada dunia financial technology (**Fintech**) yang terus berkembang dan memiliki kegiatan usaha yang beragam, perbankan memiliki risiko yang semakin kompleks dan tentunya melakukan proses persetujuan yang dilakukan manual akan memakan banyak waktu [1]. 

Dalam menjalankan fungsinya, perbankan dapat mengoptimalkan penyaluran pinjaman kepada masyarakat. Akan tetapi pinjaman yang diberikan oleh pihak bank tidak menutup kemungkinan mengandung risiko, sehingga dalam pelaksanaannya bank harus memperhatikan asas–asas perkreditan yang sehat serta memiliki fundamental yang lebih kuat, supaya pinjaman dapat dilaksanakan secara konsisten dan berdasarkan asas–asas pinjaman yang sehat. Risiko dalam hal ini merupakan **potensi terjadinya suatu peristiwa yang dimana dapat menimbulkan kerugian** pada pihak bank [2][3].

**Oleh sebab itu, diperlukan suatu aplikasi yang dapat mengklasifikasi secara akurat, bagaimana tingkat risiko kegagalan bayar dalam peminjaman bank dapat dihindari, sehingga mempercepat memberikan sebuah persetujuan kredit peminjaman tanpa perlu memeriksa secara manual informasi pribadi pemohon.**

Pada kasus ini, aplikasi machine learning secara spesifik akan mengklasifikasi tingkat risiko kegagalan bayar dalam suatu kredit peminjaman, sehingga dapat dijadikan acuan oleh pihak bank dalam memberikan kredit peminjaman di Bank Jerman, dalam menetapkan keputusan apakah kredit peminjaman itu **Disetujui** atau **Tidak**.

## Alasan Penting yang Mendasari Proyek ini:
---
Alasan penting yang mendasari bahwa permasalahan kredit gagal bayar, yaitu sebagai berikut:
- Kegagalan bayar menyebabkan kerugian yang akan timbul oleh pihak yang memberi pinjaman **Bank**.
- Penilaian pengajuan secara manual akan menjadikan penilaian secara **subjektif** apabila yang mengajukan peminjaman memiliki hubungan dengan pihak yang akan melakukan Approval. Hal ini tentunya akan berpengaruh terhadap ancaman gagal bayar atau melebihi durasi waktu yang telah ditentukan untuk melunasi.
- Untuk menyelesaikan masalah tersebut, maka akan dibuat aplikasi yang dapat mengklasifikasi tingkat kegagalan pembayaran (dalam kasus ini sebagai pedoman atau acuan dalam menentukan apakah yang melakukan peminjaman berisiko tinggi atau rendah) dalam melakukan pelunasan.
- Aplikasi ini akan memanfaatkan teknologi Machine Learning serta bahasa pemrograman Python dalam membuat klasifikasi tingkat risiko untuk menjadi bahan keputusan bagi pihak Bank dalam memberikan sebuah **Approval**.

## Hasil Riset Terkait:
---
- [Transparent Decision Support System for Credit Risk Evaluation: An automated credit approval system](https://ieeexplore.ieee.org/document/9242905) 
- [Credit Risk Assessment for Rural Credit Cooperatives based on Improved Neural Network](https://ieeexplore.ieee.org/document/8104372)
- [Theoretical and Applied Aspects of Bank Credit Risks Minimization](https://ieeexplore.ieee.org/document/9468056)


# Business Understanding
---
Dari latar belakang yang telah dijelaskan sebelumnya, maka Bank X memerlukan suatu aplikasi atau program yang mampu menentukan apakah peminjam memiliki risiko tinggi untuk gagal bayar.
Oleh sebab itu, diperlukan sistem yang mampu mengklasifikasikan dari **informasi pengguna** maupun **informasi bank akun** untuk mengetahui bagaimana tingkat risiko kegagalan bayar sehingga hasil tersebut mampu menjadi bahan pertimbimbangan pengambilan keputusan bagi pihak Bank.
## Problem Statements
---
Berdasarkan penjelasan yang telah disampaikan sebelumnya, maka problem statements (rumusan masalah) yaitu sebagai berikut:
- Apa faktor yang dapat mempengaruhi bahwa peminjam tersebut memiliki risiko gagal bayar ?
- Bagaimana persebaran data dari setiap atributenya berdasarkan tingkat risikonya?
- Bagaimana hubungan fitur kategorikal dengan risiko kegagalan pembayaran ?
- Bagaimana korelasi antara tingkat risiko dengan fitur yang lainnya ?
- Bagaimana hasil dari penerapan model machine learning yang dilakukan?
- Apa saja tiga (3) model algoritma yang memberikan akurasi yang paling tinggi?
- Model algoritma apa yang mampu memberikan akurasi paling tinggi dibandingkan yang lainnya?
 

## Goals
---
Tujuan yang ingin dicapai dari pembuatan aplikasi klasifikasi kegagalan bayar di Bank Jerman ini, yaitu sebagai berikut:
- Mengetahui faktor-faktor yang mempengaruhi kegagalan bayar.
- Mengetahui hubungan fitur kategorikal dengan risiko kegagalan pembayaran.
- Mengetahui korelasi antara tingkat risiko dengan fitur yang lainnya.
- Mengetahui model algoritma yang mampu memberikan akurasi paling tinggi.
- Membuat aplikasi yang dapat mengklasifikasikan risiko kegagalan bayar secara akurat, sebagai bahan pengambilan keputusan dalam memberikan Approval terhadap peminjam.

### Solution statements
---
- Solusi yang dapat dilakukan untuk menangani permasalahan sebagaimana terdapat dalam problem statements, yaitu dengan membuat aplikasi yang dapat mengklasifikasikan risiko kegagalan bayar. Adapun aplikasi tersebut dibuat dengan menerapkan teknologi machine learning serta bahasa pemrograman python.
- Algoritma machine learning yang akan digunakan, yaitu **Linear Discriminant Analysis**, **LightGBM**  dan **XGBoost** Algorithm. Untuk mengukur keakuratan klasifikasi yang dilakukan oleh aplikasi yang dibuat, maka metrik yang digunakan adalah Confusion Matrix.

# Data Understanding
---
Data yang digunakan adalah dataset yang bersumber dari situs Kaggle yang berisi informasi kredit peminjaman bank di Jerman. Dataset tersebut dapat didownload pada link berikut ini:  [German Credit Risk](https://www.kaggle.com/datasets/kabure/german-credit-data-with-risk). Jumlah data yang terdapat didalam German Credit Risk sebanyak 1000 data dan 10 kolom.
## Sample Data
---
Ada pun sample data yang bisa dilihat seperti dibawah ini.

|#| Age | Sex  | Job | Housing | Saving_accounts | Checking_account | Credit_amount | Duration | Purpose | Risk |
|-|-------------------------------|--------|-----------------------|------------------------|----------------------|-------------|--------------|--------------|-----------|----------|
|1|67 | male| 2 | own | NaN| little | 1169| 6 | radio/TV | good|
|2|22 | female| 2 | own | little| moderate | 5951| 48 | radio/TV | bad|
|3|49 | male| 1 | own | little| NaN | 2096| 12 | education | good|
|4|45 | male| 2 | free | little| little | 7882| 42 | furniture/equipment | good|
|5|53 | male| 2 | free | little| little | 4870| 24 | car | bad|

###### Tabel 1 : Sample Data German Credit Risk
Untuk sample data bisa dilihat seperti pada Tabel 1.
## Variabel-variabel yang terdapat pada dataset German Credit Risk adalah sebagai berikut:
---
- Age = Umur pengaju
- Sex = Jenis kelamin pengaju
- Job = Jenis pekerjaan pengaju
- Housing = Status kepemilikan rumah pengaju
- Saving accounts = Rekening Tabungan pengaju
- Checking account = Rekening Giro pengaju
- Credit amount = Jumlah Pinjaman pengaju
- Duration = Waktu Pinjaman dibayarkan
- Purpose = Alasan peminjaman kredit
- Risk = Tingkat risiko pengajuan

## Langkah-Langkah dalam melakukan Data Understanding
---
Untuk memahami dataset, langkah-langkah yang dilakukan, yaitu sebagai berikut:
- Melakukan load dataset kedalam google colaboratory.
- Melakukan Exploratory data analysis untuk memahami makna-makna variabel yang terdapat dalam dataset.
- menggunakan teknik visualisasi data kategorikal dan non-kategorikal dengan menggunakan library seaborn.
- Memvisualisasikan data dengan menggunakan boxplot untuk mencari outlier.
- Melakukan univariative analysis untuk memahami sebaran data variabel.
- Melakukan multivariative analysis untuk memahami korelasi variabel kategorikal dan non-kategorikal terhadap variabel risk.

### Hasil Visualisasi Exploratory Data Analysis
---
|   #   |    Column     | Non-Null Count |  Dtype  |
|-------|--------------|----------------|---------|
|   0   |     Age     |    1000        | int64  |
|   1   |    Sex     |    1000        | object  |
|   2   |    Job     |    1000        | int64  |
|   3   |   Housing    |    1000        | object   |
|   4   | Saving_accounts  |    817        | object |
|   5   | Checking_account  |    606        | object  |
|   6   | Credit_amount |    1000        | int64   |
|   7   | Duration |    1000        | int64   |
|   8   |  Purpose   |    1000        | object   |
|   9   |     Risk      |    1000        | object   |
###### Tabel 2 : Melihat kolom dan tipe data pada dataset 
Pada Tabel 2 dapat dilihat bahwa data memiliki 6 kolom numerik atau angka sedangkan sisanya non-numerik atau kategorikal.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/75294c2b-9f6b-457c-93ed-4aaccaf971ff)
###### Gambar 1: Univariate Analysis pada variabel Sex
Pada Gambar 1 dapat dilihat bahwa orang yang berjenis kelamin **laki-laki memiliki distribusi data yang lebih banyak sekitar 69%** dibandingkan perempuan.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/82d2f3c0-aeaa-4058-90d7-7ef3eccf947b)
###### Gambar 2: Univariate Analysis pada variabel Job
Pada Gambar 2 dapat dilihat bahwa orang yang pekerjaanya **memiliki keahlian khusus memiliki distribusi yang paling banyak** dibandingkan dengan yang lainnya. Hal ini menegaskan bahwa sebagian besar peminjam diisi oleh orang - orang yang sudah mempunyai pekerjaan.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/c406f9c1-782c-45a2-bedb-52cc19507765)
###### Gambar 3: Univariate Analysis pada variabel Housing
Pada Gambar 3 dapat dilihat bahwa orang yang **status kepemilikan rumahnya telah memiliki** memiliki distribusi yang paling banyak dibandingkan dengan yang lainnya. Hal ini menegaskan bahwa sebagian besar peminjam diisi oleh orang - orang yang sudah memiliki kemampuan ekonomi yang cukup.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/79709a81-2fbd-4ba7-a475-3a38948509fb)
###### Gambar 4: Univariate Analysis pada variabel Saving_accounts
Pada Gambar 4 dapat dilihat bahwa orang yang melakukan peminjaman kredit diisi oleh orang - orang yang memiliki **saldo rekening yang kecil**. Hal ini menegaskan bahwa sebagian besar peminjam diisi oleh orang - orang yang memiliki kemampuan ekonomi yang cukup dengan pengeluaran yang besar, sehingga tabungan yang tersisa cenderung lebih sedikit.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/50670479-020c-428f-8fb2-2d0fac784336)
###### Gambar 5: Univariate Analysis pada variabel Checking_account
Pada Gambar 5 dapat dilihat bahwa orang yang melakukan peminjaman kredit sebagian besar tidak memiliki rekening giro, sebaran data ini berlaku bagi yang lainnya.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/cf5653c6-4b74-41df-8d81-1fbe7ff8ad66)
###### Gambar 6: Univariate Analysis pada variabel Purpose
Pada Gambar 6 dapat dilihat bahwa orang yang melakukan peminjaman kredit paling banyak digunakan untuk melakukan pembelian sebuah **Mobil (car)**. Hal ini menegaskan bahwa sebagian besar peminjam diisi oleh orang - orang yang **menginginkan kebutuhan sekundernya terpenuhi**, dibandingkan dengan kebutuhan primernya yaitu **pendidikan (education)** yang hanya memiliki alasan peminjaman sebanyak 6%.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/2656663d-b012-415b-ab12-75d6078e6221)
###### Gambar 7: Univariate Analysis pada variabel Age_category
Pada Gambar 7 dapat dilihat bahwa orang yang melakukan peminjaman kredit diisi oleh kelompok anak dewasa akhir [depkes 2019](https://ejournal.unesa.ac.id/index.php/mathunesa/article/view/19398/17715) rentang usia 25-35 tahun. Hal ini menegaskan bahwa sebagian besar peminjam diisi oleh orang - orang yang **sudah dewasa**, sedangkan untuk orang lansia cenderung tidak ada keinginan untuk melakukan peminjaman.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/44fc117f-2582-4f14-90c2-7c45ea21798f)
###### Gambar 8: Univariate Analysis pada variabel Credit_category
Pada Gambar 8 dapat dilihat bahwa orang yang akan melakukan peminjaman memiliki nilai yang hampir sama pada setiap distribusinya. Hal ini menegaskan bahwa jumlah pinjaman memiliki distribusi yang seimbang dengan yang lainnya.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/396b29b4-4895-4220-994b-55fa8d6d4e37)
###### Gambar 9: Univariate Analysis pada variabel Duration_category
Pada Gambar 9 dapat dilihat bahwa orang yang melakukan peminjaman kredit cenderung mengingikan **durasi yang lebih singkat**. Hal ini menegaskan bahwa sebagian besar peminjam menginginkan pinjaman yang relatif singkat untuk dilunasi.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/98e37f61-0a1d-4d28-a16d-73d6831b70dd)
###### Gambar 10: Univariate Analysis pada variabel Risk
Pada Gambar 10 dapat dilihat bahwa orang yang melakukan peminjaman kredit memiliki history **pembayaran yang cukup baik/tepat waktu sebanyak 70%** dibandingkan dengan gagal bayar/telat bayar. Hal ini menegaskan bahwa sebagian besar **data imbalanced**.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/e18a225b-e229-4923-8d8a-e37575709eb1)
###### Gambar 11: Multivariete Analysis pada variabel Sex dan Risk
Pada Gambar 11 dapat dilihat bahwa orang yang memiliki risiko tinggi gagal bayar cenderung dialami oleh **wanita sebesar 35%**. Hal ini menegaskan bahwa wanita memiliki **risiko gagal bayar atau telat bayar yang tinggi** dibandingkan pria.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/12b82885-e801-4384-ba68-8fefe4dffc7f)
###### Gambar 12: Multivariete Analysis pada variabel Job dan Risk
Pada Gambar 12 dapat dilihat bahwa sebaran data yang memiliki kegagalan bayar terhadap jenis pekerjaan cenderung hampir sama. Hal ini menegaskan bahwa jenis pekerjaan bukanlah satu - satunya yang menyebabkan gagal bayar.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/d31dc61c-6ba9-4715-9bbc-7e838189ebc9)
###### Gambar 13: Multivariete Analysis pada variabel Housing dan Risk
Pada Gambar 13 dapat dilihat bahwa orang yang **tidak memiliki rumah cenderung memiliki risiko tinggi gagal bayar/telat bayar** sebanyak 40%. Hal ini menegaskan bahwa siapapun yang tidak memiliki rumah dalam melakukan pinjaman cenderung memiliki risiko yang tinggi untuk gagal bayar/telat bayar.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/23eba721-ef92-4900-b823-43ea9e9ab7c2)
###### Gambar 14: Multivariete Analysis pada variabel Saving_account dan Risk
Pada Gambar 14 dapat dilihat bahwa **orang yang memiliki nilai tabungan rekening yang lebih rendah cenderung berpotensi tinggi untuk melakukan gagal bayar/telat bayar** sebesar 35%. Hal ini menegaskan bahwa tabungan yang sedikit cenderung berisiko untuk gagal bayar/telat bayar.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/27947039-d476-42a5-b53d-3aaa114b3e89)
###### Gambar 15: Multivariete Analysis pada variabel Checking_account dan Risk
Pada Gambar 15 dapat dilihat bahwa **orang yang memiliki rekening giro yang lebih kecil cenderung berpotensi tinggi untuk melakukan gagal bayar/telat bayar** sebesar 49%. Hal ini menegaskan bahwa rekening giro dengan nilai yang lebih kecil berpotensi tinggi untuk melakukan gagal bayar atau telat pelunasan.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/5cb9a54e-f13d-4104-ba09-08614d2bc696)
###### Gambar 16: Multivariete Analysis pada variabel Purpose dan Risk
Pada Gambar 16 dapat dilihat bahwa **orang yang memiliki alasan peminjaman untuk liburan (vacation) cenderung berpotensi tinggi untuk melakukan gagal bayar/telat bayar** sebesar 41%. Hal ini menegaskan bahwa orang - orang yang memiliki gaya hidup mewah cenderung memiliki risiko kegagalan bayar yang tinggi.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/f29f1592-1b65-4f87-b933-4236c791a2e9)
###### Gambar 17: Multivariete Analysis pada variabel Age_category dan Risk
Pada Gambar 17 dapat dilihat bahwa **usia anak antara 18-24 tahun (Student) berpotensi tinggi untuk melakukan kegagalan bayar/telat bayar** sebesar 42%. Hal ini menegaskan bahwa orang - orang yang masih remaja cenderung belum bisa bertanggung jawab untuk melakukan pelunasan peminjaman.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/93ad590e-ba20-4b6b-ab76-859d4dcb6b25)
###### Gambar 18: Multivariete Analysis pada variabel Credit_category dan Risk
Pada Gambar 18 dapat dilihat bahwa **jumlah pinjaman yang tinggi cenderung memiliki potensi untuk kegagalan bayar** sebesar 42%. Hal ini menegaskan bahwa semakin besar nilai pinjaman yang dilakukan maka semakin besar risiko untuk mengalami kegagalan bayar atau pelunasan tepat waktu.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/52fb96ca-487b-4f53-8668-06b14aab4653)
###### Gambar 19: Multivariete Analysis pada variabel Duration_category dan Risk
Pada Gambar 19 dapat dilihat bahwa **durasi yang lebih lama cenderung memiliki potensi tinggi untuk melakukan kegagalan bayar** sebesar 44%. Hal ini menegaskan bahwa semakin lama durasi yang diambil dalam waktu pelunasan, maka semakin besar pula risiko yang terjadi dalam kegagalan pembayaran atau pelunasan tepat waktu.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/1235f8b8-0df3-4f78-987e-d93610ee4e76)
###### Gambar 20: Descriptive Analysis pada variabel Purpose dan Credit_amount
Pada Gambar 20 dapat dilihat bahwa ketika orang yang mengambil kredit untuk tujuan tertentu seperti pembelian **Mobil atau Furnitur memiliki ketimpangan mencapai 60-80%** sementara untuk beberapa tujuan seperti pembelian Radio/TV atau Pendidikan masih berada diantara nilai yang sama.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/bf0efa80-3826-47e7-85ca-16e9a1a274a9)
###### Gambar 21: Descriptive Analysis pada variabel Purpose dan Sex
Pada Gambar 21 dapat dilihat bahwa **lebih banyak pria** mengambil pinjaman untuk mengambil mobil daripada perempuan. Sedangkan untuk pendidikan wanita dan pria hampir sama untuk jumlah orang yang melakukan peminjaman.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/342f0e5c-c5f9-4a4c-8e54-acfc7ad1ca9e)
###### Gambar 22: Confusion Matrix untuk Fitur Numerik
Pada Gambar 22 dapat dilihat bahwa untuk setiap fitur memiliki korelasi positif dan korelasi negatif yang tidak terlalu tinggi, dimana fitur yang paling berpengaruh yaitu **Job, Duration dan Credit_amount**. Sedangkan pada **fitur Age, memiliki korelasi yang paling kecil diantara fitur yang lainnya**.

![image](https://github.com/agungbesti/German_Credit_Risk/assets/35904444/2136066f-2473-4518-9655-2e645bf3704f)
###### Gambar 23: Chi Squared Tes antara Fitur Risk dan Kategori
Pada Gambar 23 dapat dilihat bahwa ada beberapa fitur kategorikal yang memiliki korelasi yang signifikan terhadap risiko kegagalan bayar.
Fitur - fitur yang memiliki korelasi yang signifikan terhadap Risk:
- Sex
- Housing
- Saving_account
- Checking_account
- Age_category
- Credit_category
- Duration_category

## Data Preparation


## Modeling


## Evaluation

