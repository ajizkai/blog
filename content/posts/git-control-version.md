---
title: "Git Control Version"
date: 2019-03-06T16:21:55+07:00
draft: false
toc: false
images:
tags:
  - devops
  - scm
---
Lab git

<div style="text-align: justify">Git merupakan tools repository yang berguna untuk menyimpan source code, management versi dapat dilakukan di git, dalam kasus semisal aplikasi versi terbaru masih ada bug terdeteksi, kita dapat kembali ke versi sebelumnya dengan mudah,</div>

Install git client
```
   #ubuntu
   apt install -y git-core

   #centos
   yum install -y git-core
```
konfigurasi git untuk sisi developers, konfigurasi ini digunakan untuk memberi tanda pada saat commit sourcecode kita,
```
   #setting username
   git config –global user.name

   #setting user email
   git config –global user.email
```
command operation git
```
   #download repository online
   git clone *url*

   #menambahkan file from working directory to staging area
   git add .

   #membuat perubahan pada repository
   git commit –m “pesan perubahan”

   #upload repository to server repository
   git push origin master

   #create branch
   git branch *branchname*

   #pindah ke branch yang lain
   git checkout *branchname*   

   #menggabungkan beberapa branch
   git merge *branchname*
```

```
   #kembali ke versi sebelumnya
   git checkout *commitid* *file*
```
untuk melihat perubahan pada repository
```
   #melihat log yang ada di local repository
   git log

   #log lebih simple
   git log --decorate --oneline
```
