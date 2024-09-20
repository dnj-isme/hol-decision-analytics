Implementasi k-Nearest Neighbors
=================================

.. note::

  Untuk session ini, kita akan menggunakan dataset berikut: :download:`Car Evaluation </assets/session-09/car.csv>`

  Source: https://archive.ics.uci.edu/dataset/19/car+evaluation

1. Split data menjadi dua bagian: training dan testing. Gunakan operator Split Data. Gunakan 80% sebagai rasio training dan 20% sebagai rasio testing.

2. Lakukan preprocessing data terhadap dataset training dan testing. Ikuti langkah-langkah berikut:

  a. Filter Examples untuk menghapus data kosong
  b. Map (untuk mengubah attribut polynomial)

    * Untuk attribute **buying**, **maint**, dan **safety**; ubah map menjadi sebagai berikut:

      - low = 1
      - med = 2
      - high = 3
      - vhigh = 4
    * Untuk attribute **doors**, ubah "5more" menjadi 5
    * Untuk attribute **person**, ubah "more" menjadi 6
    * Untuk attribute **lug_boot**, ubah map menjadi sebagai berikut:

      - small = 1
      - med = 2
      - big = 3
    * Untuk attribute **class**, ubah map menjadi sebagai berikut:

      - unacc = 1
      - acc = 2
      - good = 3
      - vgood = 4 

  c. Parse Numbers (untuk kolom polynomial menjadi numeric)

  d. Normalize (untuk semua kolom, kecuali *class*)
  e. Set Role (attribute **class** sebagai "label")

  .. image:: /assets/session-09/preprocess.png
    :width: 800px
    :align: center

3. Buat model k-NN dengan menggunakan operator Naive Bayes. Gunakan dataset training sebagai inputnya. Serta ubah nilai **k** menjadi 4 (karena ada 4 class).
4. Hubungkan k-NN yang sudah digunakan dengan node Apply Model. Tujuannya supaya kita dapat mengevaluasi model yang sudah kita buat.
5. Untuk mengevaluasi model yang sudah kita buat, gunakan operator Performance (Classification). Hubungkan node Apply Model dengan node Performance.
6. Jika sudah selesai, tekan tombol Run untuk melihat hasilnya.


.. image:: /assets/session-09/full-process.png
  :width: 800px
  :align: center

Analisa Result
---------------

.. note::
  
    Hasil dari matriks ini mungkin akan berbeda dengan hasil yang akan kalian dapatkan.

Setelah proses selesai, kita dapat melihat confusion matrix kita. Pada gambar di bawah ini, kita dapat lihat bahwa accuracy kita adalah 92% yang berarti model kita sudah cukup baik dalam melakukan prediksi.

.. image:: /assets/session-09/result.png
  :width: 800px
  :align: center

Reference
----------
- https://archive.ics.uci.edu/dataset/19/car+evaluation