### 🎁 My Profile
> ### [LinkedIn Profile (Chang-Seong Kim)](https://www.linkedin.com/in/chang-seong-kim-7826142a0/)

<br>
<br>

## ✅ 프로젝트 소개
> ### 1. [KimLibrary_STS3](https://github.com/Kim-src/KimLibrary_STS3)
> - 개발 환경 : Spring Tool Suite 3
> - 개발 목적 : MVC 패턴의 Legacy Project 웹 개발 경험 및 STS3 활용 경험 습득
> - 개발 내용 : KimLibrary 도서관 웹 페이지 제작 및 도서 대여자 관리
> - 개발 역량 : STS3 활용, M-V-C 구축, Tomcat 서버 연동, 외부 라이브러리 관리, DB 생성

<br>

## 🚀 개발 현황 : KimLibrary (현재 ver. 0.5.0)
> - v0.3.0 :  
>   A. 프로젝트 기획 및 개발 환경 구축 (2024-01-19)  
>   B. 고객 목록 및 도서 대여 현황 데이터베이스 구축 (2024-01-19)  
> - v0.5.0  
>   A. MVC 중 View 및 Controller 구축 (2024-01-24)  
>   B. 브라우저에 웹 페이지 구현 (2024-01-24)  
> - v0.7.0  
>   A. MVC 중 Model 구축  
>   B. 구축된 Model과 데이터베이스 연동  
>   C. 구현된 웹 페이지의 입력 데이터와 데이터베이스 연동  
>   D. (현재 Hibernate 호환 문제로 인한 개발 중지)  
> - v1.0.0  
>   A. AWS를 이용하여 KimLibrary_STS3 웹 배포

<br>

#### <p align="right">Date : January 24, 2024</p>

## 🔔 KimLibrary_STS3 : ver. 0.5.0
### 📌 구축된 View 및 Controller
> - ### [KimLibrary_STS3_v0.5.0]()
> - [View]() : KimLibrary_STS3/src/.../views
> - [Controller]() : KimLibrary_STS3/src/.../java?

<br>

### 📌 크롬 브라우저에 구현된 웹 페이지
#### A. 홈페이지 : [index.jsp]()
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/50e489f9-aa51-44b6-9369-f3a826894c86" width="500px"></p>

#### B. 고객정보 등록 페이지 : [register.jsp]()
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/e991d72a-7870-440d-8b35-077c4052e616" width="500px"></p>

#### C. 고객목록 조회 페이지 : [list.jsp]()
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/469a39d7-ae4d-463a-9086-a7e9eb7fa4fd" width="500px"></p>

#### D. 고객정보 수정 페이지 : []()
<p align="center"><img src="" width="500px"></p>

#### E. 대여목록 조회 페이지 : [rentallist.jsp]()
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/cfbd68b7-84e6-42b2-a60d-f6c821eaf2b6" width="500px"></p>

#### F. 대여금액 조회 페이지 : [rentalamount.jsp]()
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/8bde634f-8bcf-4cf1-abb3-101b27be4658" width="500px"></p>

<br>

#### <p align="right">Date : January 19, 2024</p>

## 🔔 KimLibrary_STS3 : ver. 0.3.0
### 📌 프로젝트 개발 환경
> - Spring Tool Suite 3.9.17
> - Java Development Kit 11
> - Tomcat 9.0.52
> - MySQL 8.0.33

<br>

### 📌 프로젝트 기획
#### A. 홈페이지 : [index.jsp]()
> - 도서관 소개
> - "고객정보 등록" 페이지 접근을 위한 UI 구성
> - "고객목록 조회" 페이지 접근을 위한 UI 구성
> - "고객정보 수정" 페이지 접근을 위한 UI 구성
> - "대여목록 조회" 페이지 접근을 위한 UI 구성
> - "대여금액 조회" 페이지 접근을 위한 UI 구성
> - "홈페이지" 접근을 위한 UI 구성

#### B. 고객정보 등록 페이지 : [register.jsp]()
> - 도서 대여자 정보 입력을 위한 관리자 필드 구성
> - 입력된 고객 정보는 데이터베이스(Member_tbl)에 삽입
> - "고객이름" 입력을 위한 필드 구성
> - "전화번호" 입력을 위한 필드 구성
> - "이메일" 입력을 위한 필드 구성

#### C. 고객목록 조회 페이지 : [list.jsp]()
> - 데이터베이스에 저장된 고객 정보 표시
> - "고객번호"는 "1000"부터 데이터베이스 저장 순서대로 부여
> - "고객번호"에 고객정보 수정 페이지 접근을 위한 UI 구성
> - "가입일자"는 데이터베이스 저장 일자로 부여
> - "고객등급"은 도서 대여 금액 총계에 따라 차등 부여

#### D. 고객정보 수정 페이지 : []()
> - 데이터베이스에 저장된 고객 정보 수정 필드 구성

#### E. 대여목록 조회 페이지 : [rentallist.jsp]()
> - 도서 대여자의 대여 정보 표시
> - 대여 정보는 데이터베이스(Rental_tbl)에 저장된 내용
> - "대여번호"는 도서 대여 발생년도의 대여 순서대로 부여("20240001"부터 부여)
> - "도서코드" 및 "대여금액"은 데이터베이스(BookInfo_tbl)에 저장된 내용
> - "대여일자"는 도서 대여 발생일
> - "반납일자"는 도서 수령 발생일
> - "대여일자" 및 "반납일자"는 관리자가 조회 페이지에서 날짜 선택기를 이용해 입력 가능

#### F. 대여금액 조회 페이지 : [rentalamount.jsp]()
> - 도서 대여자의 총 대여 금액 표시
> - "고객번호" 및 "고객이름"은 데이터베이스(Member_tbl)에 저장된 내용
> -
> - 도서 대여자의 "고객등급"

> - 고객별 총 도서 대여 금액에 따라 고객 등급 구분

<br>

### 📌 도서 대여자 목록 및 대여 현황 데이터베이스
#### 🎯 Member_tbl : 고객 정보 관리 DB 구성
> - cust_no : 고객의 일련번호 / ```int``` / ```Primary Key```
> - cust_name : 고객의 이름 / ```varchar(20)```
> - phone : 고객의 전화번호 / ```varchar(20)```
> - join_date : 고객의 가입일자 / ```datetime``` / ```now()```
> - cust_email : 고객의 이메일 / ```varchar(50)```
> - grade : 고객의 등급 / ```varchar(20)```
#### 🎯 Rent_tbl : 고객 정보 및 도서 대여 정보 관리
> - cust_no : 고객의 일련번호 / ```int```
> - rent_no : 도서의 대여번호 / ```int``` / ```Primary Key```
> - book_code : 도서의 일련번호 / ```varchar(20)```
> - rent_price : 도서의 대여금액 / ```int```
> - rent_date : 도서의 대여일자 / ```datetime``` / ```now()```

<br>

***

<br>
<br>
<br>
