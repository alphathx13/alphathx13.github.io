---
title: Git / Github
date: 2024-04-20 12:00:00 +0800
categories: [Github]
tags: [github, git, repository, repo, commit, push]
math: false
mermaid: true
image:
  path: assets/img/github.png
---

<hr style="border:1px solid white">

## Git / Github ?
```
- Git : 형상 관리 도구 중 하나로, 변경사항을 추적하고, 
여러 사용자들 간에 작업을 조율하기 위한 분산 버전 관리 시스템
- Github : 버전 관리와 협업을 위한 코드 웹 호스팅 플랫폼

- PC 내의 작업 폴더 : 로컬저장소
- Github에서 생성한 폴더 (Repository) -> 원격저장소

- 로컬저장소와 원격저장소간의 연결
  -> 소스코드 관리를 편하게 할수 있음
```
- 개발은 혼자 진행하는것이 아니기 때문에, 협업 및 버전관리를 제공하는 Github를 활용

- Git 설치 : [다운로드](https://git-scm.com/downloads)

<br/><br/>

## Github에 repository 만들기
> ![111](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/a7c5a150-7aa6-47d8-8422-25440340c9eb){: .normal} ![222](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/1dbb519a-ee4e-4b7b-a473-fac67bc23915){: .normal}
- github에서 새로운 repo를 생성
- 해당 repo의 주소 확인

<br/><br/>

## git 기본셋팅
```bash
git init
```
- 연결하려는 폴더안에서
- git init : 해당 폴더를 git 관련 작업으로 사용하기 위한 기본 작업 -> 최초 한번만 하면됨

```bash
git remote add origin [repo의 주소]
```
- 현재 폴더와 github의 repo를 연결하는 작업

```bash
vim .gitignore
```
```vim
.classpath
.project
.settings
.gitignore
bin
build
```
- repo에 업로드하지 않을 파일목록 생성

```bash
git config --global user.name
git config --global user.email
```
- 현재 github 계정 / email 확인
- git 최초 설치나 여러사람이 사용하는 컴퓨터에서 commit 진행시 확인해야함
- 만약 commit 하려는 github 계정이 아니라면 아래와 같이 수정

```bash
git config --global user.name [본인 github 계정명]
git config --global user.email [본인 email 주소]
```
- user.name 및 user.email 수정

<br/><br/>

## commit 하기
```bash
git status
git add .
git commit -m "[커밋명]"
git push origin master
```
- 로컬저장소의 파일들을 commit

<hr style="border:1px solid white">

>!![111](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/4131ece8-0ef5-46d7-8fb2-acbe718b0057){: .normal}
- 만약, git push 에서 다음과 같은 에러가 발생할경우, set-url 을 수정

>![222](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/dd296dbb-3d3e-4250-95c9-c9335281eb06){: .normal}
- 정상적으로 push 됨을 확인

<hr style="border:1px solid white">

<br/>

![555](https://github.com/alphathx13/alphathx13.github.io/assets/163115993/3e86738a-54b1-4499-b0fe-d968eac1c832){: .normal}
- repo에서 commit 사항을 확인