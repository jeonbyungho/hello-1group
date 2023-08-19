# hello-1group

[Git 공식 튜토리얼](https://git-scm.com/book/ko/v2)

## GitHub 우리 조 인원 초대해보기
[🌐참고 링크](https://docs.github.com/ko/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository)

[🌐참고 링크](https://docs.github.com/ko/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/managing-teams-and-people-with-access-to-your-repository)

![저장소 설정 메뉴](./img/collaborators.jpg)

## 브런치 생성

```
> git branch testing
```

## 브런치 이동
```
> git checkout testing
Switched to branch 'testing'
```

## 다른 브런치와 병합
```
> git merge testing
Updating ...
```

## 브런치 목록 전체 보기
```
> git branch
* main
  testing
// *  현 브런치임을 표시.
```

---
# 🐸 Github 저장소 받아오기

## ✨git 저장소 생성.

```
> git init
Initialized empty Git repository in C:/{...}/.git/
```
- 지정된 폴더에 `.git/` 폴더가 생성됨.
  - `.git/` 는 숨김 처리된 폴더라서, 윈도우상 폴더 옵션에서 숨김 파일, 폴더 보기 옵션을 체크 해줘야 보입니다.

## ✨원격 저장소와 로컬 저장소간 연결.
```
> git remote add origin https://github.com/jeonbyungho/hello-1group.git
```
- 여기서 원격 저상소는 git hub를 의미함.

## ✨깃 저장소 설정 확인.
```
git config --list --local

core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
remote.origin.url=https://github.com/jeonbyungho/hello-1group.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*
```
- `remote.origin`부분을 체크해주시면 됩니다.
- 확인 절차라서 꼭 해줄 필요는 없습니다.

## ✨원격 저장소에서 있는 데이터를 로컬 저장소에 가져오기.
```
> git pull origin
remote: Enumerating objects: 45, done.
remote: Counting objects: 100% (45/45), done.
remote: Compressing objects: 100% (28/28), done.
remote: Total 45 (delta 15), reused 38 (delta 11), pack-reused 0
Unpacking objects: 100% (45/45), 113.17 KiB | 1.51 MiB/s, done.
From https://github.com/jeonbyungho/hello-1group
 * [new branch]      cat        -> origin/cat
 * [new branch]      dog        -> origin/dog
 * [new branch]      main       -> origin/main
 * [new branch]      testing    -> origin/testing
You asked to pull from the remote 'origin', but did not specify
a branch. Because this is not the default configured remote
for your current branch, you must specify a branch on the command line.
```
- 원격 저장소에 있는 데이터를 `origin`에 모두 반영됩니다.
- 어떤 브런치에서 파일들을 가져올 지, 선택하지 않았기 때문에, 로컬 저장소에 파일은 추가되지 않음.

## ✨특정 브런치에 있는 파일들을 가져오기.
```
> git pull origin main
From https://github.com/jeonbyungho/hello-1group
 * branch            main       -> FETCH_HEAD
```
- 위에 예시에는 `main`브런치를 가져와서 반영했습니다.


# 🐸Git hub에 파일 올리기

## [링크](addfile.md)
