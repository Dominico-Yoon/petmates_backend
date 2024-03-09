# 🐶 PetMate 게시판

>  구름 교육에서 진행한 팀 프로젝트입니다.
>  "반려인들을 위한 다양한 기능을 하나의 서비스에서 제공하자" 라는 목적으로 만든 펫시터 프로그램 입니다.
>
> **진행 기간은 [ 24.01.02 ~ 24.03.08 (10주) ]** 입니다.
>
>

### 🐶 목차

1. [내가 맡은 주요 기능](#내가-맡은-주요-기능)
    + [게시글 리스트 조회](#1-게시글-리스트-조회)
    + [게시글 리스트 조건 검색](#2-게시글-리스트-조건-검색)
    + [펫시터 지원하기](#3-펫시터-지원하기)
    + [펫시터 지원 글 보기](#4-펫시터-지원-글-보기)
    + [끌어올리기](#5-끌어올리기)
    + [펫시터 리뷰 보기](#6-펫시터-리뷰-보기)
2. [추가 구현하고 싶은 기능들](#추가-구현하고-싶은-기능들)
3. [사용한 기술 스택 및 라이브러리](#사용한-기술-스택-및-라이브러리)
4. [ERD 데이터 모델링](#erd-데이터-모델링)
5. [Trouble Shooting](#trouble-shooting)
6. [프로젝트를 하며 느낀 점](#프로젝트를-하며-느낀-점)

## [내가 맡은 주요 기능]

### 1. 게시글 리스트 조회

- [x] 실명, 휴대전화번호(10~11자리), 비밀번호를 입력해 회원가입 할 수 있다.
- [x] 전화번호는 중복 불가하다.

### 2. 게시글 리스트 조건 검색

- [x] 회원가입 시 사용한 휴대전화번호와 비밀번호로 로그인 할 수 있다.
- [x] 회원가입과 로그인을 제외한 BankSSun 프로그램의 모든 기능은 로그인 후 사용 가능하다.

### 3. 펫시터 지원하기

- [x] 계좌를 생성, 삭제 할 수 있다.\
  계좌 생성은 `SSun 은행`의 계좌만 가능하다.\
  다른 은행의 계좌를 등록할 때는 이미 생성되어있는 계좌라고 가정한다.
- [x] 삭제 시 데이터베이스에서 삭제되지 않고 삭제 여부가 저장된다.
- [ ] 계좌 목록 조회 요청 시 본인이 소유한 SSun 은행 계좌목록을 확인할 수 있다.\
  (계좌번호, 잔액이 표시된다.)

### 4. 펫시터 지원 글 보기

- [x] 타 은행 계좌로의 송금을 위해서는 먼저 계좌(11~13자리)가 등록되어 있어야 한다.\
  은행명, 소유주명, 계좌번호를 이용해 등록할 수 있다.\
  등록할 수 있는 은행은 `Wind`, `Rain`, `Cloud`, `Snow` 4곳이다.\
  모든 은행의 계좌번호는 중복되지 않는다.

### 5. 끌어올리기

- [ ] 계좌번호와 은행명을 이용해 계좌를 검색할 수 있다.\
  이때, 이미 생성 또는 등록된 계좌만 검색할 수 있다.\
  계좌를 검색하면 은행명, 계좌번호, 계좌 소유주명을 확인할 수 있고, 본인의 계좌는 잔액이 표시된다.

### 6. 펫시터 리뷰 보기

- [x] 원하는 계좌에 현금을 입금할 수 있다. 입금 시 입금자명을 입력해야한다.
- [x] 자신의 계좌에 있는 금액을 출금할 수 있다. 출금 시 출금자명을 입력해야한다.

## [추가 구현하고 싶은 기능들]

> 추후 여유가 된다면 구현해보고 싶은 기능입니다.

- [ ] 회원가입 시 전화번호 SMS 인증
- [ ] 계좌 비밀번호 - 계좌 생성 시 비밀번호를 등록해야 하고, 출/송금시 비밀번호를 입력해야 한다.

## [사용한 기술 스택 및 라이브러리]

<div align=center> 

<img height="30" src="https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=Spring&logoColor=white"/>
<img height="30" src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=java&logoColor=white"/>
<img height="30" src="https://img.shields.io/badge/MySql-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
<br/>
<img height="30" src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white"/>
<img height="30" src="https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=Postman&logoColor=white"/>
<img height="30" src="https://img.shields.io/badge/GitHub-black?style=flat-square&logo=GitHub&logoColor=white"/>

</div>

- 라이브러리 : Spring Web, Spring Data JPA, Lombok, Spring Security, JWT, Spring-Data-Envers

## [ERD 데이터 모델링]

![img](./docs/ERD%200730.png)

## 프로젝트 구조

## api docs

## Installation

