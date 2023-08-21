# Board
#### ⚪ About Project
* ##### 인증된 사용자가 작성한 게시글은 사용자에게 종속된 접근권한 분리형, Postgresql를 이용한 게시판 서비스
* ##### 게시글생성, 조회, 전체조회, 수정, 삭제 API 게시글 모듈, 관계형 데이터 베이스인 Postgresql로 권한분리 구현
* ##### 유저생성, 조회, 전체조회, 수정, 삭제, 전체삭제기능 API 사용자 모듈
* ##### 로그인, 회원가입 API 인증모듈에서 PassPort,Jwt-Strategy, Jwt accessToken을 사용한 인증 구현

* * * *
#### ⚪ Usage
<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

* * *
#### ⚪ Built With
<img alt="Html" src ="https://img.shields.io/badge/NestJS-E0234E.svg?&style=for-the-badge&logo=NestJS&logoColor=white"/> <img alt="Html" src ="https://img.shields.io/badge/TypeScript-3178C6.svg?&style=for-the-badge&logo=TypeScript&logoColor=white"/>

* * *
#### ⚪ Getting Strated
* ##### Prerequisites: npm, node, Postgresql
```bash
git clone https://github.com/MpqM/NestJS_Board.git
cd {project}
npm install
# development
npm run start
# watch mode
npm run start:dev
# production mode
npm run start:prod
# unit tests
npm run test
# e2e tests
npm run test:e2e
# test coverage
npm run test:cov
```

* * *
#### ⚪ Description 
* ##### user
  * ##### createUser: 사용자 엔티티 생성 및 저장
  * ##### getUser: 주어진 이메일을 이용해 사용자 조회
  * ##### getAllUser: 모든 사용자 조회 후 반환
  * ##### updateUser: 주어진 이메일을 이용해 사용자 조회 후 사용자 객체 비밀번호 해시 후 업데이트
  * ##### deleteUser: 주어진 이메일을 이용해 사용자 삭제
* ##### board
  * ##### createBoard: 게시물 엔티티 생성 및 저장
  * ##### getBoard: 주어진 ID를 이용해 게시글 조회
  * ##### getAllBoard: 유저가 가진 게시글 조회
  * ##### updateBoard: 유저가 가진 게시글을 업데이트
  * ##### deleteBoard: 유저가 가진 게시글을 삭제
* ##### auth
  * #### register: getUser로 사용자 존재여부 확인, 비밀번호 해시화후 createUser에 주입해 사용자 등록
  * #### login: getUser로 사용자 존재여부 확인, 비밀번호 비교후 JWT accessToken 생성
* ##### PassPort: Jwt Strategy, src/auth/jwt.startegy.ts참조
* ##### 자세한 내용은 src/**/*.repository.ts주석, postman참조

* * *
#### ⚪ Roadmap & Realization & Study
* ##### PassPort와 JWT를 이용한 사용자 인증, Guard를 통한 핸들러 메서드에 전달전 검증
* ##### Class-validator, ValidationPipe를 통한 유효성 검증,
* ##### TypeORM 설정과 Entity를 통한 Postgresql 연동
* ##### User와 Board Entity간 관계형성으로 접근권한 분리
* ##### config 설정 패키지 사용, 예외처리
* ##### Custom Decorator, Query builder, looger, bcrypt 공부

* * *
#### ⚪ Writer
* ##### <span>okqkrwhdtjd@gmail.com
* <a href = "https://github.com/MpqM"><img alt="GitHub" src ="https://img.shields.io/badge/GitHub-181717.svg?&style=for-the-badge&logo=GitHub&logoColor=white"/></a> <a href = "https://MpqM.tistory.com/"> <img alt="Tistory" src ="https://img.shields.io/badge/Tistory-white.svg?&style=for-the-badge"/></a>

* * *
#### ⚪ Contributing
* ##### Fork the Project https://github.com/MpqM/NestJS_Board
* ##### Create your Feature Branch (git checkout -b feature/AmazingFeature)
* ##### Commit your Changes (git commit -m 'Add some AmazingFeature')
* ##### Push to the Branch (git push origin feature/AmazingFeature)
* ##### Open a Pull Request
