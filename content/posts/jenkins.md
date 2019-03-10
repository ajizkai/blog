---
title: "Jenkins"
date: 2019-03-10T17:32:27+07:00
draft: true
toc: false
images:
tags:
  - untagged
---
### jenkins
```
yum install java-1.8.0-openjdk-devel
```
```
wget url.rpm
rpm -i jenkins.rpm
```
```
systemctl start jenkins
systemctl enable jenkins
```
```
firewall-cmd --add-port 8080/tcp --permanent
firewall-cmd --reload
```
