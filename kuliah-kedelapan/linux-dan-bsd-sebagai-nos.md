---
description: Mempelajari alasan mengapa Linux dan BSD sebagai NOS
---

# Linux dan BSD sebagai NOS

## Alasan Linux dan BSD dipilih sebagai NOS

Linux dan BSD (Berkeley Software Distribution) merupakan NOS yang paling sering digunakan sebagai sistem operasi bagi server. Terdapat beberapa alasan dibalik kepopuleran mereka, diantaranya:&#x20;

1.  Relatif Aman

    Ketika dibandingkan dengan sistem operasi _client_ seperti Windows, Linux dan BSD memiliki tingkat keamanan yang lebih tinggi karena beberapa hal ini: Hak Akses dan Hak Milik, Otentikasi pengguna _root_ yang lebih aman, Perangkat lunak sumber terbuka (_Open Source Software_), serta Pembaruan berkala.   &#x20;
2.  Dukungan Komunitas serta Enterprise

    Linux dan BSD dikembangkan oleh komunitas yang tersebar di seluruh dunia. Komunitas ini menyebabkan Linux dan BSD mampu memberikan pembaruan yang relatif cepat dibandingkan dengan sistem operasi sumber tertutup. Selain dikembangkan oleh komunitas, Linux dan BSD juga dikembangkan oleh beberapa _enterprise_ seperti Novell (OpenSUSE) dan Canonical (Ubuntu).&#x20;
3.  Open Source

    Linux dan BSD merupakan sistem operasi yang memiliki sumber terbuka (Open Source) serta lisensi GNU GPL (_General Public License_), hal tersebut berarti setiap orang mampu mengunduh, mempelajari, memodifikasi, menyalin, menggandakan, serta memperjualbelikan sistem operasi ini. Perangkat lunak _open source_ cenderung memiliki kemampuan untuk mendukung berbagai teknologi terkini, sehingga sistem operasi ini dapat digunakan pada platform paling modern sekalipun. Karena perangkat lunak yang tersedia pada sistem operasi ini memiliki sumber terbuka, pengelola server dapat menyesuaikan perangkat lunak sesuai dengan kebutuhan server.
4.  Lebih Reliabel

    Sistem operasi Linux dan BSD bekerja secara lebih reliabel karena terdapat lebih sedikit bug. Pada studi yang dilakukan oleh [Stanford University](https://www.wired.com/2004/12/linux-fewer-bugs-than-rivals/), Linux memiliki _bug_ yang jauh lebih sedikit dari jumlah rata-rata _bug_ yang ditemukan pada aplikasi komersial lainnya. Dalam 5,1 juta baris kode, hanya ditemukan 985 _bugs_. Nilai ini jauh lebih sedikit dibandingkan estimasi _bug_ pada perangkat komersial lainnya, yaitu 114.000 hingga 171.000. Selain memiliki lebih sedikit _bug,_ [Google mengatakan](https://www.zdnet.com/article/google-project-zero-finds-linux-developers-patch-security-holes-faster-than-anyone-else/) bahwa kerentanan sistem umumnya jauh lebih cepat untuk ditangani dibandingkan sistem operasi sumber tertutup yang dikeluarkan oleh Microsoft dan Apple.

## Pemilihan NOS yang Tepat

Terdapat beberapa komponen penting yang perlu diperhatikan ketika memilih sistem operasi jaringan yang tepat untuk server. Dengan mengetahui komponen ini, maka pengelola server dapat memilih pilihan yang tepat berdasarkan keperluan server.&#x20;

**Keamanan** merupakan salah satu komponen penting karena akan terdapat _n_-buah pengguna yang berada dalam jaringan yang sama, apabila pengelola server tidak mengutamakan keamanan pada server mereka, maka bukan tidak mungkin penyerang dapat mengambil informasi sensitif serta merusak server tersebut.

**Kenyamanan** merupakan komponen selanjutnya karena pada umumnya server dikelola dari jarak yang jauh. Apabila pengelola server tidak memiliki kemampuan untuk membuat koneksi terlindung (_Secure Shell_), maka pengalaman mengelola server akan jauh dari kata nyaman. Selain kenyamanan bagi pengelola server, kenyamanan pengguna layanan juga harus menjadi prioritas utama. Server yang baik akan mampu menyediakan kontennya tanpa memerlukan waktu tunggu yang lama bagi pengguna.

**Anggaran biaya** yang dapat digunakan merupakan komponen penting dalam memilih NOS yang tepat. Apabila pengelola server memiliki biaya yang memadai untuk membeli sistem operasi yang didukung oleh _enterprise_ (sebagai contoh, Red Hat Enterprise Linux)_,_ maka pada umumnya masalah yang ditemui saat mengelola server menjadi lebih sedikit, serta terdapat _customer service_ yang dapat dihubungi apabila terjadi suatu permasalahan pada sistem operasi tersebut. Namun, apabila pengelola server tidak memiliki anggaran untuk membeli NOS, maka ia dapat menggunakan sistem operasi dengan sumber terbuka. Hanya karena sebuah sistem operasi memiliki sumber terbuka, bukan berarti sistem operasi tersebut akan beroperasi dengan performa yang lebih buruk dibandingkan dengan sistem operasi berbayar.&#x20;

## Proses Manajemen NOS

Setelah memilih NOS yang tepat sebagai sistem operasi pada server, proses selanjutnya yang perlu diketahui adalah bagaimana cara melakukan manajemen NOS yang tepat sesuai dengan kebutuhan server yang dimiliki. Hal esensial untuk dapat melakukan manajemen NOS adalah:

* Memanajemen Pengguna.
* Mengatur Hak Akses dan Hak Milik atas suatu _file_ ataupun direktori.
* Konfigurasi suatu _service_ atau layanan.
* Melakukan _maintenance_ terhadap sistem operasi maupun layanan yang telah dipasang. __&#x20;

Untuk melihat pengguna mana yang sedang menggunakan suatu proses, pengelola server dapat menggunakan `glances` untuk memonitor proses yang sedang berjalan. Manajemen proses telah dijelaskan pada [Kuliah Kedua](broken-reference).

Hak Akses dan Hak Milik suatu _file_ maupun direktori dapat diatur menggunakan perintah `chmod` dan `chown`. Dengan mengatur Hak Akses dan Hak Milik, pengelola server dapat mengurangi kemungkinan eksploitasi server oleh pihak yang tak bertanggung jawab. Cara mengatur Hak Akses dan Hak Milik telah dijelaskan pada [Kuliah Kelima](broken-reference).

Melakukan konfigurasi _service_ atau layanan berfungsi untuk menyesuaikan layanan tersebut sesuai dengan keperluan server. __ Konfigurasi dapat dilakukan dengan cara melihat _file_ dengan ekstensi `.conf` pada direktori yang menyimpan layanan tersebut (umumnya terletak pada direktori `/bin`).

Pemeliharaan (_maintenance_) dapat dilakukan dengan cara mengatur _job_ khusus yang ditugaskan untuk memperbarui sistem beserta dengan layanan yang telah terpasang didalamnya. `cron` dapat digunakan sebagai alat untuk melakukan hal tersebut. Perintah yang diperlukan untuk melakukan pembaruan adalah `apt-get update && apt-get upgrade`.
