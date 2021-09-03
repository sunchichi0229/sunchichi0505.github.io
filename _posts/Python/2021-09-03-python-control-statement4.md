---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(5) - Python Function 
date: 2021-09-02 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはPython function(関数)の内容です。<br>

まず、関数とは「データを渡すと、そのデータに対応した何らかのデータを返すもの」のことです。<br>
つまり、同じ処理をプログラム内で何回も使うときに役に立つのが関数です。<br>
<br>
python functionのbodyには少なくとも一つ以上の文章が必要です。<br>
もし、内容がないfunctionを作る場合、pass keywordを使います。

function名は必要に応じた「_」で分けている単語と共に小文字を原則として使います。<br>

Python functionは大きく分けて２種類あります。<br>
<br>
1.ユーザー定義関数<br>
2.組み込み関数
<br>

本日は<ユーザー定義関数>の例文をいくつか紹介します。

<ユーザー定義関数><br>

<div style="display:inline-box;background-color:lightgray;width:50vw;height:45vh;">
# python user define function<br>
<br>
def my_sum(a, b, c):<br>
&nbsp;&nbsp;return a + b + c<br>
<br>
result = my_sum(1, 2, 3.0)<br>
<br>
print("resultの値 : {0}".format(result))
</div>

<br>