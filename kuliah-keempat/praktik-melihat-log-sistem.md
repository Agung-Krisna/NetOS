---
description: Mempelajari cara melihat log dalam sistem operasi linux
---

# Praktik Melihat Log Sistem

Dalam sistem operasi linux, setiap konfigurasi sistem yang tersimpan akan dapat dilihat sebagai sebuah file. Fenomena ini dikenal sebagai "_everything is a file_", hal tersebut memudahkan pengguna sistem operasi linux untuk melihat bahkan merubah setiap konfigurasi sistem sesuai dengan kebutuhannya masing-masing.&#x20;

Selain dapat melihat konfigurasi sistem yang tersimpan dalam sistem operasi linux, pengguna juga dapat melihat log mengenai riwayat perubahan yang terjadi didalam sistem tersebut. Dalam sistem operasi linux yang menggunakan distribusi debian, log terletak pada direktori`/var/log/`.

Untuk melihat riwayat perubahan yang berkaitan dengan sistem, pengguna dapat melihat file yang berada pada `/var/log/syslog.` Disarankan untuk menggunakan sebuah editor teks untuk melihat log yang berkaitan dengan sistem. Untuk mendapatkan sebuah editor teks "nano" pada sistem operasi linux, ketikkan perintah ini pada terminal:

```
sudo apt-get install nano
```

Setelah mendapatkan sebuah editor teks, maka hal selanjutnya yang dapat dilakukan adalah membaca isi dari log sistem. Biasanya, untuk melakukan hal tersebut, pengguna dapat mengetikkan perintah ini pada terminal:

```
nano /var/log/syslog
```

Namun hasil dari perintah tersebut akan menampilkan hal ini:

![Gambar 1. Hasil membaca file syslog melalui user biasa](<../.gitbook/assets/Debian var\_log\_syslog error permission.png>)

Alasan mengapa syslog tidak dapat dibuka oleh setiap _user_ dalam sistem operasi ini berkaitan dengan **hak akses** dan **hak milik** (akan dibahas pada materi selanjutnya). Untuk dapat melihat syslog, pengguna harus memiliki akses _root_ atau _superuser._ Membaca syslog dengan akses _root_ dapat dilakukan melalui perintah ini:

```
sudo nano /var/log/syslog
```

Hasil dari perintah tersebut dapat dilihat pada gambar dibawah:

![Gambar 2. Membaca log menggunakan akses root ](<../.gitbook/assets/Debian var\_log\_syslog success.png>)

Dapat dilihat pada gambar diatas bahwa log sistem (_syslog_) dapat dilihat ketika menggunakan akses _root._ Sebagai pengingat, ada baiknya apabila pengguna yang memiliki akses _root_ tidak mengubah apapun dalam file _syslog._

Setelah mengetahui cara untuk membaca log sistem, pengguna kini dapat melihat log lain yang tersimpan didalam direktor `/var/log`. Sebagai contoh, pengguna dapat melihat log yang berkaitan dengan _packages_ yang di-install, diperbarui, dan dihapus melalui `dpkg` log.&#x20;

Untuk dapat melihat isi dari log`dpkg`, pengguna dapat mengetikkan perintah ini kedalam terminal:

```
nano /var/log/dpkg.log
```

Pada perintah ini, akses _root_ tidak dibutuhkan untuk melihat log tersebut. Hasil dari perintah tersebut dapat dilihat pada gambar dibawah:

![Gambar 3. melihat log dpkg sebagai user biasa](<../.gitbook/assets/Debian var\_log\_dpkglog.png>)

Dapat dilihat pada gambar diatas, log `dpkg` hanya memiliki akses baca, pengguna tidak dapat melakukan operasi lainnya kecuali dilakukan pergantian hak akses. Apabila pengguna ingin mendapatkan akses lebih untuk file tersebut, maka ia perlu akses _root_ untuk melakukan pergantian tersebut (akan dijelaskan pada materi selanjutnya).
