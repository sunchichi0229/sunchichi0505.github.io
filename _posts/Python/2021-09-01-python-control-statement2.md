---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(3) - Python条件分岐2 
date: 2021-08-31 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはpython条件分岐のfor文の内容です。<br>

Pythonのfor文の条件分岐は２つの方法がある。<br>

「for ~ in range()」形と「for ~ in dict,list」形です。<br>

「for ~ in range()」を利用した場合<br>

<div style="display:inline-box;background-color:lightgray;width:50vw;height:40vh;">
mySum = 0<br>
<br>
for tmp in range(1,10,2):<br>
&nbsp;&nbsp;mySum += tmp<br>
&nbsp;&nbsp;print("現在のtmp{}で、現在の累積は{}です".format(tmp,mySum))<br>
<br>
print("合計の累積は{}です".format(mySum))<br>    
</div>

<br>

「for ~ in dict,list」を利用した場合<br>
<div style="display:inline-box;background-color:lightgray;width:50vw;height:180vh;">
myList = [1, 2, 3, 4, 5]<br>
mySum = 0<br>
<br>
for tmp in myList:<br>
&nbsp;&nbsp;mySum += tmp<br>
<br>
print("リストの合計 : {0}".format(mySum))<br>
<br>
####################################<br>
<br>
myList = [(1, 2), (3, 4), (5, 6)]<br>
mySum = 0<br>
<br>
for (tmp1, tmp2) in myList:<br>
&nbsp;&nbsp;mySum += (tmp1 + tmp2)<br>
<br>
print("リストの合計 : {0}".format(mySum))<br>
<br>
####################################<br>
<br>
myDict = { "田中" : 24, "鈴木" : 21 }<br>
<br>
for (key,value) in myDict.items():<br>
&nbsp;&nbsp;print("Key : {} , Value : {}".format(key,value))<br>
<br>
####################################<br>
<br>
<br>
score = [100, 50, 80, 90, 70, 60]<br>
mySum = 0<br>
<br>
for i in range(len(score)):<br>
    mySum += score[i]<br>
<br>
print("score合計は%d" % mySum)<br>
</div>