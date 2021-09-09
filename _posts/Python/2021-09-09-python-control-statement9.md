---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(10) - Python Object3
date: 2021-09-08 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはPythonのオブジェクト指向プログラミングの内容です。<br>

dir(obj) 関数は Python のビルトイン関数です。何もモジュールをインポートすることなく使うことができます。<br>
dir(obj) 関数は、引数に渡した obj オブジェクトの全ての属性 (メソッドやプロパティ) を返します。<br>

< dir関数 ><br>

<div style="display:inline-box;background-color:lightgray;width:40vw;height:45vh;">
class Person:<br>
&nbsp;&nbsp;age = 20<br>
&nbsp;&nbsp;name = 'John Doe'<br>
<br>
<br>
for attr in dir(Person()):<br>
&nbsp;&nbsp;if attr.startswith('__'): # __ 始まりはスキップ<br>
&nbsp;&nbsp;&nbsp;&nbsp;continue<br>
&nbsp;&nbsp;print(attr)<br>
</div>
<br>
< 実行結果 >
<div style="display:inline-box;background-color:lightgray;width:40vw;height:10vh;">
age<br>
name<br>
</div>