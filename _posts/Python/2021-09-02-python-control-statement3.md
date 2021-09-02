---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(4) - Python条件分岐3 
date: 2021-09-01 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはpython条件分岐のwhile文の内容です。<br>

Pythonのwhile文の条件分岐は他の言語と似ています。<br>

ただし、「do~while」の文は存在しないことだけは覚えときましょう。<br>

<div style="display:inline-box;background-color:lightgray;width:50vw;height:40vh;">
idx = 0<br>
mySum = 0<br>
<br>
while idx < 10:<br>
&nbsp;&nbsp;mySum += idx<br>
&nbsp;&nbsp;idx += 1<br>
<br>
print("0~9までの合計 : {}".format(mySum))
</div>