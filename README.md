## customer-segmentation : Project Overview

- project ini menggunakan dataset flight.csv
- akan dilakukan clustering untuk customer yang sudah menggunakan layanan penerbangan menggunakan maskapai ini.
- metode segmentasi customer yang digunakan adalah metode RFM
- algoritma clustering yang digunakan adalah KMeans

Sekilas tentang KMeans:
- mencari centroid yang stabil untuk mengelompokkan data
- evalusasi model menggunakan elbow method untuk mencari jumlah cluster yang sesuai.

Informasi tentang Metode RFM :
* R – Recency : Fitur ini untuk melihat berapa hari yang lalu pelanggan melakukan transaksi terakhirnya.
* F – Frequency : berapa kali customer sudah melakukan transaksi
* M – Monetary : berapa banyak uang yang sudah dihabiskan oleh customer untuk bertransaksi

RFM pada dataset ini adalah:
- R = LAST_TO_END
- F = FLIGHT_COUNT
- M = SEG_KM_SUM

## Hasil
Dengan menggunakan KMeans didapatkan 4 cluster sebagai berikut

![alt text](https://github.com/annisahumaira21/customer-segmentation/blob/main/clustering.JPG)<br>

Berikut rata-rata dan median dari 4 cluster:

![alt text](https://github.com/annisahumaira21/customer-segmentation/blob/main/mean%20and%20median%20clustering.JPG)<br>

Jumlah customer dari masing-masing cluster:

![alt text](https://github.com/annisahumaira21/customer-segmentation/blob/main/total%20user%20clustering.JPG)<br>

## Summary
- Cluster 0 adalah penumpang yang memiliki rentang waktu rata-rata 96 hari dari pemesanan terakhir, jumlah penerbangan rata-rata 11x, total jarak penerbangan sekitar 16658 km. 
- Cluster 1 adalah penumpang yang memiliki rentang waktu rata-rata 124 hari dari pemesanan terakhir, jumlah rata-rata penenrbangan 4x, total jarak penerbangan sekitar 6152 km. 
- Cluster 2 adalah penumpang yang memiliki rentang waktu rata-rata 58 hari dari pemesanan terakhir, jumlah rata-rata penenrbangan 21x, total jarak penerbangan sekitar 28138 km.
- Cluster 3 adalah penumpang yang memiliki rentang waktu rata-rata 479 hari dari pemesanan terakhir, jumlah rata-rata penenrbangan 3x, total jarak penerbangan sekitar 5473 km.
