---
description: >-
  Mempelajari lebih lanjut mengenai kernel yang pernah disinggung pada materi
  sebelumnya
---

# Kernel dalam OS

### <mark style="color:blue;">Informasi Penulis</mark>

<mark style="color:blue;">Disusun oleh: I Gusti Ngurah Agung Krisna Adhitya</mark>&#x20;

<mark style="color:blue;">NIM: 2005551072</mark>

<mark style="color:blue;">Mata Kuliah: Network Operating System (NOS)</mark>

<mark style="color:blue;">Dosen Pengampu: I Putu Agus Eka Pratama ST., MT.</mark>

<mark style="color:blue;">Jurusan Teknologi Informasi, Fakultas Teknik, Universitas Udayana</mark>

## Kernel

Kernel merupakan inti dari suatu sistem operasi. Kernel memuat utilitas, fungsi-fungsi dasar perangkat keras, dan kemampuan utama sebuah sistem operasi. Kernel berada di seluruh sistem operasi, baik itu Linux, Android, Windows, FreeBSD, dll.&#x20;

> Apabila dianalogikan sebagai makhluk hidup, kernel akan menjadi "jiwa" dari tubuh pemiliknya.
>
> Jika makhluk hidup hanya memiliki tubuh tanpa jiwa, maka ia takkan dapat hidup.
>
> Serupa dengan sebuah sistem, apabila hanya memiliki perangkat keras tanpa sistem operasi dan kernel, maka sistem tersebut tidak akan berjalan.&#x20;

### Struktur Kernel

Kernel terdiri dari beberapa _layer_, diantaranya:&#x20;

1. _Layer_ yang bertindak sebagai antarmuka (_interface_) dengan perangkat keras, seperti CPU, RAM, dan PCIe _controller._
2. _Layer_ yang mengatur manajemen memori (_memory management_), yang berfungsi untuk mengalokasikan RAM serta virtual memori (Swap).
3. _Layer_ selanjutnya bertindak sebagai _scheduler,_ yang mengatur urutan proses yang akan dieksekusi dan memastikan bahwa multitasking dapat dilaksanakan.
4. _Layer_ yang mengatur _device_ yang terhubung pada sistem.
5. &#x20;_Layer_ terakhir berfungsi untuk mengatur _file_ system.&#x20;

### Utilitas Kernel

Utilitas merupakan program yang berfungsi untuk mengerjakan sebuah tugas spesifik. Kernel memiliki beberapa utilitas penting yang berfungsi untuk mengetahui informasi mengenai perangkat keras, perangkat lunak, partisi penyimpanan, dll.
