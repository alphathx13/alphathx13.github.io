---
title: Github Page 만들기
date: 2024-04-26 12:00:00 +0800
categories: [Github Pages]
tags: [github, github pages, repo, commit, push]
math: false
mermaid: true
image:
  path: assets/img/etc.jpg
---

<hr style="border:1px solid white">
[github, github pages, repo, commit]

## 로컬 폴더내에 깃허브 repo 연동하기
```bash
git clone [깃허브 페이지 주소]
```
> ![1](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/01608b96-17b4-4af3-8e7a-a3649f00ae3b){: .normal}
- 로컬 저장소내 저장하려는 위치에 repo 연동

<hr style="border:1px solid white">

```bash
git pull
```
- 만약 로컬저장소의 변동사항을 원격저장소 내용으로 되돌리고 싶을때

<br/><br/>

## 로컬 폴더내 변경사항을 깃허브 repo에 업로드
```
git add -A
```
> ![2](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/6905924c-25b8-482e-a689-4c4929cd43d5){: .normal}
- -A는 변동사항 전부를 업로드

<br/><br/>

## commit
```bash
git commit -m "aaaa"
```
> ![3](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/fccebfce-5e46-4317-a6f1-1d5ec2f435e3){: .normal}
- 처음 commit을 하려하면 업로드 유저의 정보가 저장되어 있지 않으므로 email과 이름을 등록
- 이후 commit의 메시지를 넣어주고 commit

<br/><br/>

## push
```
git push
```
> ![4](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/fe3ccc82-9e7e-4b35-af4e-b35d3b0119db){: .normal}
- 등록한 커밋을 확정