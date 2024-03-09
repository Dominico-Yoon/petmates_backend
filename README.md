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
2. [사용한 기술 스택 및 라이브러리](#사용한-기술-스택-및-라이브러리)
3. [ERD 데이터 모델링](#erd-데이터-모델링)
4. [Trouble Shooting](#trouble-shooting)
5. [프로젝트를 하며 느낀 점](#프로젝트를-하며-느낀-점)

## [내가 맡은 주요 기능]

### 1. 게시글 리스트 조회

- [x] Petsitter 테이블에 있는 모든 값들을 조회 해 준다.

### 2. 게시글 리스트 조건 검색

- [x] Query String으로 careType, serviceArea1(시 단위), serviceArea2(구 단위)를 통하여 조건에 맞는 값들을 조회 해 준다.

### 3. 펫시터 지원하기

- [x] Petsitter 테이블에 필수 값으로 들어가는 내용을 Request로 넣어주고\
      요청 값에 대해 이상이 없을 시, 지원을 성공적으로 저장해준다.

### 4. 펫시터 지원 글 보기

- [x] Petsitter 테이블에 있는 id값으로 PathVariable주어 id값인 글을 조회한다.

### 5. 끌어올리기

- [x] POST로 끌어올리기를 실행 하면\
      orderByDate를 끌어올리기 실행 한 날짜로 변경해준다.\
      그리고 게시글 조회를 orderByDate로 정렬한다.

### 6. 펫시터 리뷰 보기

- [x] Members 테이블에 id값인 petsitterId로 리뷰 조회시\
      그 글에 달린 리뷰를 조회 한다.


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
![image](https://github.com/Dominico-Yoon/petmates_backend/assets/142984862/d3bf8ec7-a833-42db-92af-9317a8ababdf)

## [Trouble Shooting]


## [프로젝트를 하며 느낀 점]
처음으로 개발을 진행하다 보니 생각 보다 많이 오래 걸렸다.
그리고 나만 코드를 잘짜면 되는게 아니고, 팀원들과 Git을 통하여 Commit, Push, Update를 하여 공유가 잘 되어서 오류가 없게 끔 해야 하는데 팀원들도 처음인 인원이 많아 여러 에러를 Trouble Shooting 오래 걸렸다.
JPA를 처음 사용해 봐서 Native Query를 사용해야 하는데 정확히 어떻게 사용하는지 몰라서 많이 헤매었다.
아직 많이 부족하여 JPA와 GIT에 대해 조금 더 공부해야 한다고 생각합니다.
