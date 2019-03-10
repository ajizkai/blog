---
title: "Docker"
date: 2019-03-10T17:22:14+07:00
draft: false
toc: false
images:
tags:
  - devops
  - docker
---
### Docker for CentOS
```
yum install -y yum-utils \
  device-mapper-persistent-data \
  lvm2

yum-config-manager \
    --add-repo \
    https://download.docker.com/linux/centos/docker-ce.repo

yum install docker-ce docker-ce-cli containerd.io
```
```
systemctl start docker
systemctl enable docker
```
# Management permission
```
usermod -aG docker muftizakaria
systemctl restart docker
```
# Management images docker
download image dan menjalankan image diatas container
```
docker pull helloword
docker images
docker run helloword
```
simple case runnung image sebagai container dengan beberapa parameter :
    1. -i : interactive
    2. -t : tty
    3. -d : detach
    4. -p : mapping port
    5. --name : nama dari container

```
docker pull nginx
docker run -itd -p 80:80 --name container-nginx nginx
```
# Build Image
buat Dockerfile
```
docker build -t *userdockerhub*/*namaimage* .
docker login
docker push *userdockerhub*/*namaimage*
```
# Management Container
```
docker ps
docker ps -a
```
```
docker stop
docker rm
docker rmi
```
# Useful Command
```
docker --help
```
