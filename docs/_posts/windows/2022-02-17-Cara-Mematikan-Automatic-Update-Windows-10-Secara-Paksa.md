---
layout: post
title: "Cara Mematikan Automatic Update Windows 10 Secara Paksa"
judulseo: "Cara Mematikan Automatic Update Windows 10 Secara Paksa"
deskripsi: "Cara Mematikan Automatic Update Windows 10 secara paksa, bisa menggunakan commandline atau dengan GUI, cara agar kuota tidak cepat habis"
excerpt: "Pada versi Windows 10 pro dan versi yang lebih tinggi, pengguna dapat mematikan automatic update windows secara paksa"
katakunci: "Cara Mematikan Automatic Update Windows 10"
slug: "cara-mematikan-automatic-update-windows-10"
date: 2022-02-17 01:00:00
tanggalpostterbit: 2022-02-17 
tanggalpostmodif: 2022-02-17
categories: windows
tags: ["stop-windows-update" , "windows-update"]
penulis: achmad
changefreq: monthly
priority: "0.8"
banner: mematikan-windows-update.jpg

---

{% include toc.html %}

<p>Pada versi Windows 10 pro dan versi yang lebih tinggi, pengguna dapat mematikan automatic update windows secara paksa.</p>

<p>Pada sebagian pengguna tentunya ini menguntungkan, yaitu pemilik kuota internet yang pas-pasan. Bagi pemilik kuota internet yang berlimpah, misalnya berlangganan internet broadband kabel, tentu hal ini tidak menjadi kendala.</p>

<p>Namun sayang, mematikan update secara paksa ini tidak dapat diterapkan pada windows 10 home edition.</p>


## Cara Mematikan Automatic Update Windows 10

<p>Untuk mematikan fitur windows update dapat dilakukan dengan cara-cara berikut :</p>

<h3 class="{% include classh3.html %}">1. Cara Pertama</h3>

<p>Buka command prompt windows. Untuk membuka command prompt dapat dilakukan dengan cara berikut :</p>

<p>1.a. Tekan tombol windows</p>

<p>1.b. Pada kolom pencarian tuliskan cmd, maka akan muncul command prompt. Silakan klik command prompt untuk mengaksesnya.</p>

<p>Langkah berikutnya adalah mengakses local group policy editor dengan cara berikut :</p>

<p>1.c. Ketikkan gpedit.msc pada command prompt. Apabila berhasil, akan tampil menu berikut.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-1.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>1.d. Klik pada menu administrative templates pada bagian kiri, kemudian klik menu windows components pada menu sebelah kanan.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-2.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>1.e. Klik dua kali pada windows compnents dan cari menu Windows update. Pada menu windows update, cari menu "Configure Automatic Update".</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-3.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>1.f. Klik kanan pada menu "Configure Automatic Update". Kemudian klik edit. Untuk mematikan windows update secara otomatis, pilihlah no. 2 dengan nama menu "notify for download and notify for install". Dengan memilih menu no. 2, maka setiap kali ada windows update, akan muncul notifikasi terlebih dahulu sebelum update-nya diunduh. Apabila kita memilih untuk meng-update, maka windows updates akan diunduh, jika memilih jawaban tidak, maka windows updates tidak akan diunduh.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-4.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>1.g. Klik apply dan ok.</p>

<h3 class="{% include classh3.html %}">2. Cara Kedua</h3>

<p>Cara kedua untuk mematikan windows update adalah dengan mengakses menu control panel.</p>

<p>2.a. Buka menu control panel.</p>

<p>2.b. Buka menu system and security</p>

<p>2.c. Buka menu administrative tools.</p>

<p>2.d. Buka menu services.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-5.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>2.e. Cari menu windows updates.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-6.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>2.f. Klik kanan pada menu windows updates dan klik bagian properties.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-7.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Setelah itu klik apply dan ok.</p>


## Setingan Tambahan

<p>Jika kita sudah mematikan update otomatis untuk windows 10, selanjutnya ada setingan tambahan yang harus diterapkan dalam rangka supaya quota internet kita tidak cepat habis. Yaitu dengan mematikan fitur advance option di dalam windows update. Di dalam menu advanced tersebut, terdapat pilihan bagaimana perilaku komputer kita di dalam jaringan setelah mendapatkan updates terbaru dari windows. Apakah komputer kita akan membagikan update tersebut ke komputer di dalam jaringan internet atau di dalam lokal area komputer terdekat.</p>

<p>Jika kita "on"-kan pilihan tersebut, maka semua update yang telah diunduh, akan dikirimkan ke komputer terdekat di jaringan lokal atau komputer lainnya yang terdekat di dalam jaringan internet. Hal ini tentu mempermudah kecepatan waktu unduh, namun menyebabkan quota cepat habis jika quotanya terbatas. Untuk mematikan fitur ini, silakan ikuti langkah berikut :</p>

<p>1. Buka menu update</p>

<p>2. Pilih advanced option</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-8.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>3. Pilih menu "choose how update are delivered"</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-9.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>4. Pilih menu off seperti gambar berikut.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/stop-windows-update/mematikan-windows-10-update-10.jpg" alt="Cara Mematikan Automatic Update Windows 10 Secara Paksa" title="Cara Mematikan Automatic Update Windows 10 Secara Paksa" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Jika kita memilih pilihan on, maka ketika ada updates yang diunduh dari internet, file yang telah diupdate tersebut, akan dikirimkan ke komputer lain yang terdekat baik di jaringan lokal atau di komputer lain di jaringan internet. Jika kita memilih pilihan off, maka file updates tersebut tidak dikirimkan ke komputer lain. Hal inilah salah satu penyebab mengapa quota internet cepat habis jika menggunakan windows 10 untuk browsing di internet.</p>

<p>Demikian tutorial singkat tentang cara mematikan windows 10 updates agar windows tidak secara otomatis melakukan update. Sayangnya cara ini tidak dapat diterapkan untuk windows 10 home edition. Kami akan membuat tutorial lainnya tentang cara mematikan windows 10 home edition jika ada. Semoga dengan cara ini, kita dapat menghemat quota internet. Sebaiknya, setelah <a href="/cara-install-windows-10.html">install windows 10</a>, segera matikan sistem updatenya yang berjalan otomatis, jika kuota internet anda terbatas.</p>