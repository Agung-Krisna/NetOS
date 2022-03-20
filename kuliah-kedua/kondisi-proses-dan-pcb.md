---
description: >-
  Mempelajari mengenai kondisi proses (Process States) beserta dengan struktur
  data PCB (Process Control Block)
---

# Kondisi Proses dan PCB

## Kondisi Proses

Proses dalam suatu sistem operasi dapat terbagi dalam beberapa kondisi, diantaranya:&#x20;

* New -> Proses sedang diciptakan.
* Ready -> Proses sedang menunggu untuk ditugaskan pada sebuah prosesor.
* Waiting -> Proses sedang menunggu untuk suatu kejadian terjadi (seperti penyelesaian I/O).
* Running -> Instruksi sedang dijalankan.
* Terminated -> Proses setelah selesai dieksekusi.

Suatu proses akan berubah dari kondisi awal yang statis menjadi aktif melalui kondisi proses (process states). Setiap proses pasti memiliki masing-masing satu kondisi proses.

## PCB

Process Control Block (PCB) merupakan sebuah struktur data yang memuat informasi spesifik mengenai setiap proses. Terdapat berbagai jenis informasi yang harus disimpan kedalam PCB. Informasi yang telah tersimpan didalam PCB membuat sebuah proses mampu mengubah kondisi proses. Ketika sebuah proses telah mengubah kondisi prosesnya, maka sistem operasi harus memperbarui informasi tersebut kedalam PCB dari proses yang bersangkutan.

### Informasi yang tersimpan dalam PCB

Terdapat beberapa jenis informasi yang tersimpan didalam PCB, diantaranya:

{% tabs %}
{% tab title="Keadaan Proses" %}
Keadaan (state) dari suatu proses yang dapat dibagi menjadi lima bagian, yaitu:

1. New
2. Ready
3. Waiting
4. Running
5. Terminated
{% endtab %}

{% tab title="Program Counter" %}
Program Counter merupakan sebuah _counter_ yang menyimpan lokasi dari instruksi yang harus dieksekusi oleh proses yang bersangkutan.
{% endtab %}

{% tab title="CPU Register" %}
Register memiliki berbagai jenis serta jumlah yang bergantung pada arsitektur CPU yang berada di suatu komputer.

Register terdiri dari accumulator, index register, stack pointer, general-purpose register, dan code information program counter.

Register mampu menyimpan keadaan dari suatu proses ketika terjadi suatu gangguan, hal ini memungkinkan proses untuk berjalan dengan benar.
{% endtab %}

{% tab title="Informasi Manajemen Memori" %}
Informasi yang tersimpan dalam memori dapat berupa _page tables_, nilai dari dasar dan batas register, serta _segment tables_.
{% endtab %}

{% tab title="Informasi Pencatatan" %}
Informasi pencatatan (Scheduling Information) merupakan informasi yang meliputi jumlah dari CPU, jumlah akun, batas waktu, jumlah job maupun proses.
{% endtab %}

{% tab title="Informasi Status I/O" %}
Informasi mengenai perangkat I/O yang digunakan pada proses, serta berkas-berkas yang sedang dibuka.
{% endtab %}
{% endtabs %}
