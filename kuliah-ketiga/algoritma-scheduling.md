---
description: Membahas mengenai algoritma scheduling esensial dalam suatu sistem operasi.
---

# Algoritma Scheduling

## Algoritma Scheduling

Algoritma _scheduling_ dalam dalam sistem operasi memiliki jenis yang beragam, sesuai dengan kebutuhan sistem yang menggunakannya.&#x20;

Fokus utama pada tulisan kali ini adalah beberapa jenis algoritma _scheduling_ yang menjadi algoritma fundamental dan seringkali digunakan dalam berbagai sistem operasi seperti Windows, Linux, Mac, dan Android.

## Jenis Algoritma Scheduling

Algoritma _scheduling_ memiliki kemampuan untuk membantu pemrogram dalam mengembangkan aplikasi yang memiliki keterkaitan dengan sistem operasi tertentu. Algoritma yang akan dibahas saat ini diantaranya:

1. Round Robin (RR)
2. First In First Out (FIFO)
3. Shortest Job First (SJF)

### Round Robin (RR)

Round Robin (RR) merupakan sebuah algoritma _scheduling_ yang menggunakan konsep _queue_ (antrian).&#x20;

Dalam algoritma ini, setiap proses memiliki time quantum untuk menandai waktu berjalannya proses.

> Ketika time quantum selesai, maka proses yang sedang dieksekusi juga selesai.&#x20;

Setiap proses memiliki nilai time quantum yang sama, yaitu 1/N.

> N menandakan jumlah proses yang menunggu untuk dieksekusi

Untuk mendapatkan hasil yang optimal, ada baiknya apabila time quantum bernilai cukup besar untuk memastikan bahwa proses dapat diselesaikan dalam 1 quantum.&#x20;

> Apabila time quantum terlalu kecil, maka algoritma ini tidak mampu untuk menyelesaikan proses yang dieksekusi
>
> Sebaliknya, apabila time quantum terlalu besar, maka algoritma ini akan menjadi First Come First Serve (FCFS).

### First In First Out (FIFO)

Algoritma ini memprioritaskan proses yang datang terlebih dahulu dan memastikan bahwa proses tersebut telah dieksekusi secara sempurna.&#x20;

Apabila terdapat proses baru yang datang sedangkan proses lama sedang dieksekusi, maka proses baru tersebut harus menunggu dalam antrian hingga proses lama telah selesai dieksekusi.

Algoritma ini memiliki suatu kekurangan, yaitu apabila terdapat proses yang memiliki waktu eksekusi yang berbeda (panjang dan pendek), maka proses yang memiliki waktu eksekusi pendek akan dirugikan. Solusi dari kekurangan ini adalah untuk menggunakan SJF (Shortest Job First).

### Shortest Job First (SJF)

Algoritma ini bertujuan untuk memperbaiki kekurangan yang dimiliki oleh algoritma FIFO. Cara kerja algoritma ini adalah dengan menghitung waktu eksekusi proses terlebih dahulu, lalu mengeksekusi proses yang memiliki waktu eksekusi yang paling rendah.&#x20;
