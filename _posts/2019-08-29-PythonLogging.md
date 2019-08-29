---
layout:     post
title:      Python Logging
subtitle:   
date:       2019-08-29
author:     henryace
header-img: img/post-bg-ios8-web.jpg
catalog: true
tags:
    - python
    - logging
---
# python logging

Python logging 介紹

1."Python logging tutorial"<br>

<http://zetcode.com/python/logging/><br>
<http://yhhuang1966.blogspot.com/2018/04/python-logging_24.html><br>

 logging.NOTSET	  0	  未設定		x
 logging.DEBUG	  10  除錯等級		logging.debug()
 logging.INFO	  20  訊息等級	    logging.info()
 logging.WARNING  30  警告等級	    logging.warning()
 logging.ERROR	  40  錯誤等級	    logging.error()
 logging.CRITICAL 50  嚴重錯誤等級	logging.critical()
 
 logging.WARNING = 30時，logging.WARNING、logging.ERROR、logging.CRITICAL都會印出來
 
```python
#!/usr/bin/env python

import logging

logger = logging.getLogger('dev')
logger.setLevel(logging.DEBUG)

logger.debug('This is a debug message')
logger.info('This is an info message')
logger.warning('This is a warning message')
logger.error('This is an error message')
logger.critical('This is a critical message')
```