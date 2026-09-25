<div align="center">

# Backend Developer

### Java & Spring Boot Backend Developer

기능 구현에 그치지 않고  
**데이터 정합성 · 테스트 · 배포와 운영까지 고려하는 백엔드 개발**을 지향합니다.

<br>

`Java` `Spring Boot` `Spring Security` `JPA` `MySQL` `Docker`

</div>

---

## About Me

- Java와 Spring Boot를 중심으로 백엔드 개발을 공부하고 있습니다.
- REST API 설계와 관계형 데이터베이스 모델링에 관심이 있습니다.
- 기능 구현뿐 아니라 데이터 정합성, 예외 처리, 테스트까지 함께 고려하려고 합니다.
- Docker와 CI 환경을 활용해 개발부터 배포까지 이어지는 흐름을 경험하고 있습니다.
- AI 기능을 기존 서비스에 안정적으로 연결하는 Backend Integration에도 관심이 있습니다.


---

## Tech Stack

### Backend

<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white"/>
  <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square"/>
</p>

### Database

<p>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
</p>

### Infrastructure & DevOps

<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white"/>
</p>

### AI & External Integration

<p>
  <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white"/>
</p>


---

## Featured Project

### 👔 입을래? — AI 기반 명품 활용 서비스

> 취향·보유 아이템·상황 데이터를 연결해  
> 명품의 구매 전 판단부터 착용·관리까지 이어주는 서비스

**2026 멋쟁이사자처럼 중앙해커톤**

- **Role:** Backend Developer
- **Team:** Frontend 2 / Backend 2 / Design 1
- **Period:** 2026.07 ~ 2026.08

### Tech

`Java 21` `Spring Boot` `Spring Security` `JPA` `MySQL`  
`Flyway` `Testcontainers` `Docker` `GitHub Actions` `OpenAI API`

### What I Did

- Spring Boot Backend 초기 환경 및 공통 API 구조 구성
- Flyway 기반 Database Migration 관리 체계 구축
- Testcontainers 기반 실제 MySQL 통합 테스트 환경 구성
- 사용자 취향 기반 상품 추천 기능 구현
- 구매 전 활용 가능성 Rule-Based 분석 설계
- OpenAI 호출을 공통 비동기 AI Job 구조로 분리
- Cloudinary 기반 이미지 업로드 및 ImageAsset 관리
- 이미지 기반 ITEM_ANALYSIS 기능 구현
- 소재 기반 관리 가이드·캘린더·알림 기능 구현

### Technical Highlights

**AI와 Rule-Based Logic 분리**

일관된 결과가 필요한 활용 가능성 점수는 Rule-Based 방식으로 계산하고,  
OpenAI는 계산 결과를 사용자에게 설명하는 역할로 분리했습니다.

**비동기 AI 처리 구조**

외부 AI API의 응답 지연과 실패 가능성을 고려해  
`PENDING → PROCESSING → SUCCEEDED / FAILED` 형태의 AI Job 구조를 적용했습니다.

**DB 변경 관리 및 통합 테스트**

Flyway로 Schema 변경 이력을 관리하고,  
Testcontainers를 활용해 실제 MySQL 환경에서 통합 테스트를 수행했습니다.

👉 **[Repository](https://github.com/developer-sw/ippulrae-backend)**
