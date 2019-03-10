---
title: "Docker"
date: 2019-03-10T17:22:14+07:00
draft: false
toc: false
images:
tags:
  - untagged
---
### Docker
```
systemctl start docker
systemctl enable docker
```
```
usermod -aG docker muftizakaria
systemctl restart docker
```
```
docker pull helloword
docker images
docker run helloword
```
```
docker pull nginx
docker run -itd -p 80:80 --name container-nginx nginx
```
```
docker build -t *userdockerhub*/*namaimage* .
docker login
docker push *userdockerhub*/*namaimage*
```
```
docker ps
docker ps -a
```
```
docker stop
docker rm
docker rmi
```
```
docker --help
```
