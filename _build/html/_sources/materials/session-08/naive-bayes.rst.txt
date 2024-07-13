Naive Bayes
============

Naive Bayes adalah suatu metode klasifikasi yang berdasarkan teorema Bayes dengan asumsi bahwa semua prediktor adalah independen satu sama lain sesuai dengan prinsip probabilitas bersyarat (conditional probability).

Sebagai contoh, kita memiliki 2 koin dengan 2 sisi. Saat kita melempar kedua koin itu secara bersamaan, maka probabilitas munculnya sisi angka dan gambar masing-masing adalah 50%. Ruang sampelnya adalah sebagai berikut:

- Koin 1 = angka; Koin 2 = gambar
- Koin 1 = angka; Koin 2 = angka
- Koin 1 = gambar; Koin 2 = angka
- Koin 1 = gambar; Koin 2 = gambar


Jika kita perhatikan, probabilitas (P) hasil dari kedua koin tersebut adalah:

- Peluang kedua koin menunjukkan dua gambar = 1/4
- Peluang salah satu koin menunjukkan angka = 3/4
- Peluang koin kedua menunjukkan angka, dan koin pertama adalah gambar= 1/2
- Peluang koin kedua menunjukkan gambar, dan koin pertama adalah angka = 1/2

Rumus umum dari teorema Bayes adalah:

.. math::

    P(A|B) = \frac{P(B|A)P(A)}{P(B)}

Laplache Smoothing
-------------------

Dalam penerapan Naive Bayes, seringkali kita menemui masalah probabilitas nol. Misalnya, kita memiliki data yang berisi kata-kata yang muncul dalam dokumen. Jika suatu kata tidak muncul dalam dokumen, maka probabilitasnya adalah nol. Hal ini akan menyebabkan hasil klasifikasi menjadi tidak akurat. Hal ini disebabkan dengan teorema Naive Bayes yang mengasumsikan bahwa semua prediktor adalah independen satu sama lain. Untuk mengatasi masalah ini, kita dapat menggunakan metode Laplache Smoothing.

Laplache Smoothing ini bekerja dengan cara menambahkan nilai 1 pada setiap kemungkinan nilai yang muncul. Sehingga, probabilitas nol tidak akan muncul. Rumus dari Laplache Smoothing adalah:

.. math::

    P(w|c) = \frac{count(w,c) + 1}{count(c) + |V|}