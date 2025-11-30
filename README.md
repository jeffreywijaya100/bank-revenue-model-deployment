**Machine Learning API for Predicting Long-Term Deposit Subscription — Banking Revenue Optimization**

Pada proyek ini, saya berperan sebagai data scientist di sebuah institusi perbankan dengan tanggung jawab untuk mengembangkan sistem prediktif yang membantu meningkatkan penerimaan revenue bank. Bank mengalami penurunan pendapatan karena rendahnya minat nasabah untuk berinvestasi melalui deposito jangka panjang. Untuk mengatasi hal ini, dibutuhkan solusi berbasis machine learning yang dapat mengidentifikasi nasabah dengan potensi tertinggi untuk berlangganan deposito, sehingga strategi pemasaran dapat dilakukan secara lebih efektif dan tepat sasaran.
Penjelasan data diberikan dalam table dibawah:

![image](https://github.com/user-attachments/assets/ba3e174c-b4d3-41e7-b11f-b8ffc74eef65)

📌 Tahapan Pengerjaan
1. Machine Learning Modeling

  - Melakukan data pre-processing untuk memastikan kualitas dataset sebelum pemodelan, meliputi:
  
    - Handling missing values
  
    - Encoding categorical features
  
    - Feature scaling
  
    - Train–test split
  
  - Melatih model klasifikasi menggunakan 2 algoritma machine learning:
  
    - Logistic Regression
    
    - Random Forest (atau sesuai eksplorasi)
  
  - Menggunakan classification report (accuracy, precision, recall, F1-score) untuk membandingkan performa masing-masing model
  
  - Menentukan model terbaik dan menyimpannya dalam format .pkl (pickle) untuk keperluan deployment

2. Prediction Code for Deployment

  - Menyusun script inference untuk memuat model .pkl dan melakukan prediksi input data baru
  
  - Mengintegrasikan langkah preprocessing otomatis di dalam fungsi prediksi agar API hanya menerima raw input tanpa kebutuhan transformasi manual dari user

3. API Deployment using FastAPI

  - Membangun service API dengan FastAPI untuk melakukan prediksi deposito melalui metode POST
  
  - Endpoint menerima input data nasabah dan mengembalikan output:
  
    - "yes" → nasabah berpotensi tinggi berlangganan deposito
  
    - "no" → nasabah berpotensi rendah
  
  - Melakukan 3 test case via FastAPI untuk validasi API dengan screenshot hasil prediction untuk setiap request


**💼 Business Value & Real Impact**

Implementasi sistem deposit subscription prediction API dapat memberikan dampak signifikan terhadap strategi bisnis bank:

Dampak	Penjelasan

  - Optimasi strategi pemasaran	Bank dapat memfokuskan promosi, hadiah, dan tele-marketing pada nasabah yang memiliki peluang tinggi berlangganan deposito.
  - Peningkatan revenue	Konversi pemasaran yang lebih terarah meningkatkan penjualan produk deposito jangka panjang sehingga pendapatan bank meningkat.
  - Efisiensi biaya operasional	Mengurangi pemborosan biaya pemasaran karena target kampanye hanya ditujukan kepada segmen potensial.
  - Prediksi otomatis & skalabilitas	API dapat diintegrasikan ke CRM/website bank untuk memperoleh prediksi secara real-time tanpa keterlibatan manual dari tim data.
  - Pengambilan keputusan berbasis data	Memberikan insight yang terukur untuk manajemen dalam menyusun strategi pertumbuhan investasi.

**🎯 Ringkasan Keberhasilan Proyek**

  - Menghasilkan model machine learning terbaik berbasis classification
  
  - Mengonversi model menjadi sistem prediksi otomatis berbasis API FastAPI
  
  - Melakukan pengujian 3 skenario POST untuk memastikan API berjalan sesuai yang diharapkan
  
  - Solusi siap diintegrasikan ke arsitektur digital bank untuk mendukung campaign deposito yang lebih cerdas dan efektif
