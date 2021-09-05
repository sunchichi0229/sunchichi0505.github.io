---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(7) - Python Function3 
date: 2021-09-04 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはPython function(関数)の内容です。<br>

本日はlambdaを紹介します。<br>
lambdaは一行で関数を定義する方法です。<br>
ただし、関数の名前がないため、anonymous functionとも言います。<br>
<br>
lambdaは次のような使い方をします。<br>
変数 = lambda 入力変数1, 入力変数2, … : 代わりの表現式<br>
<br>
lambdaの例<br>

<div style="display:inline-box;background-color:lightgray;width:40vw;height:15vh;">

f = lambda x1,x2,x3 : x1 + x2 <br>

#returnは使ってはいけない<br>

print(f(10,20,30))<br>
</div>

<br>