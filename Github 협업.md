
Github 협업
=
> git branch, fork에 대해서 알아보고 Github 협업의 방법에 대해 학습합니다. 장고 프로젝트를 push하기 위해 .gitignore를 작성 해 보도록 하겠습니다.

[TOC]
 


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

  다른걸 협업할땐 각자 개발하는 내용이 다르기 때문에 **충돌**이 일어날 수 있음. 따라서 `git branch (name)`으로 각각의 독립된 브랜치를 활용
  => 이후 merge 할 때, pull하고 충돌이 일어나는지 확인 후에 합치는 과정을 거침

## Github을 이용한 협업

1. 원격 repo 생성
2. 팀원을 Collaborator로 추가
3. 초기 프로젝트 push
4. 팀원들의 로컬에 프로젝트 pull
5. 팀원 각자의 브랜치 생성하여 작업
6. 브랜치에 작업한 내용을 push
7. Master와 merge하기 전 pull request
8. PR확인 후 Master와 merge

### pull request 요청
Github 웹 - pr 탭에서 사용 가능
* base (어디에 적용할지) -> compare (어디서 적용할지)
: 자동으로 두개의 차이 보여줌
* Create pull request 눌러야 pr이 됨
* repo 판 사람이나 팀장이 merge pull request하면 merge됨

## Fork를 이용한 협업
Collaborator가 아닌 상태에서 pr하기

1. 작업하고싶은 repo fork 해오기 (복사)

  **Spoon-Knife**: github가 제공하는 fork test용 repo
2. 로컬에서 작업
3. 변경사항 **자신의 브랜치에** push
4. 원본 repo 소유자에게 pr 요청
5. 원본 repo 소유자가 승인하여 merge 하면 자동으로 collaborator 추가됨

### fork 실습
* [4923/Spoon-Knife: forked repo](https://github.com/4923/Spoon-Knife)
* [pull request](https://github.com/octocat/Spoon-Knife/pull/21067)