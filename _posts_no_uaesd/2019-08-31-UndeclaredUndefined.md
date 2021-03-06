---
layout:     post
title:      undefined vs undeclared vs uninitialized
subtitle:   
date:       2019-08-31
author:     henryace
header-img: img/post-bg-js-version.jpg
catalog: true
tags:
    - JavaScript
---
# undefined vs undeclared vs uninitialized

1.undefined<br>

An "undefined" variable is one that has been declared in the accessible scope, but at the moment has no other value in it.<br>

2.undeclared<br>

By contrast, an "undeclared" variable is one that has not been formally declared in the accessible scope.<br>

Reference:
<https://github.com/getify/You-Dont-Know-JS/blob/2nd-ed/types-grammar/ch1.md>

3.uninitialized<br>
3-1.a variable can be in is called the TDZ, the temporal dead zone.<br>
3-2.When something is in an uninitialized state, it is off-limits. You're not allowed to touch it in any way, shape or form, or you'll get an error, and the error you get is the TDZ error.<br>
3-3.let 或 const 聲明的變量擁有暫時性死區（TDZ)當進入它的作用域，它不能被訪問（獲取或設置）直到執行到達聲明。

舉例：

```js
console.log(aVar) // undefined
console.log(aLet) // causes ReferenceError: aLet is not defined
var aVar = 1
let aLet = 2
```

Firefox Error:
ReferenceError: can't access lexical declaration `aLet' before initialization

Reference:
<https://wizardforcel.gitbooks.io/exploring-es6/md/9.4.html>
<https://blog.csdn.net/kittyjie/article/details/50377500>
<http://eddychang.me/es6-tdz/>