# 🧩 RFM-Analysis-Online-Retail

### 🇬🇧 English — 🇮🇩 Bahasa Indonesia

---

## 🏢 Business Understanding | Pemahaman Bisnis

**Problem:**
Only have basic customer data but want to know customer behaviour to plan marketing strategy accordingly.
**Masalah:**
Hanya memiliki data dasar pelanggan tetapi ingin memahami perilaku pelanggan untuk merencanakan strategi pemasaran yang tepat.

**Question:**
How to understand customer behaviour to plan marketing strategy accordingly?
**Pertanyaan:**
Bagaimana memahami perilaku pelanggan untuk merencanakan strategi pemasaran yang sesuai?

**Measure:**
A well-clustered customer base based on the basic data that we have.
**Ukuran Keberhasilan:**
Basis pelanggan yang terkelompok dengan baik berdasarkan data dasar yang dimiliki.

---

## 📊 Data Understanding | Pemahaman Data

![1](https://user-images.githubusercontent.com/35904444/102911291-68e88800-44ae-11eb-8a67-3b6aab597461.PNG)

---

## 🧹 Data Cleaning and Preparation | Pembersihan dan Persiapan Data

![2](https://user-images.githubusercontent.com/35904444/102911455-a77e4280-44ae-11eb-98bc-32cf203ae905.PNG)

---

## 🔍 Exploratory Data Analysis | Analisis Data Eksploratif

* 80% of sales come from customers in the United Kingdom.
* 80% hasil penjualan berasal dari pelanggan negara United Kingdom.

![3](https://user-images.githubusercontent.com/35904444/102911854-37bc8780-44af-11eb-93d1-77fdfc8b6aac.PNG)

* Top 10 Customers with Highest Spending (Monetary Value)
* 10 Pelanggan dengan Pengeluaran Tertinggi (Nilai Moneter)

![4](https://user-images.githubusercontent.com/35904444/102912043-89fda880-44af-11eb-90fd-ef1bd656943f.PNG)

* Top 10 Items Contributing to Overall Sales
* 10 Produk Teratas yang Memberikan Kontribusi Penjualan Terbesar

![5](https://user-images.githubusercontent.com/35904444/102912046-8b2ed580-44af-11eb-95c3-fb6b740c147b.PNG)

* Top 10 Items Sold
* 10 Produk Terlaris

![6](https://user-images.githubusercontent.com/35904444/102912049-8bc76c00-44af-11eb-8eb2-d8acac23ec30.PNG)

---

## 🤖 Data Modelling | Pemodelan Data

Clustering based on RFM metrics:
Pengelompokan berdasarkan metrik RFM:

> **R (Recency):** Number of days since last purchase
> **R (Recency):** Jumlah hari sejak pembelian terakhir

![7](https://user-images.githubusercontent.com/35904444/102912808-76067680-44b0-11eb-8b1e-939c5a04b60c.PNG)

> **F (Frequency):** Number of transactions
> **F (Frequency):** Jumlah transaksi

![8](https://user-images.githubusercontent.com/35904444/102912814-77d03a00-44b0-11eb-982f-eaf986bca622.PNG)

> **M (Monetary):** Total amount of transactions
> **M (Monetary):** Total nilai transaksi

![9](https://user-images.githubusercontent.com/35904444/102912825-7a329400-44b0-11eb-9724-88b07f094fdf.PNG)

---

## 🧠 Conclusion | Kesimpulan

1. **Core — Your Best Customers**

   * **RFM Score:** 222
   * **Who They Are:** Highly engaged customers who have bought the most recent, most often, and generated the most revenue.
   * **Siapa Mereka:** Pelanggan yang paling aktif, sering berbelanja, dan memberikan pendapatan tertinggi.

   ![10](https://user-images.githubusercontent.com/35904444/102914090-5f611f00-44b2-11eb-80fe-668c563fad57.PNG)

---

2. **Loyal — Your Most Loyal Customers**

   * **RFM Score:** X2X
   * **Who They Are:** Customers who buy most frequently.
   * **Siapa Mereka:** Pelanggan yang paling sering berbelanja.

   ![11](https://user-images.githubusercontent.com/35904444/102914332-b2d36d00-44b2-11eb-9911-bf6a8e1cdeab.PNG)

---

3. **Whales — Your Highest Paying Customers**

   * **RFM Score:** XX2
   * **Who They Are:** Customers who generate the highest revenue.
   * **Siapa Mereka:** Pelanggan dengan total pembelian tertinggi.

   ![14](https://user-images.githubusercontent.com/35904444/102914688-4442df00-44b3-11eb-9001-2a91a2be20fe.PNG)

---

4. **Rookies — Your Newest Customers**

   * **RFM Score:** 20X
   * **Who They Are:** First-time buyers on your site.
   * **Siapa Mereka:** Pembeli baru yang pertama kali melakukan transaksi.

   ![17](https://user-images.githubusercontent.com/35904444/102915100-d3e88d80-44b3-11eb-8a0a-1a9a1baa41bb.PNG)

---

5. **Slipping — Once Loyal, Now Gone**

   * **RFM Score:** 00X
   * **Who They Are:** Previously loyal customers who haven’t purchased for a long time.
   * **Siapa Mereka:** Pelanggan lama yang dulunya loyal, tetapi sudah lama tidak berbelanja lagi.

   ![20](https://user-images.githubusercontent.com/35904444/102915805-f9c26200-44b4-11eb-99d5-f3b33a339d47.PNG)

---

6. **Regular — Average Customers**

   * **RFM Score:** Remaining scores
   * **Who They Are:** Customers with average metrics across each RFM score.
   * **Siapa Mereka:** Pelanggan dengan nilai rata-rata di setiap aspek RFM.

   ![23](https://user-images.githubusercontent.com/35904444/102915816-fd55e900-44b4-11eb-85d6-502a46e3550e.PNG)

---

7. **RFM Segments Overview | Gambaran Umum Segmen RFM**

   ![26](https://user-images.githubusercontent.com/35904444/102915825-ffb84300-44b4-11eb-9a01-97297d188666.PNG)

---

## 🧰 Tools and Libraries Used | Alat dan Pustaka yang Digunakan

| English                                                                 | Bahasa Indonesia                                                                  |
| ----------------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| **Python** – Programming language used for data analysis and modelling. | **Python** – Bahasa pemrograman yang digunakan untuk analisis dan pemodelan data. |
| **pandas** – For data manipulation and cleaning.                        | **pandas** – Untuk manipulasi dan pembersihan data.                               |
| **NumPy** – For numerical computation.                                  | **NumPy** – Untuk perhitungan numerik.                                            |
| **Matplotlib & Seaborn** – For data visualization.                      | **Matplotlib & Seaborn** – Untuk visualisasi data.                                |
| **scikit-learn (sklearn)** – For clustering and RFM segmentation.       | **scikit-learn (sklearn)** – Untuk klasterisasi dan segmentasi RFM.               |
| **Jupyter Notebook** – For analysis and reporting.                      | **Jupyter Notebook** – Untuk analisis dan pelaporan hasil.                        |

---

## 📚 References | Referensi

* [RFM Analysis Concept – Marketing Analytics](https://en.wikipedia.org/wiki/RFM_%28market_research%29)
* Online Retail Dataset – UCI Machine Learning Repository

---
