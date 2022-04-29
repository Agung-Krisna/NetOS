---
description: Mempelajari teknologi virtualisasi dan VMM
---

# Virtualisasi dan VMM

## Virtualisasi

Komputer modern memiliki sumber daya (_resource_) yang cukup untuk menggunakan virtualisasi untuk menciptakan ilusi menggunakan banyak mesin virtual kecil (VM), dimana setiap mesin virtual dapat memiliki alokasi sumber daya serta sistem operasi yang berbeda-beda. Sumber daya yang dapat divirtualisasikan diantaranya: media penyimpanan (_storage media_), perangkat lunak, perangkat keras, jaringan serta berbagai layanan yang dapat dijalankan pada jaringan.

#### VMM

Untuk dapat melakukan virtualisasi, diperlukan sebuah VMM (Virtual Machine Manager) yang berfungsi untuk melakukan abstraksi perangkat keras fisik menjadi perangkat keras maya dari suatu sistem. Hypervisor merupakan sebuah perangkat lunak VMM yang menciptakan dan menjalankan mesin virtual (_Virtual Machine_).&#x20;

![Gambar 1. Ilustrasi VMM diantara Perangkat Keras dan Guest OS](<../.gitbook/assets/Type one hypervisor.png>)
