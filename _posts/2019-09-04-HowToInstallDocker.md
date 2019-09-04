---
layout:     post
title:      How to install tensorflow on docker
subtitle:   
date:       2019-09-03
author:     henryace
header-img: img/post-bg-js-version.jpg
catalog: true
tags:
    - docker
    - tensorflow
---
# How to install tensorflow on docker #

## How to install Docker<br>

Following the steps: <br>
縮網址<http://bit.ly/2Lovqhq><br>

在第3步驟安裝nvidia docker時<br>

設置Repository configuration <br>

step 1:Add the package repositories <br>
step 2: <br>
step 3: <br>

可以直接參考下面的bash script<br>

```bash
curl -s -L https://nvidia.github.io/nvidia-docker/gpgkey | \
  sudo apt-key add -
distribution=$(. /etc/os-release;echo $ID$VERSION_ID)
curl -s -L https://nvidia.github.io/nvidia-docker/$distribution/nvidia-docker.list | \
  sudo tee /etc/apt/sources.list.d/nvidia-docker.list
sudo apt-get update
```

Repository configuration:<br>
<https://nvidia.github.io/nvidia-docker/><br>

## 目錄掛載至 Docker

想要將實體機器的目錄直接掛載至 Docker 容器內，使用 -v 參數

```bash
docker run --runtime=nvidia -it -v /home/G/test:/data tensorflow/tensorflow:latest-gpu bash
python # default:python2.7
python3 # python3.6.8
```

<https://blog.gtwang.org/linux/docker-commands-and-container-management-tutorial/>