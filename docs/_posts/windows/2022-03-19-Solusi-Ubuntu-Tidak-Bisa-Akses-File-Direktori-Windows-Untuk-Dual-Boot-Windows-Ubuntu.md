---
layout: post
title: "Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu"
judulseo: "Solusi Tidak Bisa Akses File Direktori Dual Boot Windows Ubuntu"
deskripsi: "Tidak Bisa Akses Direktori Dual Boot Windows Ubuntu, os ubuntu tidak bisa akses file dan direktori windows, perbaiki lewat control panel"
excerpt: "Mempunyai komputer yang bisa dual boot windows dan ubuntu, ternyata, memiliki satu kekurangan yang harus diperbaiki. Salah satu kekurangan yang biasa ditemui adalah tidak bisa akses file atau direktori windows ketika menggunakan OS ubuntu"
katakunci: "Solusi Tidak Bisa Akses Direktori Dual Boot Windows Ubuntu"
slug: "ubuntu-tidak-bisa-akses-direktori-windows"
date: 2022-03-19 01:00:00
tanggalpostterbit: 2022-03-19
tanggalpostmodif: 2022-03-19
categories: windows
tags: [ "dual-boot-windows-ubuntu" , "dual-boot" ]
penulis: achmad
changefreq: monthly
priority: "0.8"
banner: ubuntu-tidak-bisa-akses-direktori-windows.jpg

---

{% include toc.html %}

<p>Mempunyai komputer yang bisa <a href="/dual-boot-windows-10-ubuntu">dual boot windows dan ubuntu</a>, ternyata, memiliki satu kekurangan yang harus diperbaiki. Salah satu kekurangan yang biasa ditemui adalah tidak bisa akses file atau direktori windows ketika menggunakan OS ubuntu.</p>

<p>Berikut ini gambar error yang biasa ditemui :</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/dual-boot-windows-ubuntu/ubuntu-tidak-bisa-akses-windows-1.jpg" alt="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" title="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" {% include classlazy.html %} {% include classimage.html %} ></p>


## Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu

<p>Agar os ubuntu bisa akses file dan direktori windows, berikut ini solusinya :</p>

<p>1. Buka Control Panel.</p>

Klik icon pencarian yang ada di kiri bawah sebelah icon windows. Ketika "control panel". Ketika aplikasi "control panel" muncul, klik aplikasi tersebut.

<p>2. Buka Hardware And Sound</p>

<p>3. Buka Power Options</p>

<p>4. Buka Choose what power options does</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/dual-boot-windows-ubuntu/ubuntu-tidak-bisa-akses-windows-2.jpg" alt="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" title="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>5. Klik change setting that currently unavailable</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/dual-boot-windows-ubuntu/ubuntu-tidak-bisa-akses-windows-3.jpg" alt="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" title="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>6. Hilangkan centang di bagian Turn on fast startup (recommended)</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/dual-boot-windows-ubuntu/ubuntu-tidak-bisa-akses-windows-4.jpg" alt="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" title="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" {% include classlazy.html %} {% include classimage.html %} ></p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/dual-boot-windows-ubuntu/ubuntu-tidak-bisa-akses-windows-5.jpg" alt="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" title="Solusi Ubuntu Tidak Bisa Akses File Direktori Windows Untuk Dual Boot Windows Ubuntu" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>7. Save changes</p>

<p>Selanjutnya klik restart dan pilih menu os ubuntu serta nikmati akses lancar ke file-file windows. Akses file dan direktori windows dapat melalui file explorer layaknya di windows atau melalui terminal ubuntu.</p>

<p>Hal seperti ini biasa ditemui jika dual boot windows ubuntu, dual boot windows linux mint dan dual boot windows debian dan turunannya. Kami pernah melakukan dual boot windows linux opensuse dan masalah seperti ini tidak ditemukan.</p>


## Kekurangan

<p>Dengan menonaktifkan fitur "turn on fast startup" dapat mengakibatkan lambatnya saat komputer windows pertama kali dihidupkan atau direstart. Salah satu solusinya agar tetap terasa lebih cepat adalah dengan menggunakan hard disk SSD. Selain start up menjadi lebih cepat, akses file dan direktori windows dari OS ubuntu juga terasa lebih cepat.</p>


## Fitur Fast Startup

<p>Fast startup merupakan fitur terbaru untuk windows 8 dan windows 10 yang secara default akan memiliki posisi "on". Dalam posisi "on", ketika windows 8 dan windows 10 di-shutdown, sebenarnya windows tidak benar-benar shutdown, tetapi windows akan berada dalam kondisi "hybrid shutdown". Dalam kondisi ini, semua informasi tentang aktifitas windows yang terakhir sebelum di-shutdown, akan disimpan di dalam hard disk. Sehingga ketika windows dihidupkan lagi, semua aktifitas terakhir sebelum windows di-shutdown akan tertampil kembali persis sama. Hal inilah yang mengakibatkan windows dapat booting lebih cepat ketika dihidupkan kembali. Oleh karena itu, jika pengguna komputer windows menginginkan supaya komputernya shut down secara total, maka fitur ini harus di-off-kan, sehingga mounting partisi windows dapat berjalan dengan benar. Jika windows tidak benar-benar shutdown (fast startup "on"), maka proses mounting partisi windows tidak terjadi secara benar. Hal inilah yang mengakibatkan pengguna ubuntu tidak bisa akses partisi windows.</p>

<p>Oleh karena itu, sebaiknya semua aplikasi, file, direktori dan lain sebagainya harus ditutup secara total saat komputer akan di-shutdown. Hal ini dengan mudah dilakukan jika fitur fast startup "off". Tetapi komputer akan menjadi lebih lambat dalam booting.</p>

<p>Ubuntu tidak bisa akses file dan direktori windows dalam posisi masih hibernated, karena melindungi partisi windows. Karena jika ubuntu dapat mengakses file dan direktori dalam kondisi hibernated, partisi windows bisa mengalami crash ketika menggunakan os windows lagi, dan akibat terburuknya adalah windows akan rusak.</p>


## Note :

<p>Jika dengan cara di atas, ubuntu tetap tidak bisa akses file direktori windows, kemungkinan besar sobat harus melakukan turn off proses hibernation secara total. Untuk itu, bukalah aplikasi cmd dengan hak akses "Run As Administrator". Kemudian ketik perintah berikut :</p>

<div style="border: solid 1px blue;
    font-size: 1.3 em; 
    color: blue; 
    margin: 10px; 
    padding:10px; 
    background: #FFFFB3;">
powercfg /h off</div>

<p>Semoga dengan solusi yang disebutkan di artikel ini, para pengguna dual boot windows dan ubuntu, dapat melakukan akses ke file dan direktori windows dengan lancar ketika menggunakan OS ubuntu.</p>