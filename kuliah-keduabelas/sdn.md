---
description: Mengenali lebih jauh mengenai SDN (Software Defined Networking)
---

# SDN

> Kuliah Kesebelas digantikan menjadi pengumpulan progress tugas besar

### <mark style="color:blue;">Informasi Penulis</mark>

<mark style="color:blue;">Disusun oleh: I Gusti Ngurah Agung Krisna Adhitya</mark>&#x20;

<mark style="color:blue;">NIM: 2005551072</mark>

<mark style="color:blue;">Mata Kuliah: Network Operating System (NOS)</mark>

<mark style="color:blue;">Dosen Pengampu: I Putu Agus Eka Pratama ST., MT.</mark>

<mark style="color:blue;">Jurusan Teknologi Informasi, Fakultas Teknik, Universitas Udayana</mark>

## Software Defined Networking

[Software Defined Network](http://www2.technologyreview.com/news/412194/tr10-software-defined-networking/) (SDN) merupakan sebuah arsitektur jaringan dimana _forwarding state_ dalam _data plane_ dapat diatur dari sebuah _control plane_ yang terpisah. [Menurut Jurnal IEEE](https://www.researchgate.net/profile/Siamak-Azodolmolky/publication/262805723\_Software-Defined\_Networking\_A\_Comprehensive\_Survey/links/0deec539ae007cdb38000000/Software-Defined-Networking-A-Comprehensive-Survey.pdf) SDN dapat didefinisikan secara lebih jauh menjadi empat pilar utama:

* Pemisahan antara _control_ dan _data_ _plane_. Fungsionalitas untuk melakukan kontrol akan dihapuskan dari perangkat jaringan, setiap perangkat jaringan akan hanya menjadi elemen _forwarding_ saja.
* Keputusan untuk melakukan _forwarding_ akan dilakukan secara _flow-based_ dan bukan _destination-based_. Hal ini mampu menyatukan berbagai perilaku dari tipe perangkat jaringan yang berbeda-beda seperti _router_, _switch_, dan _middlebox_. Dengan menggunakan _flow-based forwarding_, perangkat jaringan akan mampu diprogram dengan fleksibilitas yang jauh lebih tinggi.
* Logika kontrol dipindahkan menjadi entitas eksternal, yang dinamakan **SDN Controller** atau **Network Operating System**.
* Jaringan akan mampu diprogram melalui aplikasi yang dijalankan diatas NOS dimana aplikasi tersebut mampu untuk berkomunikasi dengan perangkat jaringan. Karakteristik ini merupakan pembeda utama antara SDN dengan jaringan tradisional.

### Latar Belakang SDN

Jaringan komputer dapat dibagi menjadi tiga _plane_, yaitu _data plane_, _control plane_ dan _management plane_. _Data plane_ berfungsi untuk melakukan penerusan (_forwarding_) data yang diterima. _Control plane_ berfungsi untuk mengatur bagaimana data akan diteruskan, sebagai contoh _routing table_ merupakan bagian dari _control plane_. _Management plane_ berfungsi untuk memonitor serta melakukan konfigurasi pada _control plane_. Dalam jaringan tradisional, _data plane_ dan _control plane_ terdapat pada satu perangkat yang sama, hal tersebut membuat arsitektur jaringan menjadi statis dan kompleks, sehingga tidak banyak hal yang dapat dilakukan untuk memanajemen arsitektur tersebut. Karena kompleksitas tersebut, pengelola kesulitan untuk dapat mengatur jaringan sesuai dengan kebutuhan perusahaan/instansi tertentu.&#x20;

![Gambar 1. Perbedaan diantara jaringan tradisional dan SDN](<../.gitbook/assets/Perbedaan Jaringan Tradisional dan SDN.jpg>)

Dengan menggunakan SDN, pengelola jaringan dapat mengatur perilaku jaringan secara lebih fleksibel karena terpisahnya _control plane_ dan _data plane_ dalam suatu perangkat jaringan. Dengan fleksibilitas tersebut, pengelola jaringan maupun administrator sistem mampu dengan lebih mudah memanajemen serta mengatur jaringan sesuai dengan kebutuhan instansi seperti:

* Maintenance jaringan dan perangkat jaringan tanpa perlu bergantung sepenuhnya pada perangkat keras saja
* Manajemen bandwidth
* Manajemen Quality of Service (QoS)
* Manajemen Keamanan
