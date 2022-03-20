---
description: Mempelajari mengenai penjadwalan (scheduling) dalam sistem operasi
---

# Pengenalan Scheduling

### <mark style="color:blue;">Informasi Penulis</mark>

<mark style="color:blue;">Disusun oleh: I Gusti Ngurah Agung Krisna Adhitya</mark>&#x20;

<mark style="color:blue;">NIM: 2005551072</mark>

<mark style="color:blue;">Mata Kuliah: Network Operating System (NOS)</mark>

<mark style="color:blue;">Dosen Pengampu: I Putu Agus Eka Pratama</mark>

<mark style="color:blue;">Jurusan Teknologi Informasi, Fakultas Teknik, Universitas Udayana</mark>

## Definisi Scheduling

_Scheduling_ (penjadwalan) merupakan sebuah aktivitas yang dilakukan berdasarkan satu atau berbagai jumlah aturan, mekanisme, serta prosedur didalam sistem operasi terkait dengan urutan kerja yang dilakukan oleh komputer dan sistem komputer.

_Scheduling_ dalam sistem operasi memiliki peran penting untuk memastikan bahwa setiap proses yang berjalan dapat dialokasikan sumber daya secara optimal. Perannya yang vital bagi semua komputer membuat _scheduling_ menjadi hal yang pasti terdapat dalam setiap sistem operasi modern.

## Alasan Scheduling diperlukan dalam Sistem Operasi

Dalam sistem operasi modern, _scheduling_ memiliki beberapa alasan penting dalam penciptaannya, diantaranya:

1. Meningkatkan efisiensi waktu.&#x20;
   * Sebuah proses pada umumnya memerlukan waktu I/O dan CPU. Tanpa adanya _scheduling_, pengguna harus menunggu alokasi waktu I/O untuk diselesaikan terlebih dahulu sebelum memulai kegiatan _processing_ oleh CPU. Sehingga, banyak waktu yang terbuang oleh ketidakefisiensian tersebut. Dengan menggunakan _scheduling,_ satu proses dapat menggunakan alokasi waktu I/O sembari menunggu alokasi waktu CPU.&#x20;
2. Untuk meminimalisir kemungkinan terjadinya kegagalan dalam mengeksekusi suatu proses.
   * Kegagalan dalam melakukan eksekusi suatu proses dapat dengan mudah terjadi ketika terdapat berbagai proses yang berjalan dalam satu waktu. _Scheduling_ mampu memastikan setiap proses tidak mengalami _starvation_ dengan cara memberikan sumber daya yang cukup, sesuai dengan urutan mereka.&#x20;
3. Untuk mendukung "_multiprogramming_" dalam sistem operasi.
   * _Multiprogramming_ merupakan suatu kemampuan yang dimiliki oleh sistem operasi untuk menjalankan lebih dari satu program dalam satu waktu.&#x20;
