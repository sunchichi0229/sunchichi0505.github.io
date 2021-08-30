---
layout: post
current: post
cover:  assets/built/images/snoopy.jpeg
navigation: True
title: Jekyll講座(2) - ブログ更新 
date: 2021-08-28 16:40:00
tags: [jekyll]
class: post-template
subclass: 'post tag-jekyll'
author: sunchichi0229
---

<自らJekyllを作った場合><br>
  
1. Githubに「Sign in」します。<br>    
<br>
2. New Repositoriesを作成します。<br> 
- Repositoryの名前は「GitのUsername.github.io」にします。<br>  
<br>
3. GithubからCloneしたHTTPSをVSCodeなどのEditorで実行します。<br>
<br>
4. Editorに自分で作成したJekyllの内容をCOPYします。<br>
<br>
5. 新たにターミナルを開きます。そして、下記の内容を入力します。<br>   
- a) git status (Repositoryの現状況を確認)<br>   
- b) git add . (LocalにあるすべてのファイルをStaging Areaに入れる)<br>   
- c) git commit -m "残したいメッセージ"(RepositoryにすべてのファイルをCommit)<br>   
- d) git push -u origin main(originというRepositoryのmain branchにpush)<br>   
