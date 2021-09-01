---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(2) - Python条件分岐 
date: 2021-08-26 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはpython条件分岐のif文の内容です。

Pythonのif文の条件分岐は２つの方法がある。<br>

一つは「if ~ elif ~ else」の形である。<br>
もう一つは「in文」の形である。<br>
また、コードblockを表現するため、他の言語のように{ }を利用せず、「indentation」を利用する。<br>
以下の例文を参考にする<br>
「if ~ elif ~ else」を利用した場合<br>

<div style="display:inline-box;background-color:lightgray;width:50vw;height:40vh;">
a = 20<br>

if a % 3 == 0:<br>
&nbsp;&nbsp;print("{}は3の倍数です".format(a))<br>
elif a % 5 == 0:<br>
&nbsp;&nbsp;print("{}は5の倍数です".format(a))<br>
else:<br>
&nbsp;&nbsp;print("{}は3と5の倍数ではないです".format(a)) <br>
</div>

<br>

「in文」を利用した場合<br>
<div style="display:inline-box;background-color:lightgray;width:50vw;height:80vh;">
area = ["東京", "大阪", "沖縄"]<br>
region = "兵庫県"<br>
<br>
if region in area:<br>
&nbsp;&nbsp;pass<br>
else:<br>
&nbsp;&nbsp;print("{} 地域は含まれません".format(region))<br>   
<br>
<br>
mydict = { "東京" : 100, "名古屋" : 200 }<br>
region = "愛知県"<br>
<br>
if region in mydict:<br>
&nbsp;&nbsp;print("キーの値がdict中にあります")<br>
else:<br>
&nbsp;&nbsp;print("キーの値がdict中にありません")<br>
</div>