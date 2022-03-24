---
layout: post
title: "Cara Membuat Dual Boot Windows 10 Ubuntu"
judulseo: "Cara Membuat Dual Boot Windows 10 Ubuntu Bios Legacy Partisi MBR"
deskripsi: "Cara membuat dual boot windows 10 ubuntu dengan menggunakan sistem BIOS windows legacy dan partisi hard disk MBR dengan file ubuntu terpisah"
excerpt: "Dual boot windwos 10 ubuntu menjadi salah satu pilihan bagi banyak orang ketika ingin merasakan indahnya windows 10 dan gratisnya ubuntu dengan fitur yang melimpah. Ubuntu dengan dukungan dari komunitas opensource dan perusahaan canonical menjadikannya salah satu"
katakunci: "Cara Dual Boot Windows 10 Ubuntu"
slug: "dual-boot-windows-10-ubuntu"
date: 2022-03-06 01:00:00
tanggalpostterbit: 2022-03-06 
tanggalpostmodif: 2022-03-06
categories: windows
tags: ["dual-boot-windows-ubuntu" , "dual-boot"]
penulis: achmad
changefreq: monthly
priority: "0.8"
banner: windows-ubuntu.jpg

---

{% include toc.html %}

<p>Dual boot windwos 10 ubuntu menjadi salah satu pilihan bagi banyak orang ketika ingin merasakan indahnya windows 10 dan gratisnya ubuntu dengan fitur yang melimpah. Ubuntu dengan dukungan dari komunitas opensource dan perusahaan canonical menjadikannya salah satu distro linux paling mudah digunakan dan paling banyak dioprek oleh banyak developer atau penyuka linux.</p>

<p>Ubuntu merupakan turunan dari debian yang memiliki fitur yang sangat banyak, diantaranya adalah koneksi modem GSM baik mifi atau broadband, koneksi wifi yang plug and play, plug and play printer dan masih banyak fitur lainnya. Dengan kata lain menggunakan ubuntu atau debian, serasa menggunakan windows. Tentunya ini sangat cocok untuk pemula.</p>

## Cara Membuat Dual Boot Ubuntu Dan Windows 10

## Persiapan

<p>Berikut ini daftar yang harus disiapkan :</p>

<p>1. Komputer windows 10.</p>

<p>Partisi yang kami gunakan menggunakan jenis MBR. Oleh karena itu, <a href="/cara-mengetahui-jenis-partisi-harddisk">kenali dulu jenis partisi windows</a> yang digunakan. Jika akan melakukan install windows dan ubuntu dengan fresh install, pastikan saat melakukan <a href="/cara-install-windows-10">instal windows 10</a> menggunakan partisi MBR. Jika partisi windows 10 yang digunakan menggunakan partisi GPT, maka sebaiknya dirubah terlebih dahulu menjadi MBR, walaupun secara teori menggunakan partisi GPT pun bisa, tetapi belum pernah kami lakukan. Silakan baca tutorialnya tentang <a href="/cara-merubah-partisi-mbr-menjadi-gpt">cara merubah partisi MBR ke GPT dan sebaliknya</a>. Karena tutorial yang kami buat menggunakan partisi windows berjenis MBR.</p>

<p>2. Ubuntu yang dapat diperoleh di web resminya ubuntu.com</p>

<p>3. Buat installer untuk ubuntu.</p>

<p>4. <a href="/partisi-harddisk-windows">Buat partisi windows</a> sebesar 40 giga untuk menampung file-file ubuntu dan jangan diformat.</p>


## Partisi Windows Dan Sistem BIOS

<p>BIOS yang digunakan di dalam komputer windows ada dua jenis yaitu Legacy dan UEFI. Dual boot windows 10 dan ubuntu dapat berjalan baik dengan sistem BIOS Legacy atau UEFI. Jika sobat membeli komputer pc atau laptop, biasanya sistem BIOS yang tertanam di dalamnya adalah Legacy. Sistem BIOS Legacy sudah mencukupi untuk dual boot windows dan ubuntu.</p>

<p>Hal lainnya yang perlu diperhatikan adalah partisi windows. Partisi windows yang banyak digunakan saat ini adalah <a href="/perbedaan-partisi-mbr-dan-gpt">partisi MBR</a>. Tutorial yang kami buat di artikel ini menggunakan jenis partisi MBR. Dan kabarnya jenis partisi GPT juga tidak mengalami masalah untuk dual boot linux windows. Namun hal ini belum pernah kami lakukan.</p>

<p>Aplikasi untuk membuat installer ubuntu yang kami gunakan adalah menggunakan rufus. Karena di dalam rufus ada pilihan pembuatan installer ubuntu dengan sistem MBR dan UEFI (Walau komputernya menggunakan Legacy pun tetap bisa), karena <a href="/partisi-harddisk-windows">partisi windows</a> yang kami gunakan adalah MBR.</p>

<p>Kesimpulannya adalah windows 10 yang kami gunakan menggunakan sistem BIOS Legacy (UEFI pun bisa) dan jenis partisinya adalah MBR. Kami anggap sobat yang mengikuti tutorial ini sudah mempunyai komputer pc atau laptop berbasis windows 10.</p>


## Instal Ubuntu

<p>1. Booting melalui installer ubuntu </p>

<p>Lakukan booting dengan menggunakan installer ubuntu. Caranya adalah dengan merestart komputer dan langsung tekan tombol yang bisa masuk ke menu pilihan booting. Masing-masing laptop dan pabrikan motherboard untuk pc berbeda-beda tombolnya. Untuk laptop MSI, tombolnya adala F11.</p>

<p>2. Pilih pilihan booting menggunakan installer ubuntu.</p>

<p>3. Membuat partisi ubuntu</p>

<p>Sebelumnya partisi windows sebesar 40 giga telah dibuat. Sekarang saatnya membuat partisi untuk ubuntu.</p>

<p>Untuk pemula, pembuatan partisi ubuntu yang paling mudah dan disarankan adalah 3 jenis, yaitu partisi swap, partisi boot dan partisi file sistem. Tipe partisi yang digunakan adalah ext4 journey file system.</p>

<p>Saat pertama kali booting menggunakan installer ubuntu, akan tampak tampilan awal ubuntu seperti berikut ini.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-1.png" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Selanjutnya klik icon install ubuntu yang ada di sebelah kiri atas.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-2.png" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Pilih install ubuntu dan klik continue.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-3.png" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Klik di bagian install aplikasi pihak ketiga yang akan di download ketika proses install ubuntu. Untuk itu pastikan koneksi internet lancar.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-4.png" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Proses install ubuntu dual boot dengan windows 10 dapat dilakukan dengan 2 cara.</p>

<p><strong>Cara pertama</strong> adalah dengan "install ubuntu alongside windows 10". Dengan cara ini, file-file ubuntu akan berada di dalam drive C bersama dengan windows 10.</p>

<p><strong>Cara kedua</strong> adalah dengan install ubuntu di partisi tersendiri di luar drive C. Cara inilah yang digunakan di dalam tutorial ini. Klik bagian "Something Else"</p>

<p>Setelah itu akan tampak partisi kosong sebesar 40 giga yang telah dibuat sebelumnya.</p>

<h3 class="{% include classh3.html %}">Partisi Swap</h3>

<p>Untuk membuat partisi baru klik tombol plus yang ada di kiri bawah. Buatlah partisi swap sebesar 4 giga. Tipe partisinya adalah logical.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-5.jpg" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<h3 class="{% include classh3.html %}">Partisi Boot</h3>

<p>Buat lagi partisi boot sebesar 1 giga dari sisa partisi yang dibuat sebelumnya. Tipe partisinya adalah logical. Sistem hard disknya menggunakan Ext4 journaling file system. Mount poin pilih "boot".</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-6.jpg" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<h3 class="{% include classh3.html %}">Partisi File Sistem</h3>

<p>Sisanya buat untuk file sistem dengan tipe partisi logical. Sistem partisinya adalah Ext4 journaling file system. Mount point pilih "/".</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-7.png" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>4. Install Ubuntu</p>

<p>Klik tombol install dan arahkan pada partisi dengan mount point "/".</p>

<p>4.a. Lokasi negara</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-8.jpg" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Pilih lokasi jakarta untuk negara indonesia.</p>

<p>4.b. Pilihan keyboard</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-9.jpg" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Pilih tipe keyboard yang English.</p>

<p>4.c. User atau pengguna</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-10.jpg" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Buatlah nama user/pengguna dan password sesuai keinginan.</p>

<p>Selanjutnya tunggu hingga proses instalasi selesai. Apabila proses instalasi selesai, komputer harus direstart bila ingin menggunakan ubuntu secara penuh.</p>

## Dual Boot

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/windows-ubuntu/dual-boot-ubuntu-windows-11.png" alt="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR" title="Cara Membuat Dual Boot Ubuntu Dan Windows 10 Bios Legacy Partisi MBR"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Setelah ubuntu berhasil diinstall bersamaan dengan windows 10, maka setiap kali komputer dihidupkan atau direstart, secara otomatis komputer akan memberikan dua pilihan sistem OS yaitu ubuntu dan windows. Jika ingin menggunakan windows, arahkan pada partisi windows dan klik enter. Jika ingin menggunakan ubuntu, arahkan pada partisi ubuntu dan kilik enter.</p>

<p>Di dalam sistem operasi linux terdapat aplikasi GRUB. Singkatan dari GRUB adalah GNU GRand Unified Bootloader. Grub adalah sistem bootloader package yang digunakan sistem linux sebelum masuk ke dalam sistem. Sistem grub ini akan tersimpan juga di dalam memori partisi MBR windows. Dengan fitur ini, para pecinta linux ubuntu dapat dengan mudah melakukan dual boot ubuntu dengan windows 10 tanpa aplikasi tambahan lainnya.</p>