---
description: Mempelajari bagaimana cara menciptakan jaringan virtual menggunakan mininet
---

# Praktik Menggunakan Mininet

## Mininet

Mininet merupakan sebuah emulator jaringan yang mampu menciptakan jaringan yang berisikan _host_, _controller_, dan _link virtual_.

* Untuk dapat menggunakan mininet, pengguna harus mengunduh perangkat lunaknya dengan menggunakan perintah: `sudo apt-get install mininet`

![Gambar 1. Mengunduh package mininet](<../.gitbook/assets/Installing Mininet 0.png>)

* Untuk dapat membuat sebuah jaringan melalui mininet, ketikkan perintah ini pada terminal: `sudo mn --mac --topo single,3 --switch ovsk --controller=remote`&#x20;

![Gambar 2. Menciptakan jaringan virtual dengan mininet](<../.gitbook/assets/mininet controller 1.png>)

> flag --mac berfungsi untuk mengatur Media Access Controller secara otomatis flag -- topo berfungsi untuk memilih topologi yang digunakan flag --switch berfungsi untuk memilih OpenvSwitch flag --controller berfungsi untuk memilih host yang digunakan sebagai controller

* Untuk melihat seluruh antarmuka jaringan yang telah diciptakan, ketikkan perintah ini ke terminal: `net`

![Gambar 3. Memperlihatkan seluruh antarmuka jaringan yang telah diciptakan](<../.gitbook/assets/mininet net 2.png>)

* Untuk melihat seluruh informasi dari setiap _node_, ketikkan perintah ini ke terminal: `dump`

![Gambar 4. Memperlihatkan seluruh informasi node yang telah diciptakan](<../.gitbook/assets/Mininet dump 3.png>)
