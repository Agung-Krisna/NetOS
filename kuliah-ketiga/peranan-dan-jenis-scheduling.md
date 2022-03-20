---
description: Memahami lebih lanjut mengenai berbagai peran serta jenis-jenis scheduling
---

# Peranan dan Jenis Scheduling

## Peran Scheduling

_Scheduling_ memiliki peranan penting dalam sistem operasi, beberapa peran tersebut diantaranya:

1. Memaksimalkan _throughput._
2. Memaksimalkan kinerja dan waktu prosesor.
3. Efisiensi proses.
4. Memberikan keadilan (_fairness_) kepada setiap _job_ dan aplikasi.
5. Meminimalkan waktu tanggap (_time respond_)
6. Mengoptimalkan sumber daya (_resource_).

## Jenis Scheduling

Terdapat empat jenis _scheduling_, yaitu:&#x20;

1. Long Term Scheduling
2. Medium Term Scheduling
3. Short Term Scheduling
4. I/O Scheduling

### Long Term Scheduling

Long Term Scheduling merupakan jenis penjadwalan yang menambahkan _pool_ untuk proses yang akan dieksekusi.&#x20;

Long Term Scheduling juga disebut sebagai _job scheduler_ karena tujuan utama dari jenis penjadwalan ini adalah mengatur jadwal eksekusi job, baik secara CPU time maupun I/O time.

### Medium Term Scheduling

Medium Term Scheduling merupakan jenis penjadwalan yang menambahkan jumlah dari process baik secara penuh maupun parsial di dalam memori utama.

Medium Term Scheduling juga disebut sebagai _Swapping Scheduler_ karena memiliki tujuan utama untuk mengeluarkan proses yang _suspended_ dan menggantikannya dengan proses selanjutnya.

> Proses dapat menjadi _suspended_ apabila proses tersebut meminta akses I/O.

### Short Term Scheduling

Short Term Scheduling merupakan jenis penjadwalan yang melakukan pemilihan proses yang akan dieksekusi terlebih dahulu oleh prosesor dalam jangka waktu yang singkat.

Short Term Scheduling juga disebut sebagai _CPU Scheduler_ karena tugasnya untuk mengalokasikan waktu CPU kepada salah satu proses yang menunggu untuk dieksekusi.

### I/O Scheduling

I/O Scheduling merupakan jenis penjadwalan yang melakukan pemilihan proses yang sedang dalam kondisi _suspended_ untuk dapat dilanjutkan kembali berdasarkan ketersediaan perangkat I/O.
