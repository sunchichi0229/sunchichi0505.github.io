---
layout: post
current: post
cover:  assets/built/images/python.jpg
navigation: True
title: Python講座(8) - Python Object
date: 2021-09-05 1:10:00
tags: [Python]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

{% include python-table-of-contents.html %}

これはPythonのオブジェクト指向プログラミングの内容です。<br>

<ol>[オブジェクト指向プログラミングの特徴]<br>
<br>
    <li>現実で解決すべき問題をそのままプログラミングで表現</li><br>
    <li>プログラムを構成しているオブジェクトを把握し、<br>データの流れに併せてプログラムを作成</li><br>
    <li>プログラムの設計、作成が比較的に難しい</li><br>
    <li>維持、補修、再利用に利点がある</li><br>
<br>
</ol>

「オブジェクト指向プログラミングが便利な理由」<br>
以下の例を見てみましょう！<br>
次のコードは学生の名前、学科、学籍番号、成績を表す様々な方法を見せます。<br>

<div style="display:inline-box;background-color:lightgray;width:70vw;height:280vh;">

# 学生の名前、学科、学籍番号、成績を表す方法<br>
<br>
# 1人の学生情報を登録<br>
<br>
stu_name = "田中"    # 名前<br>
stu_dept = "経済"    # 学科<br>
stu_num = "21-1-001-0001"   # 学籍番号<br>
stu_grade = 3.5      # 成績<br>
<br>
# もし、３人の学生情報を登録したい時は？<br>
<br>
stu1_name = "藤井"   # 名前<br>
stu1_dept = "医学"   # 学科<br>
stu1_num = "20-2-002-0002"   # 学籍番号<br>
stu1_grade = 4.5     # 成績<br>
<br>
stu2_name = "川崎"    # 名前<br>
stu2_dept = "社会"    # 学科<br>
stu2_num = "19-3-003-0003"   # 学籍番号<br>
stu2_grade = 3.4      # 成績<br>
<br>
stu3_name = "中村"    # 名前<br>
stu3_dept = "化学"    # 学科<br>
stu3_num = "18-4-004-0004"   # 学籍番号<br>
stu3_grade = 3.8      # 成績<br>
<br>
# 上記のコードは重複しているコードが多すぎる。<br>
# リストを使い、もうちょっといいコードに変更します。<br>
<br>
stu_name = ["藤井", "川崎", "中村"]<br>
stu_dept = ["医学", "社会", "化学"]<br>
stu_num = ["20-2-002-0002", "19-3-003-0003", "18-4-004-0004"]<br>
stu_grade = [4.5, 3.4, 3.8]<br>
<br>
print("名前 : {}\n学科 : {}\n学籍番号 : {}\n成績 : {}".format(
    stu_name[0], stu_dept[0], stu_num[0], stu_grade[0]))<br>

# indexが同じデータは一人のデータを意味するように処理しました。<br>
# もうちょっといいコードですが、ミスることが考えられます。<br>

# 最後にclassを利用し、一人のデータを論理的なオブジェクトにしてみます。<br>

class Student(object):<br>
&nbsp;&nbsp;def __init__(self, name, dept, num, grade):<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.name = name<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.dept = dept<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.num = num<br>
&nbsp;&nbsp;&nbsp;&nbsp;self.grade = grade<br>
<br>
&nbsp;&nbsp;def __repr__(self):<br>
&nbsp;&nbsp;&nbsp;&nbsp;return self.name<br>
<br>
<br>
students = []<br>
students.append(Student("藤井", "医学", "20-2-002-0002", 4.5))<br>
students.append(Student("川崎", "社会", "19-3-003-0003", 3.4))<br>
students.append(Student("中村", "化学", "18-4-004-0004", 3.8))<br>
<br>
print(students)<br>
print(students[0].dept)<br>
</div>

<br>