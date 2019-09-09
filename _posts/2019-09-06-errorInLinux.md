---
layout:     post
title:      How to solve "Sub-process /usr/bin/dpkg returned an error code (1)"
subtitle:   
date:       2019-09-06
author:     henryace
header-img: img/post-bg-js-version.jpg
catalog: true
tags:
    - ubuntu
---
# How to solve "Sub-process /usr/bin/dpkg returned an error code (1)"

執行下列 bash 指令時出現"Sub-process /usr/bin/dpkg returned an error code (1)"<br>
無法自動修復

```bash
sudo apt --fix-broken install
```

參考下面解決方法
Reference:
<https://sites.google.com/a/cnsrl.cycu.edu.tw/da-shu-bi-ji/home/jie-jue-cuo-wusub-process-usr-bin-dpkg-returned-an-error-code-1>

```bash
sudo mv /var/lib/dpkg/info /var/lib/dpkg/info.bak 
sudo mkdir /var/lib/dpkg/info
sudo apt update
sudo apt --fix-broken install
sudo mv /var/lib/dpkg/info/* /var/lib/dpkg/info.bak
sudo rm -rf /var/lib/dpkg/info
sudo mv /var/lib/dpkg/info.bak /var/lib/dpkg/info
```