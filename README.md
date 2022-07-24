# Customer-Lifetime-Value-In-The-Company-Of-Car-Insurance

Divisi Development dari sebuah perusahaan asuransi mobil ingin melakukan prediksi skor customer lifetime value (CLV) bagi para pelanggannya. Customer Lifetime Value atau disingkat dengan CLV merupakan sebuah prediksi atas nilai total pendapatan yang bisa perusahaan dapatkan dari satu pelanggan. CLV adalah nilai yang penting untuk diketahui karena membantu perusahaan membuat keputusan tentang berapa banyak uang yang akan diinvestasikan untuk mendapat pelanggan baru dan mempertahankan pelanggan yang sudah ada.

Pada project kali ini business objective yang hendak dicapai adalah untuk memperoleh sistem prediksi yang dapat digunakan untuk mengetahui aspek apa saja yang memengaruhi perolehan hasil customer lifetime value (CLV) dari sebuah perusahaan asuransi mobil. Keluaran yang diharapkan yaitu prediksi hasil customer lifetime values dari suatu pelanggan.

Pendekatan machine learning yang diterapkan pada project ini adalah supervised learning berupa regression problem. Sistem akan memprediksi nilai kontinu berupa customer lifetime value score. Untuk permulaan, root mean squared error akan digunakan sebagai rangkuman pengukuran error pada model prediksi. Apabila nanti ditemukan pencilan pada error model, metrik lain seperti mean absolute error akan dipertimbangkan. Kemudian R-squared akan dihitung untuk melihat seberapa baik model dalam menjelaskan data yang ada.

Model Regresi Linier dengan Random Forest menjadi model yang terbaik untuk data ini dengan koefisien determinasi 92.17% dan kesalahan absolut rata-rata 321.42, yang berati model regresi ini mampu mempresentasikan data dengan baik sebesar 92.17%. Dengan hasil yang cukup tinggi ini, dapat diyakini bahwa model ini mampu untuk digunakan pada proses prediksi skor Customer Lifetime Value pelanggan di masa depan.

Pada hyperparameter tuning dengan RandomizedSearch, parameter terbaik yang dihasilkan adalah {'n_estimators': 1200, 'min_samples_split': 6, 'min_samples_leaf': 2, 'max_features': 'auto', 'max_depth': 10}. Jika masih ingin mencoba meng-improve model Random Forest ini, kita bisa coba melakukan tuning pada scaler.

Dari fitur-fitur yang ada memang tidak memiliki korelasi yang signifikan terhadap nilai Customer Lifetime Value (CLV) suatu pelanggan. Sebaiknya perusahaan perlu menambahkan lagi fitur-fitur yang mampu meningkatkan prediksi nilai CLV pelanggan, seperti jumlah tanggungan keluarga atau jumlah pengeluaran kebutuhan masing-masing pelanggan.
