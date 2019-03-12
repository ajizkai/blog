---
title: "Jenkins"
date: 2019-03-10T17:32:27+07:00
draft: false
toc: false
images:
tags:
  - devops
  - ci/cd
---
### jenkins
#### Install java untuk jenkins
```
yum install java-1.8.0-openjdk-devel
```
#### Mengunduh jenkins untuk CentOS dari link [jenkins](https://pkg.jenkins.io/redhat-stable/)
```
#mengunduh jenkins.rpm
wget jenkins.rpm
#menginstal jenkins
rpm -i jenkins.rpm
```
#### Manage service jenkins
```
#menjalankan service jenkins
systemctl start jenkins
#auto start service Jenkins
systemctl enable jenkins
```
#### Allow port jenkins
```
firewall-cmd --add-port 8080/tcp --permanent
firewall-cmd --reload
```
