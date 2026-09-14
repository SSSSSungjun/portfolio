# 윤성준 | Android Developer

Kotlin과 Jetpack Compose 기반 Android 네이티브 앱 개발을 주력으로 하고 있습니다. 모바일 앱의 구조 설계와 네트워크·데이터 처리 경험을 중심으로 쌓아왔으며, 서비스 전체 흐름을 이해하기 위해 Java·Spring Boot 기반 백엔드도 함께 개발했습니다.

**GitHub** https://github.com/SSSSSungjun  
**Focus** Android · Mobile Application · Backend

---

## Experience

### 한국동서발전 울산본부 | 인턴
**2026.04.06 ~ 2026.08.28**

- 정보보안 부서 업무 지원
- 정보보안 관련 자료 조사 및 문서 관리

---

## Education & Training

### 건국대학교 컴퓨터공학부 | 학사
**2018.03 ~ 2025.02**

### Samsung SW·AI Academy For Youth 13기 | Mobile Track
**2025.01 ~ 2025.12 | 수료**

- Java, Kotlin, Android, Spring Boot, MySQL, 알고리즘, Vue.js 학습
- Android 네이티브 앱 개발을 중심으로 모바일 및 백엔드 팀 프로젝트 수행

---

## Tech Stack

### Android

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=flat-square&logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)

Kotlin · Jetpack Compose · XML · MVVM · MVI · UDF · Hilt  
Coroutines · Flow · Retrofit2 · Ktor Client · OkHttp  
Room · DataStore · WorkManager · Paging3 · Navigation · WebSocket · Firebase · ML Kit

### Backend & Database

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

Java · Spring Boot · Spring MVC · Spring Security · Spring Data JPA  
JDBC · MyBatis · PostgreSQL · MySQL · Redis · JWT · Flyway

### Frontend

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vuedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)

React · TypeScript · Vue.js

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white)

Kotlin · Java · JavaScript · TypeScript · Python · C++ · SQL

### Infra & Tools

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

Docker · Docker Compose · Nginx · AWS EC2 · Git · GitHub · GitHub Actions  
Jira · Figma · Notion · Codex

---

## Projects

### Bike-book | 사내 자전거 예약 Android·Backend 앱
**2026.07 ~ 2026.08 | Android & Backend Developer · 기술 설계**

- 사내 공용 자전거의 신청, 관리자 승인, 이용, 반납을 관리하는 앱을 구현했습니다.
- Android 전체 구조와 API·데이터 계약, 개발 환경 및 테스트 구조를 설계했습니다.
- Room을 단일 데이터 원본으로 사용하고 WorkManager 기반 오프라인 반납 재전송을 구성했습니다.
- Screen·ViewModel이 Repository interface에 의존하도록 하고 RemoteDataSource를 Fake와 Ktor 구현으로 분리해 서버 연결 전에도 앱 흐름을 개발·검증할 수 있도록 구성했습니다.
- PostgreSQL exclusion constraint로 활성 예약의 시간 충돌을 방어하고 UUID 멱등키와 advisory lock으로 네트워크 재시도에 따른 중복 요청을 방어했습니다.
- Transactional Outbox를 적용해 예약 상태 변경과 알림 이벤트의 정합성을 관리했습니다.
- JWT와 Refresh Token Rotation을 적용하고 역할 및 예약 소유권을 서버에서 검증하도록 구성했습니다.
- Codex 작업 범위와 개발 규칙을 정하고 GitHub Actions를 활용해 결과 확인과 코드 검수 과정을 자동화했습니다.
- 앱을 완성해 실사용 가능성 검토 단계까지 진행했으며, 보안 검토 미통과로 실제 도입은 하지 않았습니다.

**Tech** `Kotlin` `Jetpack Compose` `Room` `WorkManager` `Ktor Client` `Hilt` `Coroutines` `Java 17` `Spring Boot` `Spring Security` `PostgreSQL` `JWT` `Flyway` `Docker Compose` `GitHub Actions`

---

### 대나무숲 | 익명 웹 게시판
**2026.07 | Full-stack Developer · 기술 설계**

- 로그인 없이 글과 댓글을 작성하는 익명 게시판의 프론트엔드와 백엔드를 구현했습니다.
- 쿠키 기반 익명 세션으로 같은 브라우저에서 작성한 글과 댓글의 수정·삭제 권한을 서버에서 검증했습니다.
- Controller, Service, Repository, DTO의 책임을 분리하고 Entity를 API 계약에 직접 노출하지 않도록 구성했습니다.
- 조회수는 단일 UPDATE 쿼리로 원자 증가시키고, 게시글·댓글 수정과 좋아요 요청에는 비관적 잠금과 unique constraint를 적용해 동시 요청의 중복과 충돌을 방어했습니다.
- 게시글 목록의 좋아요·댓글 관련 반복 조회를 줄이기 위해 ID 목록을 모아 집계 쿼리로 조회하도록 구성했습니다.
- React에서는 reducer 기반 상태 관리와 API 레이어 분리로 화면 상태와 데이터 요청 로직을 분리했습니다.
- GitHub-hosted runner에서 PostgreSQL 16과 애플리케이션을 함께 실행해 200 VU, 3분 부하 테스트를 수행했습니다.
- 총 HTTP 요청 75,336건, 처리량 357.16 req/s, 오류율 0%, HTTP p95 52.89ms를 확인하고 SQL 정합성 검사를 수행했습니다.

**Tech** `Java` `Spring Boot` `Spring Data JPA` `PostgreSQL` `Flyway` `React` `TypeScript` `Axios` `Docker Compose` `Nginx` `k6` `SSE`

---

### Mori | 서버 리포트 Android 앱
**2025.09 | Android Developer**

- EC2 서버의 CPU, 메모리, 디스크, 네트워크 등 서버 메트릭을 Android 앱에서 조회하고 시각화했습니다.
- feature, core, data 모듈을 분리한 멀티모듈 구조를 설계했습니다.
- Coroutines `async/await`를 활용해 여러 API 호출을 병렬 처리했습니다.
- Canvas API 기반 서버 메트릭 차트를 직접 구현하고 Navigation 기반 화면 흐름을 구성했습니다.
- 서버 지표의 의미와 백엔드 요구사항을 이해하기 위해 서버·JVM 관련 기본 개념을 학습하고 백엔드 팀과 지표 의미와 그래프 표현 방식을 조율했습니다.

**Tech** `Kotlin` `Jetpack Compose` `Hilt` `Coroutines` `Flow` `Retrofit2` `Canvas` `Navigation` `Multi-Module`

---

### 관:상견례 | 실시간 1대1 채팅 Android 앱
**2025.07.08 ~ 2025.08.21 | Android Developer**

- 얼굴 인식과 관상 분석을 활용해 사용자를 매칭하고 실시간 1대1 채팅을 제공하는 Android 앱을 개발했습니다.
- MVVM과 Repository 패턴을 기반으로 Android 코드베이스와 데이터 계층을 구성했습니다.
- WebSocket과 OkHttp를 활용해 실시간 메시지 송수신을 구현했습니다.
- DataStore를 활용해 로그인 세션과 토큰을 관리했습니다.
- Paging3를 적용해 채팅 이력을 페이지 단위로 불러오도록 구성했습니다.

**Tech** `Kotlin` `Jetpack Compose` `Hilt` `Retrofit2` `OkHttp` `WebSocket` `DataStore` `Paging3` `Navigation` `Firebase` `ML Kit`

---

### 싱싱과일 | 매장 주문·NFC 결제 플랫폼
**2025.05 | Android & Backend Developer**

- 비콘 감지와 GPS 위치 확인을 연동해 매장 내 모바일 주문 흐름을 구현했습니다.
- Android NFC API를 활용해 결제 시뮬레이션을 개발했습니다.
- XML UI와 ViewModel을 이용한 MVVM 구조를 적용했습니다.
- Spring Boot와 MyBatis 기반 백엔드를 개발하고 AWS EC2에 배포했습니다.

**Tech** `Kotlin` `XML` `MVVM` `Beacon` `GPS` `NFC` `Java` `Spring Boot` `MyBatis` `AWS EC2`

---

### 따숨 | 환경 공공데이터 활용 친환경 실천 Android 앱
**2025.04 ~ 2025.05 | Android Developer**

- 환경부 공공데이터를 활용한 친환경 실천 유도 Android 앱을 개발했습니다.
- 사용량 기반 친환경 보일러 추천, AI 컨설팅 챗봇, 환경 실천 커뮤니티, 자가 사용량 검침 기능을 포함한 서비스에 참여했습니다.
- 멀티모듈 구조로 모듈 간 의존성과 코드 재사용을 관리했습니다.
- Hilt 의존성 주입과 MVVM 기반 ViewModel 구조를 적용했습니다.

**Tech** `Java` `XML` `ViewModel` `Hilt` `Multi-Module`

---

### AI 심리 상담사 앱 | AI 해커톤
**2024.07.15 ~ 2024.07.26 | Android Developer**

- AI가 상담을 진행하고 상담 결과를 제공하는 모바일 앱을 개발했습니다.
- Android 채팅 UI와 비즈니스 로직을 담당했습니다.

---

### 카본풋풋 | 졸업 프로젝트
**2023.09.04 ~ 2023.11.16 | Android Frontend**

- 음식 사진을 촬영하면 음식의 탄소 발자국을 알려주는 온디바이스 AI Android 앱을 개발했습니다.
- Android 프론트엔드 전반을 담당했습니다.
- Figma로 UI, 화면 흐름, 데이터 방향과 API 연동 지점을 시각화했습니다.
- 비대면 환경에서 정기 화상회의를 진행하며 Android 파트를 완성했습니다.

---

## Certifications & Language

- **TOEIC Speaking IH (140)** | ETS | 2026.09.06 | 유효기간 2028.09.06
- **한국사능력검정시험 2급** | 국사편찬위원회 | 2026.06.05
- **SQLD** | 한국데이터산업진흥원 | 2025.09.19
- **정보처리기사** | 한국산업인력공단 | 2024.06.18

---

## Awards & Activities

### AI Worker 해커톤 최우수상(2등)
**2022 | 4인 팀**

- Arduino와 HuskyLens를 활용한 자동화 기기를 개발했습니다.
- HuskyLens 기반 색상 인식 로직 구현을 담당했습니다.
- 코드 병합 및 버전 관리, 하드웨어·소프트웨어 통합 협업을 담당했습니다.

### CS 스터디 | 조장
**2025.02.10 ~ 2025.05.23**

- Computer Science 주제를 분담해 학습한 뒤 발표와 질의응답을 진행하는 스터디를 운영했습니다.
