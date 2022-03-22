# todo-application
To Do List를 생성/조회/수정/삭제할 수 있는 웹 애플리케이션의 백엔드 프로젝트입니다.  
JWT를 통해 사용자를 인증하고, 사용자별로 자신의 To Do List를 관리할 수 있습니다.  
각 기능은 REST API로 구현하여, 프론트엔드 서버의 request 에 대하여 JSON 형식으로 응답합니다.  
<br>

## 기능
### 1. To Do 생성/조회/수정/삭제
로그인한 사용자의 To Do를 조회하여 목록을 보여줍니다.  
사용자가 To Do를 생성, 조회, 삭제하면 DB에 해당 내용을 반영합니다.  

### 2. 회원 가입
회원가입 시, BCryptPasswordEncoder 를 통해 비밀번호를 암호화하여 저장합니다.

### 3. 회원 로그인 / 로그아웃
로그인 시, JWT을 통해 인증합니다.  
프론트엔드에서 발급받은 토큰을 로컬 스토리지에 저장하고, 로그아웃 시에 로컬 스토리지에서 토큰을 지웁니다.

## Spring Data JPA
* JpaRepository를 상속하여 CRUD 기능을 구현하였습니다.
<br><br><br>

## JWT를 이용한 인증 - 스프링 시큐리티
* jjwt 라이브러리를 이용하여 토큰 생성 및 인증합니다.
  <br><br><br>


## 프론트엔드 연동
CORS (Cross-Origin Resource Sharing)
* 리액트 프론트엔드 서버에서 백엔드 서버로 HTTP 요청 시 문제가 발생하였습니다.
* WebMvcConfigurer 인터페이스를 구현하여 해결하였습니다.
  <br><br><br>

## AWS 배포
* React 기반의 프론트엔드 서버와 연동하여 AWS의 Elastic Beanstalk를 통해 배포하였고, 
  프론트엔드 소스코드는 아래 링크를 통해 확인할 수 있습니다.
  <br><br><br>


참고 서적: React.js, 스프링 부트, AWS로 배우는 웹 개발 101
* https://github.com/fsoftwareengineer/todo-application
