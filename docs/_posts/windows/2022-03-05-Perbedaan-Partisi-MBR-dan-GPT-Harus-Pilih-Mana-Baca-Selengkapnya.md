---
layout: post
title: "Perbedaan Partisi MBR dan GPT Harus Pilih Mana Baca Selengkapnya"
judulseo: "Perbedaan Partisi MBR dan GPT - Arti Partisi MBR - Arti Partisi GPT"
deskripsi: "Perbedaan MBR dan GPT, dua jenis partisi yang bisa dipakai dalam penggunaan komputer, yaitu komputer windows, macbook atau distro linux"
excerpt: "Stuktur partisi dari suatu harddisk yang dipakai di dalam komputer ada 2 tipe saat ini, yaitu MBR dan GPT. Kedua jenis partisi harddisk ini sering dipakai bagi pengguna komputer windows atau linux. Partisi itu sendiri adalah suatu ruang tersendiri yang"
katakunci: "Perbedaan Partisi MBR dan GPT"
slug: "perbedaan-partisi-mbr-dan-gpt"
date: 2022-03-05 01:00:00
tanggalpostterbit: 2022-03-05 
tanggalpostmodif: 2022-03-05
categories: windows
tags: ["partisi-mbr" , "partisi-gpt"]
penulis: achmad
changefreq: monthly
priority: "0.8"
banner: beda-partisi-gpt-dan-mbr.jpg

---

{% include toc.html %}


<p>Stuktur partisi dari suatu harddisk yang dipakai di dalam komputer ada 2 tipe saat ini, yaitu MBR dan GPT. Kedua jenis partisi harddisk ini sering dipakai bagi pengguna komputer windows atau linux. Partisi itu sendiri adalah suatu ruang tersendiri yang dibuat di dalam suatu harddisk yang berfungsi layaknya harddisk itu sendiri. Partisi dapat diakses oleh sistem operasi itu sendiri, misalnya windows.</p>

<p>Bagi pemula, menggunakan jenis MBR sangat disarankan karena mudah penggunannya. Sedangkan untuk jenis GPT, masih sangat jarang digunakan karena masih sedikit pembuat harddisk yang support jenis ini. Jika pun ada, masih belum support dengan banyak perangkat yang ada. Mari kita tengok sedikit keterangan tentang harddisk MBR dan GPT.</p>

## MBR (Master Boot Record)

<p>Kebanyakan harddisk komputer windows masih menggunakan jenis MBR karena MBR adalah jenis pertama yang banyak digunakan di komputer PC yang banyak kompatible dengan banyak perangkat dan juga mudah untuk pengoperasiannya.</p>

<p>MBR adalah suatu struktur data yang terdapat di dalam harddisk yang terbentuk ketika suatu partisi dibuat di dalam harddisk tersebut. Di dalam MBR terdapat suatu executable kode yang biasa disebut master boot code, the disk signature dan tabel partisi untuk disk.</p>

<h3 class="{% include classh3.html %}">Master Boot Code</h3>

<p>Master boot code akan melakukan aktifitas berikut :</p>

<p>1. Scan tabel partisi yang sedang aktif</p>

<p>2. Scan partisi dimulai dari awal boot sektor yang sedang aktif</p>

<p>3. Boot sektor yang aktif partisinya akan diloads ke dalam memori</p>

<p>4. Executable code akan ditransfer ke dalam boot sektor</p>

<p>Jika master boot code tidak bisa melakukan aktifitas ini, maka akan muncul beberapa pesan berikut :</p>

<p>1. Tabel partisi akan invalid</p>

<p>2. Loading sistem operasi akan mengalami error</p>

<p>3. Missing operation system</p>

<p>Partisi utama yang bisa dibuat di dalam harddisk MBR maksimal 4 buah. Sehingga jika ingin membuat lebih dari 4 partisi, sisanya harus dibuat menjadi logical. Di dalam disk logical akan dapat memuat extended boot record. Banyaknya volume logic yang dibuat bisa banyak sekali.</p>

<p>Berikut gambaran singkat struktur data di dalam harddisk MBR.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/partisi-mbr-gpt/partisi-mbr.png" title="Beda harddisk jenis MBR dan GPT" alt="Beda harddisk jenis MBR dan GPT"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Kapasitas penyimpanan harddisk jenis MBR adalah 2,2 terabytes. Untuk pengguna komputer rumah, sekolah dan pekantoran, kapasitas 2 tera sudah sangat mencukupi.</p>

<p>Seiring dengan hadirnya harddisk GPT, keberadaan MBR akan tergantikan sedikit demi sedikit. Walaupun mencari atau mengubah harddisk MBR menjadi GPT tidaklah semudah membalikkan telapak tangan atau mungkin memang tidak bisa. Jika kita membeli harddisk baru, maka kebanyakan masih berjenis MBR. Karena memang MBR adalah jenis harddisk yang masih sangat kompatible dengan berbagai perangkat.</p>

<p>Besarnya master boot record biasanya sebesar 512 MB atau lebih. File ini akan otomatis terbentuk ketika melakukan instalasi windows, yang berakibat jenis harddisknya akan otomatis menjadi MBR. Kami telah melakukan uji coba untuk mengubah harddisk MBR menjadi GPT, namun akan berubah sendiri menjadi MBR ketika instalasi selesai dilakukan.</p>

<p>Jika di dalam MBR mengalami kerusakan, maka harus dilakukan perbaikan supaya windows dapat loading melalui MBR. Mulai windows 7, ketika windows gagal untuk loading, maka dapat dilakukan repair master boot record dengan perintah "bootrec" yang kemudian diikuti dengan perintah "fixmbr". Hal ini biasa terjadi jika harddisk digunakan untuk dual boot windows dan linux serta partisi linux dihapus atau gagal booting.</p>

## GPT (GUID Partition Table)

<p>GPT adalah standar baru dalam hal partisi hard disk yang biasa digunakan di komputer pc atau server, seperti hard disk biasa atau SSD menggunakan Globally Unique Identifier (GUID. Biasanya semua jenis sistem operasi sudah support GPT, yaitu di antaranya MacOS, windows dan berbagai jenis distro linux.</p>

<p>Dengan menggunakan GPT, memungkinkan untuk membuat partisi dengan jumlah yang tak terbatas dan kapastis harddisk pun tak terbatas. Namun banyaknya jumlah partisi terbatas dari sistem operasi itu sendiri. Misalnya untuk windows, maksimal banyaknya partisi yang bisa dibuat adalah 128 buah.</p>

<p>Keuntungan menggunakan GPT adalah data yang disimpan di dalam hardidisk akan disebarkan di berbagai sektor di dalam disk. Sehingga memudahkan untuk recovery data jika terjadi kerusakan sistem. Recovery dapat dilakukan dengan mudah dari disk yang tidak mengalami kerusakan. Istilah kerennya yang biasa dibaca adalah redudancy on the disk dan kemampuan untuk self-repair.</p>

<p>Namun membuat partisi GPT tidaklah mudah. Kami sendiri telah mencobanya dan tidak mudah. Apalagi ada beberapa keluhan di berbagai forum online yang menyebutkan adanya kesulitan untuk install windows di dalam partisi GPT. Partisi GPT bisa digunakan sebagai penyimpan data mulai windows 7 dan Vista.</p>

<p>Khusus untuk komputer windows, windows hanya dapat booting menggunakan partisi GPT yang menggunakan tipe BIOS terbaru yang disebut UEFI. Sistem UEFI BIOS mulai dikenalkan sejak tahun 2011. Mulai windows 7 64-bit dan Vista 64-bit dapat booting menggunakan UEFI dan GPT tanpa harus menggunakan driver microsoft.</p>

<p>Penggunaan GPT cocok untuk perusahaan yang memiliki jumlah data yang besar dengan kapasitas hard disk yang tentunya besar juga, melebihi 2,2 terabytes.</p>

<p>Gambaran Skema Partisi GPT.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/partisi-mbr-gpt/partisi-gpt.png" title="Beda harddisk jenis MBR dan GPT" alt="Beda harddisk jenis MBR dan GPT"  {% include classlazy.html %} {% include classimage.html %} ></p>

## Kesimpulan

<p>Perbandingan Partisi GPT dan MBR.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/partisi-mbr-gpt/gpt-dan-mbr.png" title="Beda harddisk jenis MBR dan GPT" alt="Beda harddisk jenis MBR dan GPT"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Pemilihan partisi hard disk, apakah menggunakan MBR atau GPT menjadi salah satu pilihan penting dalam menggunakan komputer. Jika harddisk mempunyai kapasitas tidak lebih besar dari 2,2 tera, sebaiknya menggunakan jenis partisi MBR. Karena kebanyakan perangkat dan aplikasi sudah sangat support dengan keberadaan MBR dan mudah untuk digunakan.</p>

<p>Sedangkan untuk harddisk dengan kapasitas lebih dari 2,2 terabytes, sebaiknya menggunakan jenis partisi GPT. Karena ada beberapa kasus yang kami baca di forum online bahwa hard disk dengan kapasitas lebih dari 2,2 terabytes, yang maksimal terbaca adalah 2,2 terabytes, dan sisanya tidak terbaca oleh sistem. Kemungkinan hal ini dikarenakan jenis MBR hanya mampu membaca partisi sampai dengan 2,2 tera. Mungkin solusinya adalah dengan dipecah menjadi dua jenis partisi yaitu partisi MBR dan partisi GPT. Juga masalah lainnya seperti kesulitan dalam hal <a href="/cara-install-windows-10">install windows 10</a> di partisi GPT.</p>

<p>Jenis partisi MBR dapat digabungkan dengan jenis partisi GPT. Misalnya partisi GPT untuk data dan partisi MBR untuk booting. Namun hal ini tidak disarankan untuk pengguna komputer pemula.</p>

<p>Sebelum memutuskan menggunakan MBR atau GPT, teliti terlebih dahulu dalam membeli motherboard, jenis hard disk dan komponen lainnya. Penggunaan MBR masih sangat luas dan kompatible dengan banyak perangkat dan aplikasi terbaru. Sedangkan penggunaan partisi GPT masih jarang digunakan untuk pengguna rumahan dan kantoran.</p>
