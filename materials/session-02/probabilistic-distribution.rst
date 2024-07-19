Probabilistic Distribution
===========================

Pendahuluan
------------

Probabilistic Distribution adalah metode untuk menggambarkan distribusi probabilitas dari suatu variabel acak. Metode ini digunakan untuk memodelkan ketidakpastian dalam data dan memprediksi kemungkinan hasil yang berbeda. 

Distribusi probabilitas adalah versi ideal dari distribusi frekuensi. Distribusi frekuensi menggambarkan sampel atau dataset tertentu. Ini adalah jumlah kali setiap nilai yang mungkin dari sebuah variabel muncul dalam dataset. Jumlah kali suatu nilai muncul dalam sampel ditentukan oleh probabilitas kemunculannya.

Contoh:

.. image:: https://upload.wikimedia.org/wikipedia/commons/thumb/8/8c/Standard_deviation_diagram.svg/250px-Standard_deviation_diagram.svg.png
    :alt: Distribution Diagram
    :align: center

Referensi: wikipedia

Contoh Kasus
-------------
Gunakan template di file berikut: :download:`Template.xlsx </assets/session-02/template.xlsx>`, lihat di page "Probabilistic Distribution"

Di sini, kita dapat menganalisa distribusi data dengan menggunakan variance, dan standard deviation.

Berikut adalah rumus untuk menghitung Variance:

.. math::
    \text{Variance} = \frac{\sum_ (x_i - \bar{x})^2}{N}

Sedangkan untuk standard deviation: :

.. math::
    \text{Standard Deviation} = \sqrt{\text{Variance}}

Untuk implementasi di Excel, lakukan beberapa step berikut:

#. Dapatkan probabilitas di P(x) dengan cara Frequency / Total Frequency
#. Untuk menghitung Expected Value (E(x)), gunakan rumus E(x) = P(x) * x. x di sini adalah score (sumbu X).
#. Jumlahkan E(x) di semua baris, maka nilai mean (rata-rata) sudah ditemukan.
#. Ikuti rumus (x - mean)^2, lalu jumlahkan di semua baris sebagai hasil variance. ()
#. Dapatkan Standard Deviation dengan cara mengakar kuadratkan hasil variance. (=sqrt(variance))

Jika semuanya sudah benar, maka hasilnya akan seperti berikut:

.. image:: /assets/session-02/distribution-done.png
    :alt: Distribution Diagram
    :align: center