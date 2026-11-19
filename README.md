<div align="center">

<img src="./backend-banner(5).gif" alt="Backend Developer — Building reliable systems, from code to production" width="100%" />

<br>

**Java / Spring Boot Backend Developer**

실제 사용자가 있는 서비스를 개발·운영하며  
**데이터 정합성, 테스트, 장애 복구까지 고려하는 백엔드 개발**을 지향합니다.

`Java` `Spring Boot` `PostgreSQL` `MySQL` `Docker` `AWS`

</div>

---

## About Me

- **실서비스 개발·운영:** 밴드 동아리 예약 서비스를 직접 개발하고 AWS 환경에서 운영하고 있습니다.
- **데이터 정합성:** PostgreSQL 트랜잭션과 행 잠금으로 예약 충돌·중복 처리 문제를 다루었습니다.
- **검증과 운영:** Testcontainers 통합 테스트, GitHub Actions CI, DB 암호화 백업·독립 복원 경험이 있습니다.
- **팀 개발:** 프론트엔드 경험을 바탕으로 Java / Spring Boot 백엔드 개발과 팀 협업을 이어가고 있습니다.

---

## Featured Projects

### 🎸 [정음 | JEONGEUM](https://github.com/developer-sw/jeongeum-band-scheduler)

**밴드 동아리 합주실 예약 및 공연조 관리 웹 서비스**  
`개인 주도 개발` · `Full-stack` · `Deployment & Operations` · `2026.10 ~ Present`

- **실제 운영:** 2026년 10월부터 운영 중이며, **가입자 30명 이상**(2026년 11월 기록 기준)
- **핵심 구현:** 개인·공연조 예약, 주간 반복 배정, 예약 변경·교환, 역할별 권한, Web Push 알림
- **데이터 정합성:** PostgreSQL 트랜잭션·행 잠금·DB 제약을 활용한 예약 충돌 및 중복 처리 방지
- **테스트·자동화:** Testcontainers 기반 실제 PostgreSQL 통합 테스트와 GitHub Actions CI 구축
- **운영·복구:** AWS Lightsail·Docker 배포, S3 암호화 백업 및 별도 PostgreSQL 환경으로의 복원 검증

**검증 기록:** [2026-11-15 기준 CI 7개 작업 성공](https://github.com/developer-sw/jeongeum-band-scheduler/actions/runs/43561431440) · Backend **406건** / Frontend **441건** 테스트 통과(해당 실행 기록 기준)

**Tech:** `Java 21` `Spring Boot` `PostgreSQL` `Next.js` `TypeScript` `Docker` `AWS Lightsail`

[Live Service](https://bandjeongeum.studio/) · [Repository](https://github.com/developer-sw/jeongeum-band-scheduler) · [예약 통합 테스트 코드](https://github.com/developer-sw/jeongeum-band-scheduler/blob/main/backend/src/test/java/kr/jeongeum/scheduler/ReservationIntegrationTest.java)

### 👔 [입을래? | Ippulrae](https://github.com/developer-sw/ippulrae-backend)

**AI 기반 명품 구매·활용 지원 서비스**  
`팀 프로젝트` · `Backend Developer (2인 중 1명)` · `2026.07 ~ 2026.08`

- **담당 영역:** DB 마이그레이션, 통합 테스트 환경, 구매 활용성 분석, 공통 비동기 AI Job 및 이미지 분석 파이프라인
- **데이터 관리:** Flyway **V1~V21** 마이그레이션과 Testcontainers 기반 MySQL 통합 테스트
- **AI 처리 설계:** 일관된 점수 계산은 Rule-Based 로직으로 처리하고, OpenAI API는 자연어 설명에 활용
- **비동기 처리:** 외부 AI 호출을 Job으로 분리하고 멱등성 키·입력 식별·상태 조회를 고려

**Tech:** `Java 21` `Spring Boot` `JPA` `MySQL` `Flyway` `Testcontainers` `Docker` `OpenAI API`

[Repository](https://github.com/developer-sw/ippulrae-backend) · [Flyway·통합 테스트 기여 PR](https://github.com/pro660/Hackathon_BE/pull/21) · [비동기 AI Job 기여 PR](https://github.com/pro660/Hackathon_BE/pull/36)

---

## Tech Stack

실제 프로젝트에서 활용한 기술을 중심으로 정리했습니다.

### Backend
<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security"/>
  <img src="https://img.shields.io/badge/Spring%20JDBC-6DB33F?style=flat-square&logo=spring&logoColor=white" alt="Spring JDBC"/>
  <img src="https://img.shields.io/badge/JPA-59666C?style=flat-square" alt="JPA"/>
</p>

### Database & Migration
<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" alt="Flyway"/>
</p>

### Testing
<p>
  <img src="https://img.shields.io/badge/JUnit%205-25A162?style=flat-square&logo=junit5&logoColor=white" alt="JUnit 5"/>
  <img src="https://img.shields.io/badge/Testcontainers-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Testcontainers"/>
</p>

### Infrastructure & DevOps
<p>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
  <img src="https://img.shields.io/badge/AWS%20Lightsail-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white" alt="AWS Lightsail"/>
  <img src="https://img.shields.io/badge/AWS%20S3-569A31?style=flat-square&logo=amazons3&logoColor=white" alt="AWS S3"/>
</p>

### Tools & Integration
<p>
  <img src="https://img.shields.io/badge/Gradle-02303A?style=flat-square&logo=gradle&logoColor=white" alt="Gradle"/>
  <img src="https://img.shields.io/badge/Swagger%20%2F%20OpenAPI-85EA2D?style=flat-square&logo=swagger&logoColor=black" alt="Swagger / OpenAPI"/>
  <img src="https://img.shields.io/badge/OpenAI%20API-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI API"/>
</p>

---

## Experience & Activities

### 🦁 멋쟁이사자처럼 대학 13기 · 14기

- 프론트엔드 개발 경험을 쌓은 후 Java / Spring Boot 중심의 백엔드 개발로 역량 확장
- 팀 프로젝트에서 프론트엔드·백엔드·디자인 직군과 협업
- REST API, 관계형 데이터베이스, 서비스 개발 과정 경험

---

## Contact

- **Email:** [swjsoftware01@gmail.com](mailto:swjsoftware01@gmail.com)
