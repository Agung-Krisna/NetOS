---
description: Mempelajari lebih lanjut mengenai scheduling yang telah dibahas sebelumnya
---

# Scheduling Lanjutan

### <mark style="color:blue;">Informasi Penulis</mark>

<mark style="color:blue;">Disusun oleh: I Gusti Ngurah Agung Krisna Adhitya</mark>&#x20;

<mark style="color:blue;">NIM: 2005551072</mark>

<mark style="color:blue;">Mata Kuliah: Network Operating System (NOS)</mark>

<mark style="color:blue;">Dosen Pengampu: I Putu Agus Eka Pratama ST., MT.</mark>

<mark style="color:blue;">Jurusan Teknologi Informasi, Fakultas Teknik, Universitas Udayana</mark>

## Algoritma Scheduling Lanjutan

Pada pembahasan sebelumnya telah dijelaskan beberapa algoritma _scheduling_ yang paling umum untuk diterapkan pada sistem operasi modern. Pembahasan kali ini akan berfokus pada algoritma _scheduling_ lanjutan, yaitu Shortest Process Next (SPN), Feedback, Shortest Remaining Time (SRT), dan Highest Response Ratio Next (HRRN).

## Shortest Process Next (SPN)

Shortest Process Next (SPN) merupakan sebuah algoritma _scheduling_ yang bekerja dengan cara melakukan pengecekan waktu pemrosesan (_processing time_) dari setiap _job_. _Job_ yang memiliki waktu proses terpendek akan didahulukan dengan cara dimasukkan ke dalam urutan antrian terdepan, sedangkan _job_ dengan waktu proses terpanjang akan dimasukkan ke dalam urutan antrian terbelakang.&#x20;

Algoritma ini bekerja dengan baik untuk mengurangi waktu tunggu dari setiap proses, namun kekurangannya adalah terdapat kemungkinan beberapa proses dengan waktu proses yang panjang akan mengalami _starvation_ karena tidak mendapatkan giliran untuk dieksekusi.&#x20;

## Feedback

Feedback _scheduling_ merupakan algoritma yang menempatkan _job_ dalam suatu antrian dengan urutan prioritas yang bervariasi. Dengan menggunakan strategi ini, sumber daya dapat dialokasikan secara lebih efektif karena tidak ada yang terbuang untuk mengawasi waktu eksekusi setiap _job_.

Fokus dari feedback _scheduling_ adalah memindahkan proses dari suatu antrian ke antrian lainnya berdasarkan prioritas antrian tersebut. Jika sebuah proses menghabiskan terlalu banyak waktu CPU, maka proses tersebut akan dikeluarkan (_release_) menuju antrian dengan prioritas yang lebih rendah. Hal ini berlaku juga sebaliknya, apabila terdapat proses dari antrian prioritas rendah yang tidak kunjung mendapatkan waktu eksekusi, proses tersebut dapat dipindahkan ke antrian dengan prioritas tinggi.

> Metode memindahkan suatu proses dari satu antrian ke antrian lainnya merupakan penerapan dari konsep "_aging_"

Dengan menggunakan __ algoritma ini, _starvation_ dapat dikurangi karena diterapkannya konsep "_aging_". _Aging_ memastikan bahwa tidak ada proses yang dapat secara terus menerus memonopoli waktu eksekusi CPU.

## Highest Response Ratio Next (HRRN)

Highest Response Ratio Next merupakan algoritma _scheduling_ yang bekerja dengan cara memilih _job_ yang memiliki waktu respon (_Response Time_) terendah. Waktu respon dikalkulasikan pada setiap job yang sedang menunggu untuk dieksekusi. Rumus untuk menghitung waktu respon adalah:

$$
R = (w+s)/s
$$

Dimana:

* R = Waktu Respon
* w = waktu tunggu
* s = waktu _service_

## Shortest Remaining Time

Shortest Remaining Time merupakan sebuah algoritma yang bekerja dengan cara mengeksekusi _job_ dengan waktu tunggu lebih pendek.&#x20;

_Job_ yang sedang dieksekusi dapat digantikan dengan _job_ baru yang memiliki waktu eksekusi lebih singkat.&#x20;
