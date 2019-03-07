---
title: "Git Control Version"
date: 2019-03-06T16:21:55+07:00
draft: false
toc: false
images:
tags:
  - devops
---
Lab git

<div style="text-align: justify">Git merupakan tools repository yang berguna untuk menyimpan source code, jadi management versi dapat dilakukan di git, dalam kasus semisal aplikasi versi terbaru masih ada bug terdeteksi, kita dapat kembali ke versi sebelumnya dengan mudah,</div>

Install git client
```
   apt install -y git-core #ubuntu

   yum install -y git-core #centos
```
konfigurasi git untuk sisi developers, konfigurasi ini digunakan untuk memberi tanda pada saat commit sourcecode kita,
```
   git config –global user.name #setting username

   git config –global user.email #setting user email
```
command operation git
```
   git clone *url* #download repository online

   git add . #menambahkan file from working directory to staging area

   git commit –m “pesan perubahan” #membuat perubahan pada repository

   git push origin master #upload repository to server repository

   git branch *branchname* #create branch

   git checkout *branchname* #pindah ke branch yang lain  

   git merge *branchname* #menggabungkan beberapa branch
```

```
   git checkout *commitid* *file* #kembali ke versi sebelumnya
```
```
   git log
```
