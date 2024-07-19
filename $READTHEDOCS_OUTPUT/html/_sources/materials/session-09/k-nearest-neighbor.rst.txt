K-Nearest Neighbors (kNN)
==========================

Algoritma k-Nearest Neighbors (kNN) adalah salah satu algoritma machine learning yang digunakan untuk melakukan klasifikasi dan regresi. Algoritma ini merupakan algoritma supervised learning, dimana algoritma ini akan diberikan dataset training sebagai basis pembelajarannya.

Algoritma kNN sendiri bekerja dengan memperhatikan kedekatan suatu data dengan data lainnya. Dalam implementasinya, algoritma ini menghitung jarak antara data yang akan diklasifikasikan dengan data-data lain dalam dataset, kemudian memilih k data tetangga terdekat (k-nearest neighbors).

Penghitungan Darak dalam kNN
-----------------------------
- **Euclidean Distance**, adalah jarak antara dua titik dalam ruang Euclidean. Jarak ini dihitung dengan rumus berikut:

    .. math::

        d(x, y) = \sqrt{\sum_{i=1}^{n} (x_i - y_i)^2}
- **Manhattan distance** merupakan jarak antara dua titik dalam ruang Euclidean. Jarak ini dihitung dengan rumus berikut:

    .. math::

        d(x, y) = \sum_{i=1}^{n} |x_i - y_i|
- **Minkowski distance**, merupakan generalisasi dari Euclidean dan Manhattan distance. Jarak ini dihitung dengan rumus berikut:

    .. math::

        d(x, y) = \left( \sum_{i=1}^{n} |x_i - y_i|^p \right)^{1/p}

    di mana :math:`p` adalah parameter yang digunakan untuk mengontrol jarak yang dihasilkan. Jika :math:`p = 1`, maka jarak yang dihasilkan adalah Manhattan distance, sedangkan jika :math:`p = 2`, maka jarak yang dihasilkan adalah Euclidean distance.
- **Hamming distance**, merupakan jarak yang digunakan untuk mengukur perbedaan antara dua vektor biner. Jarak ini dihitung dengan rumus berikut:

    .. math::

        d(x, y) = \sum_{i=1}^{n} |x_i - y_i|

    di mana :math:`x_i` dan :math:`y_i` adalah elemen ke-i dari vektor :math:`x` dan :math:`y`.


Reference
----------
- https://www.elastic.co/what-is/knn
- https://www.saedsayad.com/k_nearest_neighbors.htm