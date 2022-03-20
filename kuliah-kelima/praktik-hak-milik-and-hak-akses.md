---
description: Mempraktikkan pengetahuan yang telah dipelajari mengenai hak milik & hak akses
---

# Praktik Hak Milik & Hak Akses

Dalam praktik ini, proses pengaturan hak milik dan hak akses akan dimulai dari pembuatan _file_ yang menjadi objek dalam studi kasus ini. Untuk dapat membuat sebuah _file_ baru yang bertipe .txt melalui terminal linux, pengguna dapat mengetikkan perintah:&#x20;

```
touch not_a_secret.txt
```

Untuk mengetahui hak akses pada _file_ tersebut, pengguna dapat mengetikkan perintah ini pada terminal:

```
ls -lah not_a_secret.txt
```

Perintah tersebut akan menghasilkan keluaran seperti ini:

![Gambar 1. Informasi file "not\_a\_secret.txt"](<../.gitbook/assets/ls -lah result.png>)

Terlihat bahwa file tersebut memiliki hak akses `rw` bagi pemilik _file_, `r` bagi pengguna _group_, dan `r` bagi pengguna lainnya. Hak milik dari _file_ tersebut dimiliki oleh pengguna "buster". Apabila pengguna ingin memberikan _file_ tersebut hak akses tertinggi, perintah ini dapat digunakan untuk melakukan hal tersebut:

```
chmod 777 not_a_secret.txt
```

Setelah menjalankan perintah diatas, hak akses pada _file_ "not\_a\_secret.txt" akan terlihat seperti gambar dibawah ini:

![Gambar 2. Informasi file setelah pengaturan hak akses](<../.gitbook/assets/ls -lah after chmod.png>)

Gambar diatas menunjukkan bahwa hak akses pada _file_ tersebut telah berubah menjadi `rwxrwxrwx` yang berarti setiap pengguna yang berada dalam sistem operasi tersebut dapat membaca, menulis, serta mengeksekusi _file_ "not\_a_\__secret.txt". Untuk mengubah kepemilikan _file_ dari pengguna biasa menjadi pengguna _root_, pengguna dapat menggunakan perintah ini:

```
sudo chown root not_a_secret.txt
```

Hasil dari perintah tersebut dapat dilihat pada gambar dibawah:

![Gambar 3.Hasil pemindahan hak milik](<../.gitbook/assets/chown to root.png>)

Gambar diatas menunjukkan bahwa _file_ "not\_a_\__secret.txt" telah berhasil dirubah kepemilikannya dari yang sebelumnya dimiliki oleh pengguna "buster" menjadi pengguna _root._&#x20;
