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
>   1. 프로젝트 기획 및 개발 환경 구축 (2024-01-19)  
>   2. 고객 목록 및 도서 대여 현황 데이터베이스 구축 (2024-01-19)  
> - v0.5.0  
>   1. MVC 중 View 및 Controller 구축 (2024-01-24)  
>   2. 브라우저에 웹 페이지 구현 (2024-01-24)  
> - v0.7.0  
>   1. MVC 중 Model 구축  
>   2. 구축된 Model과 데이터베이스 연동  
>   3. 구현된 웹 페이지의 입력 데이터와 데이터베이스 연동  
>   4. (현재 Hibernate 호환 문제로 인한 개발 중지)  
> - v1.0.0  
>   1. AWS를 이용하여 KimLibrary_STS3 웹 배포

<br>

#### <p align="right">Date : January 24, 2024</p>

## 🔔 KimLibrary_STS3 : version 0.5.0
### 📌 크롬 브라우저에 구현된 웹 페이지
### A. 홈페이지 : index.jsp 
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/50e489f9-aa51-44b6-9369-f3a826894c86" width="500px"></p>

### B. 고객등록 페이지 : register.jsp
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/e991d72a-7870-440d-8b35-077c4052e616" width="500px"></p>

### C. 고객목록 조회 페이지 : list.jsp
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/469a39d7-ae4d-463a-9086-a7e9eb7fa4fd" width="500px"></p>

### D. 고객대여목록 조회 페이지 : rentallist.jsp
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/cfbd68b7-84e6-42b2-a60d-f6c821eaf2b6" width="500px"></p>

### E. 고객대여금액 조회 페이지 : rentalamount.jsp
<p align="center"><img src="https://github.com/Kim-src/Images/assets/150884526/8bde634f-8bcf-4cf1-abb3-101b27be4658" width="500px"></p>

<br>

#### <p align="right">Date : January 19, 2024</p>

## 🔔 KimLibrary_STS3 : version 0.3.0
### 📌 크롬 브라우저에 구현된 웹 페이지

### 📌 프로젝트 수행을 위한 프로그램
> - Java Development Kit 11
> - Spring Tool Suite 3.9.17
> - Tomcat 9.0.52
> - MySQL 8.0.33

<br/>

### 📌 프로그램 구현을 위해 필요한 DataBase
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

<br/>

### 📌 프로그램이 구현된 웹 페이지
#### 🎯 Home
> - 도서 대여 관련 페이지 및 UI 구성
> - "고객 등록" 버튼
> - "고객 목록 조회/수정" 버튼
> - "고객 대여 리스트" 버튼
> - "고객 대여 금액 조회" 버튼
> - "홈으로" 버튼
#### 🎯 "고객 등록" 페이지
> - 관리자가 고객의 정보를 생성할 수 있는 페이지
> - 고객번호 : 시스템이 부여한 고객의 일련번호
> - 고객이름 : 고객의 이름
> - 전화번호 : 고객의 전화번호
> - 이메일 : 고객의 이메일
> - 고객등급 : 총 대여금액에 따른 고객의 등급
#### 🎯 "고객 목록 조회" 페이지
> - 고객 등록 정보 및 가입일자를 조회할 수 있는 페이지
> - 고객별 고객번호에 따라 각 "고객 목록 수정" 페이지를 링크로 연결
#### 🎯 "고객 정보 수정" 페이지
> - 고객번호를 제외한 모든 항목에 대한 수정 가능
#### 🎯 "고객 대여 리스트" 페이지
> - 도서 대여 정보를 조회할 수 있는 페이지
> - 고객번호, 대여번호, 도서코드, 대여금액, 대여일자 등 조회 가능
#### 🎯 "고객 대여 금액 조회" 페이지
> - 도서 대여 이력이 있는 고객의 총 도서 대여 금액 조회 가능
> - 고객별 총 도서 대여 금액에 따라 고객 등급 구분

<br/>

***

<br/>
<br/>
<br/>
