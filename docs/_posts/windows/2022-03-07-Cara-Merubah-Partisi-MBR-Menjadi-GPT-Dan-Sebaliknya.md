---
layout: post
title: "Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"
judulseo: "Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"
deskripsi: "Cara merubah partisi mbr menjadi gpt atau sebaliknya, menggunakan command line windows atau aplikasi yang mendukung"
excerpt: "Partisi GPT menjadi standar baru dalam hal partisi hard disk karena memiliki beberapa keunggulan daripada MBR. Bagi orang yang pertama kali menggunakan komputer, alangkah baiknya mengenal terlebih dahulu"
katakunci: "Cara Merubah Partisi MBR Menjadi GPT"
slug: "cara-merubah-partisi-mbr-menjadi-gpt"
date: 2022-03-07 01:00:00
tanggalpostterbit: 2022-03-07
tanggalpostmodif: 2022-03-07
categories: windows
tags: ["partisi-mbr" , "partisi-gpt"]
penulis: achmad
changefreq: monthly
priority: "0.8"
banner: mbr-ke-gpt.jpg

---

{% include toc.html %}

<p>Partisi GPT menjadi standar baru dalam hal partisi hard disk karena memiliki beberapa keunggulan daripada MBR. Bagi orang yang pertama kali menggunakan komputer, alangkah baiknya mengenal terlebih dahulu <a href="/partisi-harddisk-windows">jenis-jenis partisi hard disk</a>.</p>

<p>Selanjutnya setelah mengetahui keunggulan GPT daripada MBR, banyak sobat yang ingin menjajal hard disk dengan partisi GPT. Untuk memilih partisi GPT tentu harus memperhatikan syarat dan ketentuan yang harus dipenuhi seperti tersebut di dalam artikel <a href="/perbedaan-partisi-mbr-dan-gpt">beda partisi MBR dan GPT</a>.</p>

<p>Sebelum merubah jenis partisi hard disk, apakah merubah partisi MBR ke GPT, atau sebaliknya, hal terpenting yang harus dilakukan adalah melakukan backup semua file-file penting di hard disk eksternal.</p>

## Cara Mengubah Partisi MBR ke GPT

<h4>Cara Pertama Menggunakan Command Line</h4>

<p>1.a. Buka perintah cmd bagi pengguna windows. Ketik cmd di dalam kolom pencarian windows dan ketik enter pada aplikasi command line.</p>

<p>1.b. Ketik perintah diskpart.</p>

<p>1.c. Ketik perintah list disk</p>

<p>1.d. Ketik perintah list volume</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/mbr-menjadi-gpt/cara-ubah-mbr-ke-gpt-1.jpg" alt="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya" title="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>1.e. Ketik perintah select volume untuk menentukan volume yang mana yang akan kita ubah ke GPT. Misalnya volume 0.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/mbr-menjadi-gpt/cara-ubah-mbr-ke-gpt-2.jpg" alt="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya" title="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>1.f. Ketik clean untuk menghapus semua isinya. Ingat bahwa dengan melakukan perintah clean, semua data akan dihapus dan kemungkinan kecil dapat dikembalikan lagi. Untuk itu, backup terlebih dahulu semua datanya.</p>

<p>1.g. Ketik convert gpt untuk mengubah volume/hard disk menjadi gpt.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/mbr-menjadi-gpt/cara-ubah-mbr-ke-gpt-3.jpg" alt="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya" title="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"  {% include classlazy.html %} {% include classimage.html %} ></p>

<h4>Catatan Penting :</h4>

<p>1. Cara ini dilakukan untuk mengubah volume yang merupakan bagian dari hard disk.</p>

<p>2. Kita tidak bisa mengubah partisi hard disk menjadi GPT secara keseluruhan jika hard disk tersebut sedang digunakan yang berisi file-file windows(Jumlah hard disk cuman 1. Jika hard disk yang digunakan berjumlah dua, maka hard disk yang bisa diubah menjadi GPT adalah hard disk ke-2. Berikut ini langkah-langkahnya :</p>

<p>2.a. Setelah masuk ke perintah disk part, ketik perintah list disk untuk melihat jumlah hard disk yang digunakan.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/mbr-menjadi-gpt/cara-ubah-mbr-ke-gpt-4.jpg" alt="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya" title="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>2.b. Select disk 1</p>

<p>2.c. Clean, untuk menghapus seluruh isi hard disk</p>

<p>2.d. Convert GPT.</p>

<p>3. Jika hard disk yang digunakan cuman satu, maka untuk mengubah partisi hard disk secara keseluruhan menjadi GPT, harus menggunakan langkah berikut :</p>

<p>3.a. Backup seluruh file-file penting, karena semua file akan terhapus secara keseluruhan.</p>

<p>3.b. Masukkan file installer windows, bisa menggunakan flashdisk atau DVD.</p>

<p>3.c. Lakukan proses <a href="/cara-install-windows-10">install windows</a> seperti biasa dan berhenti sejenak sebelum langkah proses instalasi.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/mbr-menjadi-gpt/cara-ubah-mbr-ke-gpt-5.jpg" alt="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya" title="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>3.d. Pencet tombol shift + F10 secara bersamaan.</p>

<p>3.e. Ketik perintah diskpart</p>

<p>3.f. Ketik perintah list disk</p>

<p>3.g. Ketik perintah select disk 0.</p>

<p>3.h. Ketik perintah clean untuk menghapus semua data.</p>

<p>3.i. Ketik perintah convert to gpt, untuk mengubah partisi menjadi GPT.</p>

<h4>Cara Kedua Menggunakan Aplikasi</h4>

<p>Aplikasi yang digunakan adalah minitool partition. Download aplikasi mini partition tool di web resminya yaitu www.partitionwizard.com, pilih versi gratisnya.</p>

<p>1.a. Buka aplikasi minitool partition</p>

<p>1.b. Pilih menu "Convert MBR Disk to GPT Disk" untuk mengubah MBR menjadi GPT.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/mbr-menjadi-gpt/cara-ubah-mbr-ke-gpt-6.jpg" alt="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya" title="Cara Merubah Partisi MBR Menjadi GPT Dan Sebaliknya"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Menggunakan aplikasi ini belum pernah kami lakukan. Secara teori, hal ini bisa dilakukan. Akan tetapi, bisa saja setelah mengubah jenis partisi dari MBR ke GPT atau sebaliknya, komputer menjadi hang atau tidak bisa digunakan. Sehingga harus diinstal ulang. Oleh karena itu, backup terlebih dahulu semua file-file penting.</p>

<p>Kedua metode dalam tutorial mengubah partisi MBR menjadi GPT, dapat digunakan untuk mengubah partisi GPT menjadi MBR. Untuk cara pertama pada langkah "Convert GPT" diubah menjadi "Convert MBR". Untuk cara kedua pilih menu "Convert GPT Disk to MBR Disk".</p>