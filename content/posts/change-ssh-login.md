+++
title = "Ganti Pesan Login SSH Linux"
description = ""
type = ["posts","post"]
tags = [
    "devlog",
    "development",
    "ssh",
    "linux",
    "server"
]
date = "2022-26-02"
categories = [
    "Development",
    "Devlog",
]
series = ["Server"]
[ author ]
  name = "Agung Priambada"
+++

Untuk mengganti/menambahkan pesan yang ditampilkan sebelum masuk login:

```
sudo nano /etc/ssh/sshd_config
```

dan tambahkan atau uncomment line ini

```
Banner /etc/banner
```

Path alamat banner /etc/banner dapat diubah sesuai dengan keinginan. Setelah menambahkan line di atas lalu edit file tersebut

```
sudo nano /etc/banner
```

dan isikan pesan/teks yang diinginkan. Setelah itu restart sshd supaya perubahan dapat terlihat.
```
sudo /etc/init.d/ssh restart
```

untuk mengganti pesan setelah login, edit atau tambahkan /etc/motd
```
sudo nano /etc/motd
```

dan isikan pesan yang ingin ditambahkan.