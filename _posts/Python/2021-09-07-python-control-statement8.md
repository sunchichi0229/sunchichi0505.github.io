---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(9) - Python Object2
date: 2021-09-06 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはPythonのオブジェクト指向プログラミングの内容です。<br>

objectとは何か？<br>

objectは同じ様々なデータと関数を含んだ一つのデータ構造です。<br>

<div style="display:inline-box;background-color:lightgray;width:40vw;height:100vh;">

#objectとは何か？<br>

class Student(object):<br>
&nbsp;&nbsp;def __init__(self, name, dept, num, grade):<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.name = name<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.dept = dept<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.num = num<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.grade = grade<br>
<br>
&nbsp;&nbsp;def get_student_info(self):<br>
&nbsp;&nbsp;&nbsp;&nbsp;return "名前 : {}, 学科 : {}, 学籍番号 : {}".format(self.name,self.dept,self.num)<br>
<br>
<br>
# object生成<br>
stu1 = Student("田中", "経済", "21-1-001-0001", 3.5)<br>
<br>
# メソッド呼び出し<br>
print(stu1.get_student_info())<br>
print(Student.get_student_info(stu1))<br>
<br>
</div>