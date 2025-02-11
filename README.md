# ALE6IX PROJECT

## oo 프로젝트 Front-end/Back-end 소개

- 해외 유명 디자이너 브랜드 ALESSI (http://alessi.co.kr) 를 클론 코딩 하였습니다.
- 프로젝트 내의 짧은 기간동안 세션 복습과 새로운 기능을 도전해 보고자 디자인은 클론코딩 하였고 기능을 구현하는 데에 중점을 두었습니다.
- 개발은 최소한의 라이브러리를 사용하여 직접 구현하였고 영상에서 보여지는 부분 모두 Fetch함수와 api를 이용하여 백엔드와 통신하여 작업하였습니다.

### 개발 인원 및 기간

- 개발기간 : 2022/8/29 ~ 2022/9/8
- 개발 인원 : 프론트엔드 4명, 백엔드 2명
- [백엔드 github 링크](https://github.com/wecode-bootcamp-korea/justcode-6-1st-ale6ix-back)

### 프로젝트 선정이유

- E-commerce는 필요한 부분을 컴포넌트화하여 섹션을 나누거나 fetch를 이용하여 api통신으로 데이터를 주고 받는등
  지금까지 학습한 부분을 각자 맡은 페이지내에서 복습할 수 있고 새로운 기능을 추가로 학습할 수 있기에 선정하게 되었다.

### 데모 영상(이미지 클릭)

[![home](https://velog.velcdn.com/images/ch00ng10000/post/3ff906f7-d6ea-43a6-92f1-fc37b06e3eae/image.png)](https://youtu.be/X2f3YSx6h0Q)

<br>

## 적용 기술 및 구현 기능

### 적용 기술

> - Front-End : React.js, sass, slick, react-modal
> - Back-End : Python, Django web framework, Beautifulsoup, Selenium, Bcrypt, My SQL
> - Common : KAKAO social login, AWS(EC2,RDS), RESTful API



### 구현 기능👇

### 회원가입
![회원가입](https://user-images.githubusercontent.com/103557910/190312824-5f678c11-07ab-4eb7-a22d-3ae1ad4d2039.gif)
- 아이디 중복 검사
- 휴대폰 인증번호받기 구현(휴대전화 10자리 이상 때만 '인증번호받기' 버튼 활성화)
- 이용약관 체크박스 구현
- 회원가입 완료 페이지에 DB에 등록된 유저의 정보(ID, NAME, EMAIL) 확인 section 구현
### 로그인
![로그인](https://user-images.githubusercontent.com/103557910/190312797-298df332-6584-44a3-9ef0-a1e9aa375f2b.gif)
- 회원여부 확인
- 로그인 성공 시 유저의 TOKEN 로컬스토리지에 저장
- 로그인 상태에서 nav header에 유저의 ID 나타나게 구현
- 로그아웃 시 main page로 이동 및 로컬스토리지에 있는 token 삭제
### 메인페이지
- 이미지 슬라이드 구현(라이브러리 사용x)
- 중복 Title컴포넌트 화
- Magazine 목데이터 사용
- 데이터 받아서 섹션 제품 구현
### 제품 페이지
### 제품 상세페이지
- 수량(+,-)버튼 구현, 상품수량이 상품재고보다 많아지면 재고 알림창 구현
- POST 요청 : 수량,제품번호 post 통신
### nav,footer
### 검색창
- GET : 서버로부터 query문 사용하여 값을 가져옴
- GO!버튼 클릭 or Enter 검색한 상품들이 나오게 구현
### 장바구니
- 조건부 렌더링으로 상품이 없을때 '장바구니 가 비어있습니다' 문구 구현
- GET : 장바구니에 담긴 상품들 화면에 렌더링
- PATCH : 장바구니 상품 수량변경 -> 유저 아이디,상품 아이디,변경된 수량을 담아서 요청 
- DELETE : 개별 상품 삭제, 체크된 상품 삭제, 전체삭제(장바구니 비우기)

## 개인별 구현 사항

#### 김충만/FE
- 회원가입 페이지
- 로그인 페이지
- NAV HEADER 통신 

#### 서지원/FE
- 메인페이지 레이아웃
- 제품 상세페이지 POST 요청
- 장바구니 레이아웃, 기능구현 및 통신
- 검색창 레이아웃, 기능구현 및 통신
 ---

<br>

## 팀원 github주소

[김충만/FE](https://github.com/kimchoongman)
<br>
[서지원/FE](https://github.com/tjwldnjs123)

## Reference

- 이 프로젝트는 [알레시](http://alessi.co.kr) 사이트를 참조하여 학습목적으로 만들었습니다.
- 실무수준의 프로젝트이지만 학습용으로 만들었기 때문에 이 코드를 활용하여 이득을 취하거나 무단 배포할 경우 법적으로 문제될 수 있습니다.
- 이 프로젝트에서 사용하고 있는 사진 모두 알레시 코리아의 동의하에 작업되었습니다.
