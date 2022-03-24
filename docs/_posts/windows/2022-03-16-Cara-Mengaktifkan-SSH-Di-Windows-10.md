---
layout: post
title: "Cara Mengaktifkan SSH Di Windows 10"
judulseo: "Cara Mengaktifkan SSH Di Windows 10 Untuk Konek Ke Server"
deskripsi: "Cara mengaktifkan ssh di windows 10 menggunakan aplikasi powersheel agar dapat melakukan remote komputer menggunakan ssh server atau client"
excerpt: "Jika anda membutuhkan koneksi jaringan yang aman di komputer windows untuk remote komputer lain atau vps, maka ssh adalah salah satu solusinya. Koneksi ssh biasanya menggunakan aplikasi putty"
katakunci: "mengaktifkan ssh windows 10"
slug: "ssh-windows-10"
date: 2022-03-16 01:00:00
tanggalpostterbit: 2022-03-16 
tanggalpostmodif: 2022-03-16
categories: windows
tags: [ "ssh-windows-10" , "windows-powershell" ]
penulis: achmad
changefreq: monthly
priority: "0.8"
banner: ssh-windows-10.jpg

---

{% include toc.html %}


<p>Jika anda membutuhkan koneksi jaringan yang aman di komputer windows untuk remote komputer lain atau vps, maka ssh adalah salah satu solusinya. Koneksi ssh biasanya menggunakan aplikasi putty. Kali ini ada kabar terbaru yaitu komputer windows 10 yang sekarang ini sudah banyak dipakai oleh banyak orang, memiliki fitur built-in ssh seperti halnya komputer linux yang dapat dijalankan di PowerSheel. Ingat bahwa bukan di cmd tetapi di PowerShell.</p>

## Apakah SSH itu

<p>SSH bisa disebut sebagai secure sheel protokol. Yaitu suatu metode yang digunakan untuk login ke komputer lain dari komputer kita secara "secure" atau secara aman.</p>

<p>Protokol SSH biasanya digunakan untuk:</p>

<p>1. Akses ke suatu jaringan dengan aman melalui command line.</p>

<p>2. Transfer file dari satu komputer ke komputer lain.</p>

<p>3. Menjalankan dan memantau sistem jaringan suatu komputer dari komputer lain yang jauh jaraknya.</p>

<p>Fitur ssh secara built-in ada di komputer linux. Lambat laun, sepertinya windows mulai tertarik dengan fungsi ini. Oleh karena itu mulai windows 10, pihak pembuat windows menanamkan sistem ssh secara built-in ke dalamnya. Dan fitur ssh ini hanya bisa diakses melalui PowerSheel.</p>

<p>Fitur ssh yang ada di PowerShell tidak terinstall secara otomatis. Anda harus meng-install-nya agar dapat menggunakan fitur ssh ini. Cara untuk mengaktifkan fitur ssh ini ada dua jalan. Berikut ini penjelasannya :</p>

## Cara Pertama

<p>1. Ketikkan "optional features" pada kolom pencarian windows 10. Dengan cara ini, menu "optional features" akan muncul, klik-lah menu tersebut.</p>

<p>2. Klik "add a feature". Carilah fitur "OpenSSH Client" kemudian klik "install". Selanjutnya cari fitur "OpenSSH Server" kemudian klik "install".</p>

<p>Jika ssh belum bisa digunakan, restart komputer anda.</p>


## Cara Kedua

<p>1. Buka aplikasi PowerShell dengan permission sebagai administrator.</p>

<p>2. Cek apakah ssh sudah ter-install atau belum.</p>

<p>
{% highlight ruby %}
Get-WindowsCapability -Online | ? Name -like 'OpenSSH*'
{% endhighlight %}
</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/ssh-windows/ssh-windows-10-1.jpg" alt="Installation of OpenSSH For Windows Server 2019 and Windows 10" Title = "Installation of OpenSSH For Windows Server 2019 and Windows 10" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Jika belum ter-install, akan muncul tulisan berikut ini:</p>

<p>
{% highlight ruby %}
Name  : OpenSSH.Client~~~~0.0.1.0
State : NotPresent
Name  : OpenSSH.Server~~~~0.0.1.0
State : NotPresent
{% endhighlight %}
</p>


<p>3. Install ssh server atau ssh client.</p>

<p>Install ssh client.</p>

<p>
{% highlight ruby %}
# Install the OpenSSH Client
Add-WindowsCapability -Online -Name OpenSSH.Client~~~~0.0.1.0
{% endhighlight %}
</p>

<p>Install ssh server.</p>

<p>
{% highlight ruby %}
# Install the OpenSSH Server
Add-WindowsCapability -Online -Name OpenSSH.Server~~~~0.0.1.0
{% endhighlight %}
</p>

<p>Output dari install ssh server atau ssh client adalah sebagai berikut :</p>

<p>
{% highlight ruby %}
Path          :
Online        : True
RestartNeeded : False
{% endhighlight %}
</p>

<p>Untuk mengetahui bahwa ssh telah terinstall dengan benar, saya melakukan login ke vps server menggunakan ssh</p>

<p>
{% highlight ruby %}
ssh username@ip_address
{% endhighlight %}
</p>

<p>Hasilnya adalah sebagai berikut.</p>

<p><{% include thegambar.html %} {% include thedatasrc.html %}="{% include sourceimage.html %}/ssh-windows/ssh-windows-10-2.jpg" alt="Installation of OpenSSH For Windows Server 2019 and Windows 10" Title = "Installation of OpenSSH For Windows Server 2019 and Windows 10" {% include classlazy.html %} {% include classimage.html %} ></p>

<p>Ternyata saya bisa login ke vps menggunakan ssh di PowerSheel. Itu artinya ssh di windows 10 telah berhasil dikonfigurasi dengan benar. Dan kabarnya, pihak windows mulai meng-integrasi-kan semua fungsi linux ke dalam komputer windows secara bertahap.</p>






