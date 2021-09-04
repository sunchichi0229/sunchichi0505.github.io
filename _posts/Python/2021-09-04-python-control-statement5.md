---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(6) - Python Function2 
date: 2021-09-03 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはPython function(関数)の内容です。<br>

本日は<組み込み関数>を紹介します。<br>

Pythonは多くの組み込み関数を提供します。これを通じて、簡単にデータ処理をすることが可能です。簡単な四則演算からデータタイプの変換のような処理が簡単に出来ます。<br>

<ol><基本的な組み込み関数><br>
    <li>abs(x): 絶対値をreturn</li>
    <li>all(x): すべての要素がTrueであればTrueを返す</li>
    <li>any(x): いずれかの要素がTrueであればTrueを返す</li>
    <li>eval(expression): 実行可能な文字列の入力を受け、文字列を実行した結果をreturn</li>
    <li>int(x): xの整数への変換</li>
    <li>len(x): xの長さをreturn</li>
    <li>list(x): 繰り返し可能なxの入力を受け、listにしてreturn</li>
    <li>str(x): 文字列に変換してreturn</li>
    <li>tuple(x): 繰り返し可能な要素を受け、tupleに変えてreturn</li>
    <li>type(x): 入力値のデータタイプをreturn</li>
</ol>


<組み込み関数><br>

<div style="display:inline-box;background-color:lightgray;width:50vw;height:45vh;">

print(dir({"key" : 100}))<br>
print(dir([]))<br>
<br>
print(divmod(8,3))<br>
<br>
result = enumerate(["Show","me", "the", "money"])<br>
myList = list(result)<br>
myList[0]<br>
<br>
for idx,item in enumerate(["Show","me", "the", "money"]):<br>
&nbsp;&nbsp;print(idx, item)<br>
<br>
a = 100<br>
print(id(a))<br>
<br>
animal = ["犬","ライオン","トラ","猫"]<br>
print(",".join(animal))<br>
print("-".join(animal))<br>
<br>
def my_func(x):<br>
&nbsp;&nbsp;return x**2<br>
<br>
a = list(map(my_func,range(1,10)))<br>
print(a)<br>
<br>
print(max([7,4,9,2,3,1]))<br>
print(max("This is a sample Text"))<br>
<br>
print(pow(2,4))<br>
<br>
a = [4,7,9,2,3,6]<br>
result = a.sort()<br>
print(result)<br>
print(a)<br>
<br>
a = [4,7,9,2,3,6]<br>
result = sorted(a)<br>
print(result)<br>
print(a)<br>
<br>
a = [1,2,3]<br>
b = ["a","b","c"]<br>
c = list(zip(a,b))<br>
<br>
print(c)<br>
<br>
str=list(zip("Hello","World"))<br>
print(str)<br>
<br>
str=list(zip("Hello1234","World"))<br>
print(str)<br>
</div>

<br>