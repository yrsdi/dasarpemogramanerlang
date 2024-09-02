---
title: Sejarah dan Keunggulan Erlang
description: Sejarah singkat dan keunggulan yang menjadi unik dari bahasa ini
keywords: [erlang, belajar erlang, sejarah]
---

### Pendahuluan

Ebook tutorial ini saya susun, atas dasar sedikitnya referensi berbahasa indonesia yang membahas tentang bahasa pemrograman ini. Ketidakpopuleran bahasa ini kemungkinan menjadi penyebabnya.

Pada dasarnya bahasa pemrograman Erlang bukanlah bahasa yang susah untuk dipelajari apalagi dengan keungulan unik yang dimiliknya. Bahasa pemrograman ini dirancang kuat untuk menangani aplikasi real-time, lightweight-concurrent, dan fault-tolerant  membuatnya layak untuk dipelajari.

### Sejarah singkat

Erlang adalah bahasa pemrograman yang dikembangkan oleh Ericsson pada akhir 1980-an, dengan tujuan untuk membuat sistem telekomunikasi yang lebih *efisien*, *scalable*, dan dapat diandalkan. Bahasa ini pertama kali diperkenalkan oleh Joe Armstrong, Mike Williams, dan Robert Virding, yang bekerja di Ericsson Computer Science Laboratory. Erlang mulai digunakan secara internal pada 1986 dan kemudian dirilis *open sorce* pada tahun 1998. Nama "*Erlang*" sendiri berasal dari gabungan nama *Agner Krarup Erlang*, seorang matematikawan Denmark yang terkenal dengan karyanya di bidang teori antrian, dan ada yang menyebutkan juga sebagai singkatan dari "*Ericsson Language*".

Erlang dirancang dengan beberapa keunggulan utama yang menjadikannya pilihan ideal untuk pengembangan sistem telekomunikasi, jaringan, dan aplikasi yang membutuhkan *availability* yang tinggi

1. **Concurrency (Konkruensi)**: Erlang memiliki kemampuan untuk menjalankan ribuan hingga jutaan proses ringan (*lightweight processes*) secara bersamaan dengan manajemen memori yang efisien. Setiap proses berjalan secara independen dan tidak berbagi memori, yang membuatnya aman dari masalah seperti *deadlock* dan *race conditions*.
2. **Fault Tolerance (Toleransi Kesalahan)**: Salah satu fitur utama Erlang adalah kemampuannya untuk menangani kegagalan dengan baik. Erlang menerapkan model "*let it crash*", di mana aplikasi dirancang untuk tetap berjalan meskipun beberapa bagiannya mengalami kegagalan. Fitur ini sangat penting dalam sistem telekomunikasi yang memerlukan uptime tinggi.
3. **Distributed Computing (Komputasi Terdistribusi)**: Erlang mendukung komputasi terdistribusi secara alami. Ini memungkinkan pengembang untuk membangun sistem yang tersebar di banyak node atau server, yang dapat berkomunikasi dan bekerja sama satu sama lain dengan mulus.
4. **Hot Code Swapping**: Erlang memungkinkan programmer untuk memperbarui kode aplikasi yang sedang berjalan tanpa perlu menghentikan sistem. Fitur ini sangat penting dalam aplikasi yang memerlukan uptime 24/7, seperti server telekomunikasi, banking.

Erlang memiliki beberapa keunikan yang membedakannya dari bahasa pemrograman lainnya:

1. **Actor Model**: Erlang menggunakan model aktor untuk concurrency, di mana setiap proses adalah aktor yang dapat mengirim dan menerima pesan. Ini berbeda dari model threading tradisional yang digunakan oleh banyak bahasa lain.
2. **Functional Programming**: Erlang adalah bahasa pemrograman fungsional yang mendukung pola rekursi, immutable data, dan first-class functions. Hal ini membuat kode lebih mudah untuk dianalisis dan diuji.
3. **VM (Virtual Machine) BEAM**: Erlang berjalan di atas BEAM, virtual machine yang sangat efisien untuk menjalankan aplikasi yang membutuhkan waktu respons rendah dan throughput tinggi.

Erlang telah digunakan secara luas di berbagai industri, terutama dalam sistem yang memerlukan skalabilitas tinggi dan toleransi terhadap kegagalan. Beberapa perusahaan yang sukses menggunakan Erlang antara lain:

1. **Ericsson**: Sebagai perusahaan yang menciptakan Erlang, Ericsson telah menggunakannya untuk membangun sistem telekomunikasi yang andal selama beberapa dekade.
2. **WhatsApp**: WhatsApp menggunakan Erlang untuk membangun sistem pesan instan yang dapat menangani jutaan pengguna aktif secara bersamaan dengan latensi rendah.
3. **RabbitMQ**: Platform pesan (message broker) populer yang dibangun di atas Erlang, mendukung komunikasi antar-sistem yang andal dan terukur.
4. **Cisco**: Menggunakan Erlang dalam pengembangan produk-produk jaringan yang memerlukan skalabilitas dan ketersediaan tinggi.
