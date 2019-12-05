---
layout: post
title: "How many of me"
date:   2019-12-04 22:23:24 +0900
categories: softwrae engineering 
author: Malik Wali
author_pic: /assets/DIO.jpg 
project_link: https://github.com/malikilamalik/How_Many_Of_Me_In_Indonesia
---

## Abstrak
Aplikasi ini digunakan untuk melihat berapa banyak nama yang sama dengan memasukan nama depan dan nama belakang atau nama depan saja.
Dataset akan diambil dari website daftar pemilih KPU dengan metode scraping menggunakan BeautifulSoap4 dan Selenium,Dataset yang sudah diambil akan dijadikan API menggunakan djangorestframework untuk menghindari terblokirnya IP,lalu untuk tampilan antar muka akan menggunakan framework react.

## Deskripsi
Website untuk melihat berapa banyak orang dengan nama yang sama dengan memasukan nama depan dan nama belakang atau nama depan saja.

## Cara Kerja
1. User memasukan nama
2. Website akan menampilkan jumlah nama yang sama,jumlah nama yang sama di tiap kota,jumlah nama yang sama untuk tiap jenis kelamin.
