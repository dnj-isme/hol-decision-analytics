K-Means (Clustering)
=====================

K-Means adalah salah satu metode yang dapat kita gunakan untuk melakukan Clustering. Clustering sendiri adalah suatu proses **pengelompokkan** data ke dalam beberapa cluster (kelompok) yang memiliki kemiripan karakterisitik antar suatu data dengan data lainnya.  K-Means merupakan algoritma unsupervised learning yang berarti tidak memerlukan label atau target output dalam proses pembelajarannya. 

Cara kerja
-----------

Algoritma ini bekerja dengan cara mengelompokkan data ke dalam cluster-cluster yang memiliki jarak terdekat dengan centroid. Centroid sendiri adalah titik pusat dari cluster tersebut. Pada tahap awal, suatu titik centroid akan ditentukan (baik secara acak maupun ditentukan manual). Kemudian, setiap data akan dikelompokkan ke masing-masing cluster berdasarkan distancenya yang kemudian akan dicek apakah centroid dari cluster itu sudah sesuai atau belum.

1. Tentukan centroid

  .. image:: https://cdn.prod.website-files.com/61af164800e38cf1b6c60b55/642d4cb0de81f819f6e8266a_86.webp

2. Kelompokkan data berdasarkan centroid

  .. image:: https://cdn.prod.website-files.com/61af164800e38cf1b6c60b55/642d4cba2141ba3a7ead91ae_87.webp

3. Kemudian, tentukan centroid baru berdasarkan titik tengah dari cluster yang ada.

4. Ulangi langkah 2 dan 3 hingga titik-titik pada cluster tidak bervariasi

  .. image:: https://cdn.prod.website-files.com/61af164800e38cf1b6c60b55/642d4cc4952aaf746c233dcb_88.webp

