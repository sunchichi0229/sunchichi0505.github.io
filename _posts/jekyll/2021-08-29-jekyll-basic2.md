---
layout: post
current: post
cover:  assets/built/images/snoopy.jpeg
navigation: True
title: Jekyll講座(2) - ブログ更新 
date: 2021-08-28 16:40:00
tags: [jekyll]
class: post-template
subclass: 'post tag-python'
author: sunchichi0229
---

<自らJekyllを作った場合>

1. Githubに「Sign in」します。

2. New Repositoriesを作成します。

- Repositoryの名前は「GitのUsername.github.io」にします。

3. GithubからCloneしたHTTPSをVSCodeなどのEditorで実行します。
4. Editorに自分で作成したJekyllの内容をCOPYします。
5. 新たにターミナルを開きます。そして、下記の内容を入力します。

- a) git status (Repositoryの現状況を確認)
- b) git add . (LocalにあるすべてのファイルをStaging Areaに入れる)
- c) git commit -m "残したいメッセージ"(RepositoryにすべてのファイルをCommit)
- d) git push -u origin main(originというRepositoryのmain branchにpush)
