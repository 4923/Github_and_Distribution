> Github 소개와 사용을 위한 환경설정을 해 봅니다. 그리고 첫 레포지토리를 생성해 보고, 첫 푸시를 해 보도록 하겠습니다.

## Github란?
**git + hub (git이 모여있는 곳)**
 & 개발자 포트폴리오를 겸함

* git이란?

  파일의 변천사를 저장하는 역할 (누가, 언제, 무엇을, 어떻게)

## Github의 명령어

1. git을 시작 (initiate)
  
    `git init`

2. github의 원격 repo와 연결

    `git remote add origin (repo URL)`

3. dir 안의 파일을 업로드 전 준비상태로 전환 (.은 모든 파일을 의미)
  
    `git add .`

4. 커밋
  
    `git commit -m "원하는 내용"`
  
    -m : 커밋 내용을 적겠다

5. 원격 repo로 push
  
    `git push origin master`
