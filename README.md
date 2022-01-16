# todo-application
간단한 to do list를 생성/조회/수정/삭제할 수 있는 웹 애플리케이션의 백엔드 프로젝트입니다.
<br><br><br>

## 기능
1. to do 생성/조회/수정/삭제
2. 회원 가입
3. 회원 로그인
4. 회원 로그아웃
<br><br><br>

## Spring Data JPA
* JpaRepository를 상속하여 단순한 CRUD 기능 구현.
* (추가 예정) Pageable을 이용한 페이징 기능 구현.
<br><br><br>

## CORS (Cross-Origin Resource Sharing)
* 리액트 프론트엔드 서버에서 백엔드 서버로 HTTP 요청 시 문제가 발생.
* WebMvcConfigurer 인터페이스를 구현하여 해결.
<br><br><br>


## JWT를 이용한 인증 - 스프링 시큐리티
* jjwt 라이브러리를 이용하여 토큰 생성 및 인증.
<br><br><br>


참고 서적: React.js, 스프링 부트, AWS로 배우는 웹 개발 101
* https://github.com/fsoftwareengineer/todo-application
