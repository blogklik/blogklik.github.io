---
layout: post
title: "3 Cara Mengetahui Jenis Partisi Hard Disk Paling Mudah"
judulseo: "3 Cara Mengetahui Jenis Partisi Hard Disk Paling Mudah"
deskripsi: "Cara mengetahui partisi hard disk, 3 cara paling mudah untuk mengetahui jenis hard disk komputer, bisa lewat command line, control panel"
excerpt: "Misalkan sobat telah membeli komputer baru, entah itu komputer desktop atau laptop. Kemudian setelah membaca beda partisi MBR dan GPT, penasaran ingin mengetahui partisi apa yang digunakan pada komputer dan laptop terbaru tersebut"
katakunci: "Cara Mengetahui Jenis Partisi Hard Disk"
slug: "cara-mengetahui-jenis-partisi-harddisk"
date: 2022-03-05 01:00:00
tanggalpostterbit: 2022-03-05
tanggalpostmodif: 2022-03-05
categories: windows
tags: ["partisi-mbr" , "partisi-gpt"]
penulis: achmad
changefreq: monthly
priority: "0.8"
banner: jenis-partisi-harddisk.jpg

---

{% include toc.html %}

<p>Misalkan sobat telah membeli komputer baru, entah itu komputer desktop atau laptop. Kemudian setelah membaca <a href="/perbedaan-partisi-mbr-dan-gpt">beda partisi MBR dan GPT</a>, penasaran ingin mengetahui partisi apa yang digunakan pada komputer dan laptop terbaru tersebut.</p>

<p>Pengetahuan jenis partisi hard disk adalah hal dasar yang seharusnya dipahami bagi sobat-sobat yang ingin atau sedang sekolah komputer atau mungkin bukan pakar komputer tetapi ingin mendalami tentang komputer. Karena jenis partisi MBR adalah metode partisi yang paling banyak digunakan saat ini sedangkan partisi GPT adalah metode partisi terbaru dengan menjanjikan banyak fitur unggulan dibanding MBR. Walau dalam kenyataannya sampai saat ini masih banyak partisi MBR yang sering dipakai.</p>

## Cara Mengetahui Jenis Partisi Hard Disk

<h3 class="{% include classh3.html %}">1. Menggunakan Command Line</h3>

<p>1.a. Buka aplikasi command prompt (cmd. Cari di kolom pencarian dan ketik cmd, tekan enter pada aplikasi command prompt.</p>

<p>1.b. Ketik perintah diskpart dan tekan enter</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/jenis-partisi-harddisk/cara-mengetahui-jenis-harddisk-1.jpg" alt="Cara Mengetahui Jenis Partisi Hard Disk" title="Cara Mengetahui Jenis Partisi Hard Disk"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>1.c. Ketik list disk</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/jenis-partisi-harddisk/cara-mengetahui-jenis-harddisk-2.jpg" alt="Cara Mengetahui Jenis Partisi Hard Disk" title="Cara Mengetahui Jenis Partisi Hard Disk"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Perhatikan pada gambar yang ditunjukkan oleh panah pada kolom GPT. Jika terlihat tanda bintang pada kolom GPT, maka partisi yang digunakan adalah GPT. Jika tidak terlihat tanda bintang pada kolom GPT, maka partisi yang digunakan adalah MBR.</p>

<h3 class="{% include classh3.html %}">2. Melalui Control Panel</h3>

<p>2.a. Buka aplikasi "create and format hard disk partitions". Pada kolom pencarian windows, ketika "create and format hard disk partitions" dan tekan enter pada aplikasi "create and format hard disk partitions".</p>

<p>2.b. Klik kanan pada partisi hard disk, misalnya partisi C. Pilih properties.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/jenis-partisi-harddisk/cara-mengetahui-jenis-harddisk-3.jpg" alt="Cara Mengetahui Jenis Partisi Hard Disk" title="Cara Mengetahui Jenis Partisi Hard Disk"  {% include classlazy.html %} {% include classimage.html %} ></p>


<p>2.c. Klik pada bagian hardware dan arahkan pada hard disk. Klik properties.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/jenis-partisi-harddisk/cara-mengetahui-jenis-harddisk-4.jpg" alt="Cara Mengetahui Jenis Partisi Hard Disk" title="Cara Mengetahui Jenis Partisi Hard Disk"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/jenis-partisi-harddisk/cara-mengetahui-jenis-harddisk-5.jpg" alt="Cara Mengetahui Jenis Partisi Hard Disk" title="Cara Mengetahui Jenis Partisi Hard Disk"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>2.d. Klik pada bagian volumes dan klik Populate. Hasilnya akan terlihat pada Partition Style. Pada contoh kali ini terlihat bahwa hard disk yang digunakan menggunakan jenis partisi MBR (Master Boot Record.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/jenis-partisi-harddisk/cara-mengetahui-jenis-harddisk-6.jpg" alt="Cara Mengetahui Jenis Partisi Hard Disk" title="Cara Mengetahui Jenis Partisi Hard Disk"  {% include classlazy.html %} {% include classimage.html %} ></p>

<h3 class="{% include classh3.html %}">3. Menggunakan Aplikasi</h3>

<p>Aplikasi yang dapat digunakan untuk mengetahui jenis partisi hard disk adalah mini partition tools. Kabarnya baiknya ada versi gratisnya atawa tidak usah bayar.</p>

<p>3.a. Download aplikasi mini partition tool di web resminya yaitu www.partitionwizard.com.</p>

<p>3.b. Instal aplikasinya. Setelah selesai diinstall, buka aplikasi tersebut dan perhatikan pada bagian informasi disk(terlihat pada panah. Jika jenis partisinya adalah MBR, maka akan terlihat tulisan MBR pada Disk. Jika jenis partisinya adalah GPT, maka akan terlihat tulisan GPT pada Disk.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/jenis-partisi-harddisk/cara-mengetahui-jenis-harddisk-7.jpg" alt="Cara Mengetahui Jenis Partisi Hard Disk" title="Cara Mengetahui Jenis Partisi Hard Disk"  {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Tidak menutup kemungkinan masih ada cara lainnya untuk mengetahui jenis partisi hard disk. Menurut kami, 3 saja sudah cukup.</p>