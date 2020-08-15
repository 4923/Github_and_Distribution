[TOC]

# Github 협업
> git branch, fork에 대해서 알아보고 Github 협업의 방법에 대해 학습합니다. 장고 프로젝트를 push하기 위해 .gitignore를 작성 해 보도록 하겠습니다.

 


## 자주쓰는 Git 명령어

  `git init`

  git 저장소를 초기화

  `git add .`

  폴더의 변경된 모든 파일 staging area에 올리기

  `git commit -m "(커밋에대한설명)"`

  유사시 돌아갈 수 있는 저장소의 체크포인트 생성

  `git remote add origin (원격repo주소).git`

  원격저장소 (remote repo) 연결

**자주쓰는 명령어 도식화**

![자주쓰는 명령어 도식화](https://github.com/4923/Github_and_Distribution/blob/master/%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C-%EB%A1%9C%EC%BB%AC.png)

`git branch (브랜치이름)`

새로운 브랜치를 생성

브랜치: 한 repo 안에서 용도에 따라 저장소를 나누는 것 (ex 출시할 브랜치, 기능을 개발할 브랜치 등등)

`git checkout (브랜치이름)`

해당 브랜치로 이동

`git push origin (브랜치이름)`

원결저장소의 특정 브랜치에 프로젝트 저장

`git pull origin 브랜치`

원격저장소의 특정 브랜치에서 변경사항 pull/내려받기

`git clone (원격저장소 url).git`

원격 저장소에 있는 파일 전체 복사 (* 자주사용함!)

`git status`

git 저장소의 현재 상태 확인
staging area에 올라오지 않은 파일이 있는지, 어느 브랜치에 있는지 등등을 출력

**협업과정 도식화**
![협업과정 도식화](https://github.com/4923/Github_and_Distribution/blob/master/%ED%98%91%EC%97%85%EA%B3%BC%EC%A0%95.png)



