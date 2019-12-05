---
layout: post
title:  "API Gateway for a home automation device using MQTT & nodeJS"
date:   2019-12-04 22:23:24 +0700
categories: product design
author: Muhammad iqbal syamil ayasy
author_pic: https://avatars3.githubusercontent.com/u/22183588?s=400&v=4
project_link: https://github.com/2pai/kiana
---

## Abstrak
API gateway IOT device atau yang nanti nya kita sebut sebagai Kiana merupakan sebuah API yang menghubungungkan perangkat IOT dengan REST Server. API gateway ini dibuat untuk mempermudah untuk berinteraksi dengan perangkat IOT yang ada di rumah.API gateway ini menggunakan protokol MQTT untuk berkomunikasi dengan perangkat IOT. API Gateway ini ditulis menggunakan bahasa pemrograman nodeJS dengan menggunakan framework expressJS dan influxDB untuk database nya.

## Deskripsi
Kiana merupakan sebuah API gateway yang menghubungkan perangkat IOT dengan REST server menggunakan protokol MQTT. Pengguna dapat melakukan proses input melalui perangkat IOT dan mentrigger (aksi) perangkat IOT melalui REST server

## Cara Kerja 
- Setiap perangkat IOT akan di daftarkan dan memperoleh topic dari MQTT server untuk di publish dan subscribe  dari device IOT tersebut 
- Apabila user ingin melihat info (input) dari perangkat IOT maka API gateway akan membaca log dari influxDB tentang device tsb
- Apabila user ingin melakukan aksi pada perangkat IOT melalui REST server. maka ketika request diterima akan mempublish aksi kedalam topic pada perangkat IOT yang terdaftar

## Teknologi yang digunakan

- Bahasa Pemograman Server : nodeJS
- REST Server : expressJS
- MQTT Client : mqtt
- MQTT server : mosquitto
- Database : influxDB, redis (caching)
- Design Pattern : CQRS
- Testing : Jest
- Containerization : Docker + docker-compose
