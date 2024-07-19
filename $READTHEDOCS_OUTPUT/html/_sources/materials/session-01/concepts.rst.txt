Basic Concepts
===============

Sebelum kita mengolah data, kita perlu memahami data apa yang akan kita olah. Oleh karena itu, kita perlu memahami konsep-konsep data tersebut.

Populasi dan Sampel
--------------------

1. **Cerita #1**

  .. pull-quote::
    Seorang analis sedang diberi tugas untuk mencari tahu daya beli pelanggan di usahanya. Analis tersebut kemudian meminta divisi keuangan dan penjualan untuk memberikan data penjualan dan data keuangan. Data ini kemudian diolah dan dianalisa untuk mengetahui daya beli pelanggan di tahun 2020 di Indonesia. Setelah diolah, analis tersebut mendapatkan kesimpulan bahwa daya beli pelanggan di tahun 2020 di Indonesia mengalami penurunan secara signifikan. Dia juga dapat mengetahui demografi pelanggan yang paling banyak berbelanja di usahanya.

2. **Cerita #2**

  .. pull-quote::
    Seorang guru ingin mengetahui pengaruh konsumsi anak terhadap kemampuan anak dalam memahami materi. Guru tersebut mewawancarai semua orang tua murid di kelas 5 SD di sekolah tersebut. Hasil pengumpulan data ini akan dikelompokkan dan dianalisa, kemudian hasil laporannya dikirimkan ke kepala sekolah.

Mari kita analisa kedua cerita di atas.

Pada cerita pertama, kita bisa lihat bahwa data yang digunakan adalah data penjualan dan data keuangan. Dimana data penjualan ini adalah data penjualah ke **semua** pembeli yang melakukan transaksi di perusahaan tersebut. Hal ini disebut sebagai **populasi**. **Populasi** adalah kumpulan dari **semua** elemen yang memiliki nilai kepentingan yang sama. Di cerita pertama, populasi adalah **semua** pelanggan di perusahaan tersebut.

Sedangkan di cerita kedua, data yang digunakan adalah data performa murid dan hasil wawancara orang tuanya. Jika ruang lingkup penelitian ini hanya di satu kelas, maka data ini dapat dinyatakan sebagai **populasi**. Tapi, apakah data yang berasalkan dari kelas 5 SD itu mewakili **seluruh** anak di dunia? di Indonesia? ataupun di sekolah tersebut yang terdiri dari lebih dari 1 kelas? Jawabannya **belum tentu**, guru ini hanya menjadikan sebagian murid di sekolah itu (yaitu murid di kelas 5 SD) sebagai **sampel**. **Sampel** adalah sebagian dari populasi yang diambil untuk dianalisa.


**Kesimpulan**

.. pull-quote::
  **Populasi** adalah kumpulan dari semua elemen yang memiliki nilai kepentingan yang sama. Sedangkan **sampel** adalah sebagian dari populasi yang diambil untuk dianalisa.

Data Set, Variabel, dan Jenis-Jenisnya
----------------------------------------

Setelah kita memahami apa itu populasi dan sampel, maka langkah berikutnya adalah kita memahami mengenai data yang akan kita olah. Dalam analisa data quantitative, data yang akan kita olah biasanya berupa **data set**. Mari kita lihat tabel berikut ini:

.. _Customer Information:
.. list-table:: Customer Information
   :widths: 10 15 10 15 15 20 10 25 10 20
   :header-rows: 1

   * - **ID**
     - **Name**
     - **Gender**
     - **Phone**
     - **Referral**
     - **Address**
     - **Salary**
     - **Additional Info**
     - **Subscription**
     - **Last Purchase Date**
   * - 001
     - John Doe
     - Male
     - 123-456-7890
     - Website
     - 123 Main St, Anytown
     - $50,000
     - Regular customer, preferred shipping address: 123 Main St.
     - Gold
     - 2024-05-01
   * - 002
     - Jane Smith
     - Female
     - 987-654-3210
     - Referral program
     - 456 Elm St, Othertown
     - $80,000
     - VIP customer, frequent purchases, Email: jane@example.com
     - Platinum
     - 2024-04-20
   * - 003
     - Bob Brown
     - Male
     - 555-123-4567
     - Friend
     - 789 Oak St, Anycity
     - $40,000
     - New customer, referred by friend
     - Silver
     - 2024-04-15
   * - 004
     - Emily Johnson
     - Female
     - 333-222-1111
     - Advertisement
     - 321 Pine St, Newville
     - $60,000
     - Loyalty program, email: emily@example.com
     - Gold
     - 2024-05-05
   * - 005
     - Michael Lee
     - Male
     - 444-555-6666
     - Social media
     - 555 Maple Ave, Sunnytown
     - $70,000
     - Regular customer, local resident
     - Bronze
     - 2024-04-28
   * - 006
     - Sarah Wilson
     - Female
     - 666-777-8888
     - Word of mouth
     - 666 Oak St, Sunnycity
     - $55,000
     - VIP member, frequent shopper
     - Gold
     - 2024-05-10
   * - 007
     - David Brown
     - Male
     - 777-888-9999
     - Website
     - 777 Pine St, Othertown
     - $65,000
     - New customer
     - Silver
     - 2024-05-02
   * - 008
     - Lisa Miller
     - Female
     - 888-999-0000
     - Referral program
     - 888 Elm St, Anytown
     - $75,000
     - Regular customer
     - Platinum
     - 2024-05-08

Dari tabel tersebut kita bisa melihat berbagai informasi mengenai pelanggan. Misalnya, jenis kelamin, jenis *subscription*, gaji, dan lainnya. Informasi ini disebut sebagai **variabel**. **Variabel** adalah karakteristik dari suatu *unit* dari populasi.

Dalam analisa suatu data, kita juga perlu mengetahui karakteristik dari variabel dalam data set. Jenis-jenis variabel yang bisa diolah adalah:

- **Variabel Numerik**: Variabel yang berupa angka, dimana variabel ini dapat diolah secara matematis. Contoh: gaji, umur, dan lainnya.

  Variabel numerik dibagi menjadi dua jenis:

  - **Variabel Diskrit**: Variabel numerik yang berupa bilangan bulat. Contoh: umur, jumlah anak, dan lainnya.
  - **Variabel Kontinu**: Variabel numerik yang merupakan hasil dari pengukuran yang bisa dilakukan secara terus-menerus. Contoh: gaji, berat badan, dan lainnya.

  Dalam variabel numerik, kita juga dapat melakukan pengelompokan lagi, misalnya dari umur, kita kelompokkan menjadi anak-anak, remaja, dewasa, dan lansia. Hal ini disebut sebagai **binned variable** atau **discretized variable**.

- **Variabel Kategorik**: Variabel yang berupa kategori, dimana variabel ini tidak dapat diolah secara matematis. Contoh: jenis kelamin, *subscription*, dan lainnya.
  
  Variabel kategorik dibagi menjadi dua jenis:
  
  - **Variabel Ordinal**: Variabel kategorik yang memiliki tingkatan. Contoh: *subscription* (Bronze, Silver, Gold, Platinum).
  - **Variabel Nominal**: Variabel kategorik yang tidak memiliki tingkatan. Contoh: jenis kelamin.

- **Variabel Dummy** atau **Variabel Indikator**: Variabel yang berupa angka 0 atau 1, dimana variabel ini digunakan untuk menggantikan variabel kategorik. Contoh: "Male" dan "Female" diubah menjadi 0 dan 1.

Dalam analisa data, ada juga yang dinamakan **time series**, yaitu data yang dilakukan berdasarkan suatu satuan waktu. Dalam mengkategorikan time series tersebut, ada juga istilah **cross-sectional data**, yaitu data yang dikelompokkan dalam suatu rentang waktu tertentu. Contoh: data penjualan per hari, per kuartal, per tahun, dan lain sebagainya.


Latihan
--------
Berdasarkan table :ref:`Customer Information`, tentukan field apa saja yang merupakan contoh variabel dan tentukan jenisnya.