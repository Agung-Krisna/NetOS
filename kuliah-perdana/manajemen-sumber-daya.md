---
description: Mempelajari mengenai manajemen sumber daya yang dilakukan oleh OS
---

# Manajemen Sumber Daya

Dalam menjalankan sebuah program, komputer memiliki banyak sumber daya yang dapat digunakan. Sumber daya terdiri dari perangkat lunak dan perangkat keras. Untuk dapat mengalokasikan sumber daya secara efektif, sebuah komputer memerlukan _operating system_ yang dapat mengatur jumlah sumber daya yang diperlukan untuk menjalankan suatu program.  Sifat dari _operating system_ ini disebut sebagai **resource allocator** (telah dibahas pada bagian pengantar dari kuliah perdana).&#x20;

![Gambar 1. Sistem Komputer beserta Alokasi Sumber Daya OS](<../.gitbook/assets/Manajemen Resource.png>)

Ketika terdapat berbagai program untuk dieksekusi serta data untuk disimpan pada waktu yang bersamaan, maka _Operating System_ memiliki tugas untuk memastikan bahwa sumber daya dapat dialokasikan secara tepat untuk masing-masing program yang membutuhkan. _Operating System_ akan menangani berbagai instruksi secara langsung ke _processor._&#x20;

Pada ilustrasi diatas, terlihat bahwa _Operating System_ memiliki peranan untuk memastikan bagaimana cara penggunaan CPU agar mendapatkan performa yang efisien. Hal tersebut dapat dilakukan melalui sistem penjadwalan (_**scheduling**_) yang memperhatikan kecepatan (_clock_) dari CPU dan tugas yang harus diselesaikan.&#x20;

Selain itu, _Operating System_ juga berperan untuk memberikan akses untuk perangkat _input-output_ (I/O) kepada aplikasi yang membutuhkannya. Apabila terdapat sebuah aplikasi yang membutuhkan akses menulis dan membaca _file_ pada komputer, maka _Operating System_ juga bertugas untuk mengakses media penyimpanan yang terletak dalam komputer dan menampilkan informasi yang terletak pada _file_ tersebut.&#x20;
