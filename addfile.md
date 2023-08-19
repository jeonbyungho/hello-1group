# 🐸 Github에 파일 올리기

## ✨로컬 저장소에 파일 추가

```
> git add addfile.md
> git add README.md
```

## ✨파일의 상태 확인
```
> git status
   On branch main
   Changes to be committed:
   (use "git restore --staged <file>..." to unstage)
         modified:   README.md
         new file:   addfile.md

   Changes not staged for commit:
   (use "git add <file>..." to update what will be committed)
   (use "git restore <file>..." to discard changes in working directory)
         modified:   README.md
```
- `On branch main` : `main` 브런츠에서..
- `Changes to be committed:`
   - add 명령어가 반영된 파일 목록.
- `Changes not staged for commit:`
   - add 명렁어가 반영이 안 되어 있는 파일.

## ✨로컬 저장소에 반영.
```
> git commit -m "커밋 메시지 작성"
   [main 65affcd] 커밋 메시지 작성
   2 files changed, 66 insertions(+), 1 deletion(-)
   create mode 100644 addfile.md
```
- commit까지 해줘야 로컬 저장소에 파일이 추가되거나 수정된 내용들이 제대로 반영이 된다.

## ✨로컬 저장소에 반영된 데이터를 원격 저장소에 올리기
```
> git push origin main
   Enumerating objects: 6, done.
   Counting objects: 100% (6/6), done.
   Delta compression using up to 16 threads
   Compressing objects: 100% (3/3), done.
   Writing objects: 100% (4/4), 1.83 KiB | 1.83 MiB/s, done.
   Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
   To https://github.com/jeonbyungho/hello-1group.git
      4fae155..65affcd  main -> main
```
- `main` 브런치에 반영된 데이터를 원격 저장소에 올려보냄.