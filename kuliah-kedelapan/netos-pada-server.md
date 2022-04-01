---
description: Mempelajari keterkaitan operating system pada server
---

# NetOS pada Server

### <mark style="color:blue;">Informasi Penulis</mark>

<mark style="color:blue;">Disusun oleh: I Gusti Ngurah Agung Krisna Adhitya</mark>&#x20;

<mark style="color:blue;">NIM: 2005551072</mark>

<mark style="color:blue;">Mata Kuliah: Network Operating System (NOS)</mark>

<mark style="color:blue;">Dosen Pengampu: I Putu Agus Eka Pratama ST., MT.</mark>

<mark style="color:blue;">Jurusan Teknologi Informasi, Fakultas Teknik, Universitas Udayana</mark>

> Note: Kuliah Ketujuh diisi dengan UTS.

## Peran NetOS pada Server

Pada sistem komputer yang digunakan oleh pengguna reguler, sistem operasi yang digunakan umumnya berupa _client operating system_, yang mana memiliki kapabilitas untuk melakukan aktivitas jaringan yang terbatas -- seperti mengunduh _file,_ berselancar di internet, dll. Walau memberikan pengalaman yang baik bagi pengguna reguler, sistem operasi tersebut tidak layak digunakan pada server.

Server pada umumnya menggunakan sebuah sistem operasi khusus yang diciptakan untuk memaksimalkan efisiensi pada proses penyediaan layanan pada _client_ dalam suatu jaringan, baik internet maupun intranet. Contoh layanan yang diberikan pada server diantaranya Mail, Cloud, DNS, Database, dll.

Sistem operasi yang digunakan pada server bernama **Network Operating System** (NOS). NOS umumnya ini memiliki beberapa prioritas utama, yaitu:&#x20;

* Keamanan
* Kemudahan
* Hemat sumber daya komputasi
* Reliabel dalam jaringan komputer

## Sistem Operasi NetOS pada Server

Terdapat beberapa sistem operasi jaringan (NOS) yang dapat digunakan pada server, diantaranya:&#x20;

* Linux (beserta dengan berbagai distribusinya)
* FreeBSD (beserta dengan berbagai variannya)&#x20;
* Sun Solaris
* UNIX

Linux merupakan pilihan sistem operasi jaringan utama bagi pengelola server karena tingkat kustomisasinya yang tinggi. Setiap sistem operasi linux dapat diatur sesuai dengan keperluan setiap sistem, sehingga sumber daya yang dimiliki dapat dijalankan secara lebih efisien.

Distribusi Linux terbaik sebagai NOS berdasarkan [techradar](https://www.techradar.com/best/best-linux-server-distro) adalah:&#x20;

1.  Ubuntu Server

    Ubuntu Server menjadi pilihan pertama karena memiliki _Long Term Support_ (LTS) yang berarti pengelola server tidak perlu khawatir untuk melakukan pembaruan (_upgrade_) pada sistem operasi ini selama beberapa tahun kedepan. Selain itu, Ubuntu Server dapat menjadi pilihan bagi pengelola server yang ingin membuat platform _cloud_ mereka sendiri.
2.  Debian

    Debian merupakan pilihan yang baik untuk menjadi NOS karena fokus pengembang sistem operasi ini adalah stabilitas. Dengan memberikan stabilitas yang baik, pengelola server dapat memiliki reliabilitas yang tinggi saat menggunakan NOS ini.&#x20;
3.  OpenSUSE

    OpenSUSE merupakan salah satu NOS yang dapat digunakan sebagai NOS karena dukungan yang baik serta dokumentasi yang lengkap. Selain itu, OpenSUSE memiliki dukungan yang baik dari berbagai jenis perangkat keras.
4.  Fedora Server

    Fedora Server adalah sebuah NOS yang baik untuk digunakan sebagai media instalasi server dalam _cloud._ Fedora Server memiliki FreeIPA yang dapat digunakan untuk mengelola berbagai kredensial dalam satu perangkat lunak saja.
5.  Fedora CoreOS

    Fedora CoreOS merupakan sebuah NOS yang digunakan secara khusus untuk menjalankan _container._ Fedora CoreOS juga tersedia dalam bentuk yang dapat diluncurkan secara langsung ke _cloud_. Beberapa layanan _cloud_ yang didukung diantaranya Amazon Web Services (AWS) dan Google Cloud Platform (GCP).
