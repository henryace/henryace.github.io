---
layout:     post
title:      EncNet (FastFCN) 設定
subtitle:   
date:       2019-09-17
author:     henryace
header-img: img/post-bg-js-version.jpg
catalog: true
tags:
    - EncNet
    - FastFCN
---
# EncNet (FastFCN) 設定

因為執行FastFCN出現<br>
```bash
ninja: build stopped: subcommand failed
```

重新設定 EncNet FastFCN<br>

```bash
conda uninstall pytorch
conda install pytorch==1.0.0 -c pytorch
```

Python:3.6.7<br>
cuda 10.0<br>
pytorch 1.0.0<br>

<https://github.com/zhanghang1989/PyTorch-Encoding/issues/162><br>