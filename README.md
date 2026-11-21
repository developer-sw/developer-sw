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
- **테스트·자동화:** Testcontainers 기반 실제 PostgreSQL 통합 테스트와 GitHub Actions CI 구축
- **운영:** AWS Lightsail·Docker 배포 및 S3 암호화 백업 자동화

**Engineering Highlights — 문제 → 해결 → 검증**

- **동시 예약 충돌:** 개인의 악기별 공유 예약과 공연조의 합주실 독점 예약이 동시에 요청될 수 있음 → PostgreSQL 트랜잭션·행 잠금·DB 점유 제약으로 충돌 제어 → [예약 Repository](https://github.com/developer-sw/jeongeum-band-scheduler/blob/main/backend/src/main/java/kr/jeongeum/scheduler/reservation/repository/ReservationRepository.java) 및 [실제 PostgreSQL 통합 테스트](https://github.com/developer-sw/jeongeum-band-scheduler/blob/main/backend/src/test/java/kr/jeongeum/scheduler/ReservationIntegrationTest.java)로 경합·경계 조건 검증
- **예약 변경·교환 실패 시 원본 보존:** 새 점유 생성 중 충돌·권한·한도 검증이 실패할 수 있음 → 원본 점유 해제·신규 점유·한도 반영을 단일 트랜잭션으로 처리 → [변경 설계](https://github.com/developer-sw/jeongeum-band-scheduler/blob/main/docs/RESERVATION_CHANGES.md)와 [교환 설계](https://github.com/developer-sw/jeongeum-band-scheduler/blob/main/docs/RESERVATION_EXCHANGES.md)에 기록된 롤백·원본 보존 검증
- **운영 데이터 복구 검증:** 백업 파일만으로는 복원 가능성을 보장할 수 없음 → 운영 DB를 암호화 백업하고 별도 PostgreSQL 환경에서 복원 → **2026-11-15 기록 기준** 39개 테이블·29개 시퀀스·Flyway V1~V13·22개 예약 블록 대조 ([백업·복원 기록](https://github.com/developer-sw/jeongeum-band-scheduler/blob/main/docs/OPERATIONAL_DATABASE_BACKUPS.md))

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

## Other Projects

백엔드 중심 역량에 더해, 직접 담당한 프론트엔드 구현 경험도 확인할 수 있습니다.

| 프로젝트 | 담당 영역 | 현재 범위 |
| --- | --- | --- |
| [한서대 분실·습득물 관리 시스템](https://github.com/developer-sw/hanseo-lost-found-frontend) | **Frontend** · React / TypeScript / Vite 기반 학생·관리자 반응형 UI | 개발용 프로토타입 · 백엔드 API 미연동 |
| [붕붕 \| BoongBoong](https://github.com/developer-sw/boongboong) | **Frontend** · React / JavaScript 기반 프로필·설정·인증 관련 모바일 UI | 팀 프로젝트 · 본인 담당 UI 기준 |

### Representative Screens

실제 프로젝트 저장소에 포함된 화면 캡처입니다. **입을래?**는 팀 서비스 화면(본인 역할: 백엔드), **붕붕**은 본인이 담당한 UI 화면입니다. **정음**은 [운영 서비스](https://bandjeongeum.studio/)에서 확인할 수 있습니다.

<table>
  <tr>
    <td align="center" width="50%">
      <a href="https://github.com/developer-sw/ippulrae-backend">
        <img src="https://raw.githubusercontent.com/developer-sw/ippulrae-backend/main/docs/images/purchase-utility-report.png" alt="입을래? 서비스의 구매 활용성 분석 화면" width="290"/>
      </a>
      <br/>
      <sub>입을래? · 구매 활용성 분석 (팀 서비스 화면)</sub>
    </td>
    <td align="center" width="50%">
      <a href="https://github.com/developer-sw/boongboong">
        <img src="https://raw.githubusercontent.com/developer-sw/boongboong/main/docs/images/profile-edit.png" alt="붕붕 서비스의 모바일 프로필 수정 화면" width="230"/>
      </a>
      <br/>
      <sub>붕붕 · 프로필 수정 (직접 구현한 UI)</sub>
    </td>
  </tr>
</table>

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

### Frontend
<p>
  <img src="https://img.shields.io/badge/React-149ECA?style=flat-square&logo=react&logoColor=white" alt="React"/>
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white" alt="Next.js"/>
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white" alt="Tailwind CSS"/>
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite"/>
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

- 멋쟁이사자처럼 대학 13기, 14기 중앙 해커톤 참여
- 프론트엔드 개발 경험을 쌓은 후 Java / Spring Boot 중심의 백엔드 개발로 역량 확장
- 팀 프로젝트에서 프론트엔드·백엔드·디자인 직군과 협업
- REST API, 관계형 데이터베이스, 서비스 개발 과정 경험

---

## Contact

- **Email:** [swjsoftware01@gmail.com](mailto:swjsoftware01@gmail.com)
