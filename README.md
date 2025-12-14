## 📝 Deskripsi Proyek Capstone Project ASAH

---

### **ID Tim dan Use Case**

* **ID Tim:** **A25-CS248**
* **Use Case:** **AC-06 Customer Segmentation for Personalized Retail Marketing**

Use case ini berfokus pada pembangunan sistem segmentasi pelanggan yang memungkinkan bisnis ritel menerapkan strategi pemasaran yang lebih personal, efektif, dan berbasis data. Pendekatan yang digunakan mengintegrasikan metode RFM Analysis (Recency, Frequency, Monetary) sebagai model utama untuk mengukur nilai dan perilaku pelanggan secara objektif.

🔍 Mengapa RFM?

RFM adalah teknik analisis pelanggan yang terbukti efektif untuk mengidentifikasi kelompok pelanggan berdasarkan:

* Recency (R): Seberapa baru pelanggan melakukan transaksi terakhir.
* Frequency (F): Seberapa sering pelanggan bertransaksi.
* Monetary (M): Berapa banyak uang yang dihabiskan pelanggan.

Ketiga dimensi ini memungkinkan pengelompokan pelanggan ke segmen bernilai strategis seperti Loyalist, Big Spender, At Risk, Hibernating, dan New Customers. Hasil segmentasi kemudian digunakan untuk merancang strategi pemasaran yang lebih personal, retargeting yang tepat sasaran, dan pengembangan program loyalitas.

---

### **👥 Anggota Tim (Machine Learning)**

| Nama Anggota | ID Anggota | Peran |
| :--- | :--- | :--- |
| **M. Ryan Rifqi Firdaus** | M891D5Y1037 | Machine Learning |
| **Nida Rofi'Ah Hassan** | M891D5X1507 | Machine Learning |
| **Fajar Agus Dwi Rahmawan** | M891D5Y0577 | Machine Learning |

---

## Deskripsi Dataset Transaksi Ritel

---

Dataset transaksi ritel yang digunakan berfungsi untuk memetakan **profil pelanggan**, **perilaku pembelian**, **preferensi produk**, serta **riwayat transaksi** yang dibutuhkan dalam analisis **RFM** dan segmentasi lanjutan.

### **I. Informasi Pelanggan (Customer Information)**

Bagian ini mencakup data demografi dan kontak unik setiap pelanggan:

* **Customer ID:** Pengenal unik untuk setiap pelanggan.
* **Transaction_ID:** Detail transaksi yang dilakukan pelanggan.
* **Address, City, Country, State, Zipcode:** Detail geografis lokasi pelanggan.
* **Age:** Usia pelanggan.
* **Gender:** Jenis kelamin pelanggan.
* **Income:** Tingkat atau kategori pendapatan pelanggan.
* **Date:** Tanggal Transaksi.

### **II. Detail Transaksi (Transaction Details)**

Metrik utama yang berkaitan dengan aktivitas belanja pelanggan:

* **Quantity:** Jumlah total pembelian barang pada satu transaksi yang dilakukan.
* **Unit Price:** Harga satuan barang pada transaksi.
* **Subtotal:** Total Harga barang yang dibeli dalam satu transaksi.

### **III. Informasi Produk (Product Information)**

Detail spesifik mengenai barang yang dibeli:

* **Product Category:** Kategori produk yang dibeli (misalnya, elektronik, pakaian, buku).
* **Product Name:** Nama produk yang dibeli.

### **IV. Logistik dan Umpan Balik (Logistics & Feedback)**

Informasi mengenai pengiriman, pembayaran, dan kepuasan pelanggan:

* **Payment Method:** Metode pembayaran yang dipilih pelanggan.
* **Order Status:** Status pesanan (misalnya, terkirim, dalam proses pengiriman, dibatalkan).

---

### **Nilai Utama Dataset**

Dataset ini menyediakan dasar yang kuat untuk memahami perilaku pelanggan secara mendalam. Dengan menggabungkan informasi demografi, riwayat pembelian, dan detail produk, bisnis dapat memperoleh pandangan yang lebih lengkap mengenai kebutuhan serta preferensi pelanggan.

Melalui pemanfaatan dataset ini, perusahaan dapat:

1. **Mengembangkan strategi pemasaran yang lebih terarah**, sesuai dengan karakteristik dan pola transaksi dari setiap kelompok pelanggan.
2. **Meningkatkan tingkat loyalitas pelanggan** dengan mengidentifikasi segmen yang menunjukkan penurunan aktivitas dan menerapkan pendekatan yang lebih proaktif.
3. **Mendukung pengambilan keputusan terkait manajemen produk**, termasuk perencanaan persediaan dan evaluasi performa kategori, berdasarkan pola belanja yang terungkap dari data.

---

## 🚀 Cara Menjalankan (Quick Start)

### Langkah 1: Persiapan Akun Kaggle
Agar bisa mendownload dataset secara otomatis, Anda memerlukan API Token dari Kaggle:
1. Login ke akun [Kaggle](https://www.kaggle.com/).
2. Buka menu **Settings** (klik foto profil > Settings).
3. Scroll ke bawah ke bagian **API** dan klik tombol **Create New Token**.
4. File bernama `kaggle.json` akan terdownload ke komputer Anda. Simpan file ini.

### Langkah 2: Buka di Google Colab
Klik tombol di bawah ini untuk membuka notebook langsung di Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/A25-CS248/Capstone-ASAH/blob/main/Final_Capstone_(A25_CS248).ipynb)

### Langkah 3: Jalankan Program
Agar program berjalan lancar tanpa error versi library, ikuti langkah ini:

1. Download file `requirements.txt` dari repository ini ke komputer Anda.
2. Di dalam Google Colab, buka panel **Files** (ikon folder di kiri).
3. **Upload** file `requirements.txt` tersebut ke dalam sesi Colab.
4. Jalankan sel kode pertama pada notebook untuk menginstall library:
   ```python
   !pip install -r requirements.txt
```
5. Klik menu **Runtime** > **Run all** (atau Jalankan Semua).
6. Saat diminta, klik tombol **Choose Files** dan upload file `kaggle.json` yang Anda dapatkan di Langkah 1.
7. Dataset akan otomatis terdownload dan diekstrak.

---

**Catatan:**
Project ini menggunakan library versi spesifik:
- Scikit-learn: 1.8.0
- Yellowbrick: 1.5
- Plotly: 5.24.1
