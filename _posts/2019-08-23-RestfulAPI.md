---
layout:     post
title:      RestfulAPI
subtitle:   
date:       2019-08-23
author:     henryace
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - RestfulAPI
---
# Restful API

如何在ubuntu建立 PyCharm 桌面捷徑?<br>

1.Restful API 教學<br>

原始是使用 django 用作開發畫面<br>

https://github.com/twtrubiks/django-rest-framework-tutorial/tree/master/RESTful-API-Tutorial<br>

2.簡明RESTful API設計要點<br>

HTTP回傳狀態碼要注意：<br>
回傳的狀態碼，代表API這一層的執行狀態，而不是商業邏輯這一層的狀態。<br>
例如：/search?q=xyz搜尋結果是空的，<br>
API結果仍應回傳200，而非404；<br>
因為從API角度來看，/search這個「資源」存在，而且API執行成功。<br>

https://tw.twincl.com/programming/*641y<br>