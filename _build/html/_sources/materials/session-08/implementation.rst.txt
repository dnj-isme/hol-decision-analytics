Implementasi Naive Bayes
============================

.. note::
  
  Untuk session ini, kita akan menggunakan dataset berikut: `Customer Behaviour </assets/session-08/Customer_Behaviour.csv.xlsx>`_

  Source: https://www.kaggle.com/datasets/denisadutca/customer-behaviour

1. Split data menjadi dua bagian: training dan testing. Untuk langkah ini, gunakan operator Split Data. Gunakan 80% sebagai rasio training dan 20% sebagai rasio testing.

2. Lakukan preprocessing data terhadap dataset training dan testing. Ikuti langkah-langkah berikut:

  a. Filter Examples untuk menghapus data kosong
  b. Select attributes, optional (User ID, Gender, Age, EstimatedSalary, Purchased)
  c. Map (untuk kolom Gender, dari Female menjadi 0 dan Male menjadi 1)
  d. Parse Numbers (untuk kolom Gender)
  e. Normalize (untuk semua kolom, kecuali User ID dan Purchased)
  f. Set Role (User ID sebagai *id*, dan Purchased menjadi "label")

  .. image:: /assets/session-08/preprocess.png
    :width: 800px
    :align: center

3. Buat model Naive Bayes dengan menggunakan operator Naive Bayes. Gunakan dataset training sebagai inputnya.

  .. note::
    Gunakan node "Naive Bayes (Kernel)" untuk membuat model Naive Bayes dengan. Kernel memungkinkan kita untuk mengatur weight dari masing-masing kelas.

4. Hubungkan model Naive Bayes yang sudah digunakan dengan node Apply Model. Tujuannya supaya kita dapat mengevaluasi model yang sudah kita buat.
5. Untuk mengevaluasi model yang sudah kita buat, gunakan operator Performance (Classification). Hubungkan node Apply Model dengan node Performance.
6. Jika sudah selesai, tekan tombol Run untuk melihat hasilnya.

.. image:: /assets/session-08/full-process.png
    :width: 800px
    :align: center

Analisa Result
---------------

Setelah proses selesai, kita akan mendapatkan hasil berupa confusion matrix. Confusion matrix adalah tabel yang digunakan untuk menggambarkan kinerja model klasifikasi pada set data uji yang nilai sebenarnya diketahui.

.. image:: /assets/session-08/confusion-matrix.png
    :width: 800px
    :align: center

Berdasarkan matrix ini, kita dapat melihat total akurasi dari model yang sudah kita buat adalah 95%. Artinya, model yang sudah kita buat sudah cukup baik dalam melakukan prediksi.

.. note::

  Hasil dari matriks ini mungkin akan berbeda dengan hasil yang akan kalian dapatkan.