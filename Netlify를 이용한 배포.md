# Netlify를 이용한 배포

## 정적페이지, 동적페이지
* 정적페이지 : html로만 이루어진 페이지. 시간이 지나도 변하지 않음
* 동적페이지 : 백엔드언어(Django) 등을 사용해서 시간이나 사용자의 요청에 따라 달라지는 페이지 

## Netlify 배포과정
1. 코드 업로드
2. Github 연동 호스팅 (인터넷에서 접근할 수 있게 한다)

### [Netlify 페이지](https://www.netlify.com)
1. Create a new site
2. Install Netlify
3. Netlify 설치할 repo 선택
4. Continuous Deployment -> provider로 github 선택
5. repo 선택 (3단계에서 netlify가 설치된 repo만 선택할 수 있음)
  * Basic build settings 추가적으로 설정하는 부분이라 만지지 않음.
6. Deploy Site
  상태가 Published로 뜨고, url 들어가면 repo가 뜬다.
  
    근데 지금은 html 올려둔게 없어서 Page not find로 뜨나? => 안되는데? 검색해보니까 뭘 덜했나본데 index.html로 해야하나???


