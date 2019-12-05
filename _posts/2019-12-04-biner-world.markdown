---
layout: post
title: "Biner World, 2D Mobile Game Platformer"
date:   2019-12-04 22:23:24 +1000
categories: software engineering 
author: Anas Rasyid
author_pic: /assets/anas.jpeg 
project_link: https://github.com/anasrasyid/Biner-World
---
## Abstrak

2D Mobile Game Platformer adalah game yang mengharuskan pemain untuk melewati rintangan yang ada pada map untuk menyelesaikan sebuah objektif / win condition. Game tersebut dikemas dalam 2 dimensi dan dimainkan pada perangkat mobile seperti pada namanya 2D Mobile Game Platformer.


## Deskripsi

Biner World adalah game 2D mobile platformer yang memiliki konsep seperti pada umumnya game platformer akan tetapi pemain harus memecahkan kode biner yang ada untuk menuju ke level berikutnya. Pada game ini win conditionnya ketika player berhasil membuka pintu menuju level selanjutnya dengan memecahkan kode biner yang ada. Selain itu pemain juga harus melewati jebakan yang ada seperti pada game platformer umumnya. Jika terkena jebakan, maka otomatis nyawa pemain akan berkurang. Game ini bertipe endless game yang menggunakan beberapa pattern map tetapi berbeda biner yang dipecahkan. Hal yang bertindak sebagai skor pada game ini adalah jumlah level yang berhasil diselesaikan dan lamanya waktu bermain.

Experience yang ingin yang ingin disampaikan pada game ini adalah pengalaman mengubah bilangan biner ke basis 10 atau pun sebaliknya dan kemampuan untuk berfikir cepat serta keseimbangan motorik dan otak saat menyelesaikan satu level.

Adapun target dan jenis gamenya  sebagai berikut :

Target         : Umum usia 15 tahun keatas

Category        : Endless, Platformer, Puzzle

Platrom        : Mobile (Android)

Bahasa        : English


## Cara Kerja

Pada saat loading level, terjadi random key untuk membuka pintu untuk ke next level dan random beberapa pola level. Selesai loading level pemain dapat memainkan game dengan tiga buah nyawa. Pemain harus menyelesaikan objektif atau win condition untuk dapat ke level berikutnya. Seperti pada game platformer umumnya terdapat jebakan untuk membuat nyawa pemain berkurang dan ketika nyawa pemain habis maka permainan selesai. Skor pada permainan ini terdapat dua komponen yaitu banyaknya level yang telah diselesaikan dan waktu pemain bermain. Waktu disini dihitung setiap pemain memulai level permainan.

Terdapat dua jenis level pada biner world yaitu jenis pertama dimana pemain harus membuat bilangan biner yang sesuai dengan key. Adapun cara untuk membuat bilangan biner pemain cukup menyentuh kotak biner untuk mengubahnya. Misal sebelumnya angka satu maka setelah disentuh menjadi 0 begitu juga sebaliknya. Selanjutnya jenis kedua dimana pemain harus membuat bilangan yang berada di atas pintu next level sesuai dengan key yang dalam bentuk biner dengan menyentuh beberapa kotak yang dapat mengakibatkan nilai di atas pintu berubah. Level jenis kedua akan digunakan setelah pemain melewati 5 level.

![](/assets/anas1.png)
![](/assets/anas2.png)
![](/assets/anas3.png)


## Teknologi yang Digunakan
- Game Engine : Unity 2018.3.3f1 (64-bit)
- Code Editor dan IDE : Microsoft Visual Studio Community 2017 ver 15.9.4
- Bahasa Pemrograman : C#