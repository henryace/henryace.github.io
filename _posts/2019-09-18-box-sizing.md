---
layout:     post
title:      css:box-sizing屬性
subtitle:   
date:       2019-09-18
author:     henryace
header-img: img/post-bg-js-version.jpg
catalog: true
tags:
    - css
---
# 關於 box-sizing 屬性

## box-sizing 介紹

當你設定一個元素樣式為 box-sizing:<br> 
這個元素的內距和邊框將不會增加元素本身的寬度。<br> 

|參數值	     |語法	  |說明
|content-box	|box-sizing:content-box; |DIV 設定的寬度僅為內容寬度，而內距與邊框額外加上去。
|border-box	|box-sizing:border-box;      |DIV 設定的寬度就已經包含內容寬度、內距與邊框寬度。
|inherit	|box-sizing:inherit;         |繼承至父層的 broder-sizing 設定値。


參考資料：<br>
1.學習 CSS 版面配置：<br>
<http://zh-tw.learnlayout.com/box-sizing.html><br>
2.CSS3 box-sizing 屬性<br>
<http://bit.ly/2O9N1MQ>