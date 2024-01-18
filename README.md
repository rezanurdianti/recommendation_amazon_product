# Project Recommendation Amazon Product

<ul>
    <li><b>Dataset (<a href="https://www.kaggle.com/datasets/saurav9786/amazon-product-reviews">Link Dataset</a>) </b>
      <ul> 
        <li>Situs web e-commerce online seperti Amazon menggunakan berbagai model rekomendasi untuk memberikan saran yang berbeda kepada pengguna yang berbeda. Saat ini, Amazon menggunakan collaborative filtering item-to-item, yang dapat menangani data besar dan menghasilkan rekomendasi berkualitas tinggi secara real-time. Jenis pemfilteran ini mencocokkan setiap item yang dibeli dan diberi peringkat pengguna dengan item serupa, lalu menggabungkan item serupa tersebut menjadi daftar rekomendasi untuk pengguna. Dalam proyek ini, kita akan membangun model rekomendasi untuk produk elektronik Amazon.

Dataset ini berisi informasi berikut:
<ul>
    <li>userId: ID pengguna yang memberikan rating</li>
    <li>productId: ID produk yang dirating</li>
    <li>Rating: Peringkat produk dari 1 hingga 5</li>
    <li>timestamp: Tanggal dan waktu rating diberikan</li>
</ul>

Dataset ini dapat digunakan untuk berbagai tujuan, termasuk:
<ul>
    <li>Analisis sentimen: Memahami sentimen pengguna terhadap produk tertentu</li>
    <li>Rekomendasi produk: Menemukan produk yang mungkin disukai pengguna berdasarkan rating mereka</li>
    <li>Pembelajaran mesin: Mengembangkan model untuk memprediksi peringkat produk atau untuk mengelompokkan rating</li>
</ul>

</li>
      </ul>
    </li>
    <li><b>Permasalahan dan Tujuan Eksperimen</b></li>
    
<b>Permasalahan</b>
yang dihadapi oleh situs web belanja online adalah bagaimana memberikan rekomendasi produk yang tepat bagi penggunanya. Hal ini penting untuk dilakukan karena dapat meningkatkan kepuasan pengguna dan mendorong mereka untuk melakukan pembelian.

<b>Tujuan Eksperimen</b>
adalah untuk membangun model rekomendasi produk untuk situs web belanja online. Model ini diharapkan dapat memberikan rekomendasi produk yang tepat bagi pengguna, berdasarkan data pembelian dan peringkat produk yang mereka miliki.
    <li><b>Model dan Alur tahapan Eksperimen</b></li>
    Model rekomendasi yang digunakan dalam contoh kode di atas adalah berdasarkan Collaborative Filtering dengan menggunakan Matrix Factorization menggunakan metode Singular Value Decomposition (SVD).

Dalam hal ini, model direpresentasikan sebagai matriks yang diuraikan (decomposed) menggunakan SVD menjadi tiga matriks lainnya. Matriks-matriks tersebut kemudian digunakan untuk menghitung korelasi antar item.

Berikut Tahapan Proses :
<ol type="1">
  <li>Ambil atau Download dataset</li>
  <li>Import Library</li>
  <li>Load Dataset</li>
  <li>Explore Dataset</li>
  <li>Preprocessing</li>
  <li>Analysis of rating given by the user</li>
  <li>Filtering Data</li>
  <li>Model Development</li>
  <li>Recommendation</li>
</ol><br>


<li><b>Performa Model / Uji Performa Model</b></li>
    Dalam konteks sistem rekomendasi, pengukuran performa model sangat penting untuk mengevaluasi sejauh mana model dapat memprediksi preferensi pengguna dengan akurat. Dua metrik yang umum digunakan untuk mengukur performa model adalah Mean Absolute Error (MAE) dan Root Mean Squared Error (RMSE).

1. **Mean Absolute Error (MAE):**
   - **Definisi:** MAE mengukur rata-rata dari selisih absolut antara nilai prediksi dan nilai sebenarnya.
   - **Penjelasan:** Semakin rendah nilai MAE, semakin baik kinerja model. Nilai MAE dapat diartikan sebagai rata-rata kesalahan prediksi dalam skala asli (nilai sebenarnya).

2. **Root Mean Squared Error (RMSE):**
   - **Definisi:** RMSE adalah akar kuadrat dari rata-rata dari kuadrat dari selisih antara nilai prediksi dan nilai sebenarnya.
   - **Penjelasan:** Seperti MAE, tujuan dari RMSE adalah meminimalkan kesalahan prediksi. RMSE cenderung memberikan "pembobotan" yang lebih tinggi pada kesalahan besar, yang dapat membuat model lebih sensitif terhadap outlier.

**Interpretasi:**
- Jika MAE atau RMSE mendekati nol, itu menunjukkan bahwa model memiliki kinerja yang sangat baik, dengan kesalahan prediksi yang sangat kecil.
- Jika MAE atau RMSE memiliki nilai yang tinggi, itu menunjukkan bahwa model memiliki kesalahan prediksi yang signifikan.

</ul>
