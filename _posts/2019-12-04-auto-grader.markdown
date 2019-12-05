---
layout: post
title: "Aplikasi Penilaian Program secara Otomatis"
date:   2019-12-04 22:23:24 +0900
categories: softwrae engineering 
author: Muhammad Abdurrohman Al Fatih 
author_pic: /assets/fatih.jpg 
project_link: https://github.com/MAAF72/Auto-Grader
---
## Abstrak
Penilaian program secara otomatis yang selanjutnya disebut Auto Grader adalah sebuah aplikasi yang melakukan penilaian terhadap sebuah program dengan masukan dan batasan-batasan yang ditentukan. Auto Grader ini dibuat untuk mempermudah dalam penilaian terhadap sebuah program, juga menghilangkan faktor subjektivitas penilaian. Auto Grader ini dikhususkan untuk melakukan penilaian sebuah program yang ditulis dalam bahasa pemrograman Golang, C++, dan C. Aplikasi ini dibuat menggunakan framework Django untuk situs webnya, dan Python untuk server penilaiannya.

## Deskripsi
Auto Grader adalah sebuah aplikasi yang melakukan penilaian terhadap sebuah program dengan masukan dan batasan-batasan yang ditentukan. Pengguna akan berinteraksi dengan server penilaian melalui situs web. 

## Cara Kerja
Cara kerja Auto Grader ini adalah dengan memanfaatkan situs web sebagai penghubung antara pengguna dengan server penilaian. Pengguna mengunggah kode program di situs web dan masuk dalam antrian penilaian yang disimpan didalam database. Selanjutnya, server penilaian akan melakukan penilaian terhadap kode program tersebut sesuai dengan urutan antrian dan memberikan hasilnya kepada database. Lalu, situs web akan menampilkan hasilnya berdasarkan data yang ada di database.

Cara kerja penilaiannya sendiri adalah sebagai berikut. Pertama, server mengambil data antrian lalu mengkompilasi kode program tersebut dan apabila terdapat error dalam proses kompilasi, program tersebut langsung mendapatkan nilai 0. Selanjutnya, jika program berhasil dikompilasi maka program tersebut akan diuji dengan beberapa masukan yang hasil keluarannya akan dibandingkan dengan keluaran yang diinginkan dengan batasan waktu eksekusi program yang ditentukan. Jika program tersebut gagal dieksekusi dalam waktu yang ditentukan maka uji coba tersebut mendapatkan nilai 0. Program yang hasil keluarannya tidak sesuai dengan keluaran yang diinginkan juga akan mendapatkan nilai 0 untuk uji coba tersebut. Program yang mengalami error saat eksekusi juga akan mendapatkan nilai 0 untuk uji coba tersebut. Setelah diuji dengan beberapa masukan, nilai program akan dikumpulkan dan dibagi sesuai dengan banyaknya uji coba. Hasil tersebut nantinya akan diteruskan ke situs web agar dapat dilihat oleh pengguna.

![](/assets/grader.png)



## Teknologi yang Digunakan
- Database : SQLite 3
- Situs web : Bahasa Python + framework Django
- Server penilai : Bahasa Python
