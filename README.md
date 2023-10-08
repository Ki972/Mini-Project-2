# Mini-Project-2: Investigate Business Hotel using Data Visualization
## Latar Belakang
Analisis performa bisnis dalam industri perhotelan memiliki peran yang krusial dalam pengambilan keputusan yang lebih baik dan strategi pemasaran yang lebih efektif. Dalam konteks ini, Saya akan mengeksplorasi perilaku pelanggan yang melakukan pemesanan hotel, serta dampaknya terhadap tingkat pembatalan pemesanan hotel. Hasil analisis ini akan disajikan dalam bentuk visualisasi data untuk memberikan pemahaman yang lebih baik dan persuasif.
## Alat
Untuk melakukan analisis ini, Saya menggunakan bahasa pemrograman Python dan beberapa perpustakaan seperti pandas, matplotlib, dan seaborn. Alat yang digunakan yaitu **Google Colaboratory**
## Isi
### Data Preprocessing
- **Duplicate Data :**
Baris duplikat dihapus menggunakan fungsi `drop_duplicates()` untuk menghindari bias dalam analisis.

- **Missing Values :**
Nilai null diisi dengan nilai yang sesuai, seperti mengisi kolom "company" dan "agent" dengan 0, kolom "children" dengan 0 (kemungkinan sebagian besar tamu tidak memiliki anak), dan kolom "city" dengan "unknown."

- **Invalid Values :**
Nilai "Undefined" pada kolom "meal" diganti dengan "No Meal".

- **Drop Unnecessary Data :** 
Data yang tidak relevan atau tidak informatif dihapus, termasuk data dengan jumlah tamu dan durasi tinggal 0.

- **Change Data Types :**
Melakukan perubahan tipe data pada kolom “children”, “agent”, dan “company” karena kolom-kolom tersebut mewakili angka diskrit dan harus memiliki tipe data integer untuk melakukan analisis lebih lanjut.
### Analisis Data
### Monthly Hotel Booking Analysis Based on Hotel Type
Grafik menunjukkan perubahan rata-rata total pemesanan hotel setiap bulan untuk dua jenis hotel yang berbeda.

Pemesanan tertinggi untuk City Hotel terjadi pada bulan Juli, meskipun bukan yang tertinggi untuk Resort Hotel, namun juga mengalami kenaikan. Pada bulan tersebut, banyak tamu melakukan pemesanan karena bertepatan dengan masa liburan.

Namun, terdapat penurunan setelah masa liburan selesai, yang memerlukan analisis lebih lanjut untuk memahami penyebabnya.
### Impact Analysis of Stay Duration on Hotel Bookings Cancellation Rates
Analisis menunjukkan bahwa semakin lama menginap, semakin tinggi kemungkinan pesanan tersebut dibatalkan. City Hotel memiliki rasio pembatalan yang lebih tinggi daripada Resort Hotel untuk durasi menginap yang lebih lama (2 minggu, 3 minggu, dan 4 minggu).

Trend pada City Hotel juga menunjukkan kenaikan yang signifikan dibandingkan dengan Resort Hotel. Informasi ini dapat membantu manajemen hotel untuk memahami pola pembatalan pesanan dan mengidentifikasi durasi menginap yang berisiko tinggi untuk pembatalan, sehingga dapat mengambil langkah-langkah untuk mengurangi pembatalan, meningkatkan kepuasan pelanggan, dan meningkatkan efisiensi operasional.
### Impact Analysis of Lead Time on Hotel Bookings Cancellation Rate
Analisis menunjukkan bahwa City Hotel memiliki rasio pembatalan yang lebih tinggi dibandingkan dengan Resort Hotel untuk semua grup lead time. Resort Hotel cenderung memiliki rasio pembatalan yang lebih rendah, terutama untuk pemesanan dengan lead time yang lebih pendek.

Pemesanan dengan lead time yang sangat lama, yaitu 11-12 bulan dan lebih dari 12 bulan, memiliki risiko pembatalan yang tinggi, terutama di City Hotel. Informasi ini dapat membantu manajemen hotel dalam merencanakan strategi pemasaran dan kebijakan pembatalan yang lebih efektif.
## Kesimpulan
Analisis data pemesanan hotel memberikan wawasan yang berharga tentang perilaku pelanggan, dampak durasi menginap, dan pengaruh lead time terhadap tingkat pembatalan pemesanan hotel. Dengan pemahaman yang lebih dalam tentang faktor-faktor ini, manajemen hotel dapat mengambil tindakan yang lebih tepat untuk meningkatkan layanan dan efisiensi operasional mereka, serta mengoptimalkan strategi pemasaran untuk menarik lebih banyak tamu.
