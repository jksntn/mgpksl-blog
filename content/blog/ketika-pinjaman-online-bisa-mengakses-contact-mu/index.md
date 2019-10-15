---
type:        post
title:       Ketika Pinjaman Online Bisa Mengakses Contactmu
date:        2019-08-03
description: >-
    Beberapa waktu yang lalu saya dikirim sebuah sms dari pinjaman online. Ada seseorang yang saya kenal yang meminjam uang dan belum membayarkannya. 
tags:
 - software
 - apps
---

Beberapa waktu yang lalu saya kedapatan SMS yang berisi kurang lebih seperti gambar di bawah ini, intinya ada teman kantor lama yang meminjam uang tapi menurut pengirim SMS itu, teman saya ini sudah terlambat melakukan pembayaran, jadi saya diminta untuk mengingatkan dia. 

{{< figure
    src="fintech-sms.jpg" 
    caption="Screenshot SMS Saya" >}}

Kalau dari bahasanya, udah jelas sih, berarti aplikasi ini taunya saya ini cuman temen, bukan keluarga. Saya punya dua kesimpulan, antara saya dijadikan penjamin oleh temen saya ini, atau aplikasi pemberi pinjaman ini membaca isi kontak temen saya itu. Karena setelah saya lihat app permissionnya, aplikasi-nya dapat membaca isi kontak.

{{< figure
    src="fintech-app.jpg" 
    caption="Screenshot App Permission" >}}

Sebenernya bahaya **app permission** ini sudah pernah dijelaskan banyak media dari cukup lama, contohnya artikel ini [What those scary app permissions mean][1], sudah agak lama menjelaskan bahaya permission bisa membaca kontak, melihat status phone, mengetahui lokasi, mengubah isi storage, dll. 😥

Tanpa disadari, sebenernya aplikasi seperti gmail juga bisa membaca kontak (itulah mengapa ketika menulis sedikit nama di tujuan email, gmail langsung memberikan rekomendasi nama yang mirip). Apabila kamu menggunakan aplikasi fintech seperti OVO, atau seperti Gojek dan Grab, aplikasi mereka juga meminta akses kontak. Apakah ada kemungkinan mereka mengumpulkan data kontak kita? 

Bisa jadi, tapi caranya halus.  

Berbeda dengan aplikasi fintech yang mari kita sebut, mungkin belum terdaftar di OJK, yang kian kemari makin marak bermunculan di Indonesia. Tentu cara menagih ke 'penjamin' ini tidaklah etis (saya pakai petik karena mungkin penjamin ini engga tau kalau mereka ini dijadikan penjamin). 

Dan buat yang ingin mengetahui mengapa fenomena Fintech ini menjadi marak, bisa mendengarkan penjelasan @hotradeo di [podcast asumsi episode ini][2]. 

## Saran

Menurut saya hindari menggunakan layanan pinjaman online yang caranya sangat mudah dan banyak sekali bisa ditemukan di Playstore, karena tentu saja kalau dari sisi saya, tidak ramah data privacy. 

Kemudian buat yang sudah menggunakan banyak aplikasi android (fintech terjamin atau aplikasi lainnya) dan cukup memperhatikan dan takut datanya banyak diambil, bisa mengubah pengaturan app permission-nya. Caranya tinggal masuk ke setting, temukan aplikasi, dan buka salah satu aplikasi, cari pengaturan app permission, dan tinggal diubah ke no (tidak) untuk permission yang berbahaya seperti melihat kontak, dll seperti yang saya jelaskan di atas.

[1]: https://www.androidcentral.com/look-application-permissions
[2]: https://open.spotify.com/episode/3RV9NgIGr9eAHoCiuXohag?si=00P_wqtBTyCTzWBf2VsXcg