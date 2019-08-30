---
layout:     post
title:      Polyfills
subtitle:   
date:       2019-08-29
author:     henryace
header-img: img/post-bg-ios8-web.jpg
catalog: true
tags:
    - polyfills
    - javascript
    - shim
---
# Polyfills

1.什麼是Polyfills<br>

"polyfill 是小段程式碼，用各種技術來幫忙各個舊的瀏覽器，補完新的 API，讓你使用起來沒有落差"<br>

<https://medium.com/@tsoen/%E4%BB%80%E9%BA%BC%E6%98%AF-polyfills-89f98f45caf5><br>

2.Shim和Polyfill的差別?<br>

shim：一個庫,它將一個新的API引入到一個舊的環境中,而且僅靠舊環境中已有的手段實現。<br>

polyfill：一個用在瀏覽器API上的shim<br>
做法：<br>
1)我們通常的做法是先檢查當前瀏覽器是否支援某個API<br>
2)如果不支援的話就載入對應的polyfill.然後新舊瀏覽器就都可以使用這個API了<br>

術語polyfill來自於一個家裝產品Polyfilla:
Polyfilla是一個英國產品,在美國稱之為Spackling Paste(譯者注:刮牆的,在中國稱為膩子).

```js
if (!Number.isNaN) {
	Number.isNaN = function isNaN(x) {
		return x !== x;
	};
}
```

<https://codertw.com/%E5%89%8D%E7%AB%AF%E9%96%8B%E7%99%BC/29473/><br>
<https://github.com/getify/You-Dont-Know-JS/blob/1st-ed/up%20%26%20going/ch2.md><br>