Visualisasi Linear Regression (Simple)
========================================================

Untuk demonstrasi, gunakan template di file berikut: `Template.xlsx </assets/session-03/template.xlsx>`_

Menampilkan Linear Regression pada Grafik
------------------------------------------

1. Buatlah grafik scatter dari data yang ada. Lihat materi sesi 1: `Data Visualization <../session-01/data-visualization.html>`_.

.. image:: /assets/session-03/scatter-empty.png
  :width: 400px
  :align: center

2. Pilih grafik scatter yang telah dibuat, lalu klik tombol + (Chart Element), Trendline, lalu More Options

.. image:: /assets/session-03/scatter-progress-1.png
  :width: 400px
  :align: center

3. Setelah itu, akan muncul suatu menu di sebelah kanan Excel. Pastikan kalian memilih Trendline Options lalu pastikan jenis regressionnya adalah "Linear" dan centang "Display Equation on chart" agar kita bisa melihat rumus regression.

.. image:: /assets/session-03/scatter-progress-2.png
  :align: center

4. Maka tampilan grafik akan seperti berikut:

.. image:: /assets/session-03/scatter-done.png
  :width: 400px
  :align: center

Menemukan koefisien dari Linear Regression dengan manual
---------------------------------------------------------

Ingat rumus linear regression:

.. math::

  y = mx + b

di mana:

- :math:`y` adalah variabel dependen
- :math:`x` adalah variabel independen
- :math:`m` adalah kemiringan garis (*slope*)
- :math:`b` adalah *intercept* (titik potong dengan sumbu y)

Di sini, kita perlu menentukan nilai :math:`m` dan :math:`b` dari data yang ada.

Berikut adalah cara mencari nilai :math:`m` dan :math:`b`:

1. Hitung rata-rata dari kedua variabel (x dan y)
2. Hitung nilai :math:`m` dengan rumus berikut:

  .. math::    
    m = \frac{\sum_{i=1}^{n} (x_i - \bar{x})(y_i - \bar{y})}{\sum_{i=1}^{n} (x_i - \bar{x})^2}

  - :math:`n` adalah jumlah data
  - :math:`x_i` adalah nilai x pada data ke-i
  - :math:`y_i` adalah nilai y pada data ke-i
  - :math:`\bar{x}` adalah rata-rata dari x
  - :math:`\bar{y}` adalah rata-rata dari y

3. Hitung nilai :math:`b` dengan rumus berikut:

  .. math::
    b = \bar{y} - m\bar{x} 

  - :math:`\bar{x}` adalah rata-rata dari x
  - :math:`\bar{y}` adalah rata-rata dari y
  - :math:`m` adalah kemiringan garis (*slope*)

4. Setelah mendapatkan nilai :math:`m` dan :math:`b`, kita bisa mendapatkan rumus linear regression. Kita bisa memasukkan nilai x untuk menemukan prediksi tingkat kebahagian berdasarkan usia.

Latihan
--------

Selesaikan template di tab **Manual Method** dari file `Template.xlsx </assets/session-03/template.xlsx>`_.

Jika perhitungan sudah benar, maka hasilnya akan seperti berikut:

.. image:: /assets/session-03/linear-formula.png
  :width: 400px
  :align: center
