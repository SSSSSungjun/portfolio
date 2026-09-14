# 윤성준 | Android Developer

Android 네이티브 앱 개발을 중심으로 경험을 쌓아온 개발자입니다. Kotlin과 Jetpack Compose 기반 모바일 앱을 주력으로 개발해 왔으며, 서비스 연동과 전체 흐름을 이해하기 위해 Java·Spring Boot 기반 백엔드 개발도 함께 경험했습니다.

- GitHub: https://github.com/SSSSSungjun
- 주요 분야: Android, Mobile Application, Backend

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

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?logo=firebase&logoColor=black)

- Kotlin, Jetpack Compose, XML
- MVVM, MVI, UDF, Hilt
- Coroutines, Flow, Retrofit2, Ktor Client, OkHttp
- Room, DataStore, WorkManager, Paging3, Navigation
- WebSocket, Firebase, ML Kit

### Backend & Database

![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)

- Java, Spring Boot, Spring MVC, Spring Security
- Spring Data JPA, JDBC, MyBatis
- PostgreSQL, MySQL, Redis, JWT, Flyway

### Frontend

![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?logo=vuedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)

- React, TypeScript, Vue.js

### Languages

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-336791?logo=postgresql&logoColor=white)

- Kotlin, Java, JavaScript, TypeScript, Python, C++, SQL

### Infra & Tools

![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?logo=nginx&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazonwebservices&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)

- Docker, Docker Compose, Nginx, AWS EC2
- Git, GitHub, GitHub Actions, Jira, Figma, Notion
- Codex 기반 AI 개발 규칙 및 자동 검수 환경 구성 경험

---

## Projects

### Bike-book | 사내 자전거 예약 Android·Backend 앱
**2026.07 ~ 2026.08 | Android & Backend Developer / 기술 설계**

- 사내 공용 자전거의 신청, 관리자 승인, 이용, 반납을 관리하는 앱 구현
- Android 전체 구조, API·데이터 계약, 개발 환경 및 테스트 구조 설계
- Room을 단일 데이터 원본으로 사용하고 WorkManager 기반 오프라인 반납 재전송 구성
- 서버 연동을 고려해 Repository 계층과 RemoteDataSource를 분리하고, 백엔드 연결 전에도 전체 앱 흐름을 실행할 수 있도록 구성
- PostgreSQL exclusion constraint로 예약 시간 충돌을 방어하고 UUID 멱등키와 advisory lock으로 중복 요청 방어
- Codex 작업 범위와 개발 규칙을 정하고 GitHub Actions를 활용한 결과 확인 및 코드 검수 자동화
- 앱 완성 후 실사용 가능성 검토 단계까지 진행, 보안 검토 미통과로 실제 도입은 하지 않음
- **Tech:** Kotlin, Jetpack Compose, Room, WorkManager, Ktor Client, Java 17, Spring Boot, PostgreSQL, JWT, Flyway, GitHub Actions

---

### 대나무숲 | 익명 웹 게시판
**2026.07 | Full-stack Developer / 기술 설계**

- 로그인 없이 글과 댓글을 작성하는 익명 게시판의 프론트엔드와 백엔드 구현
- 쿠키 기반 익명 세션으로 서버 측 작성자 소유권 검증 구성
- Controller, Service, Repository, DTO 책임 분리 및 API 계약 설계
- 조회수 단일 UPDATE, 비관적 잠금, unique constraint로 동시 요청 정합성 관리
- React reducer 기반 상태 관리와 API 레이어 분리
- GitHub-hosted runner에서 PostgreSQL과 애플리케이션을 함께 실행해 가상 사용자 200명, 3분 부하 테스트 수행
- 총 HTTP 요청 75,336건, 오류율 0%, p95 52.89ms 확인 및 SQL 정합성 검사 수행
- **Tech:** Java, Spring Boot, Spring Data JPA, PostgreSQL, React, TypeScript, Flyway, Docker Compose, Nginx, k6, SSE

---

### Mori | 서버 리포트 Android 앱
**2025.09 | Android Developer**

- EC2 서버의 CPU, 메모리, 디스크, 네트워크 등 서버 메트릭을 Android 앱에서 조회하고 시각화
- feature, core, data 모듈을 분리한 멀티모듈 구조 설계
- Coroutines `async/await`를 활용한 다중 API 병렬 처리
- Canvas API 기반 서버 메트릭 차트 구현
- 서버 및 JVM 기본 개념을 학습해 Prometheus 지표의 의미를 이해하고 화면 요구사항에 반영
- **Tech:** Kotlin, Jetpack Compose, Hilt, Coroutines, Flow, Retrofit2, Canvas, Navigation

---

### 관:상견례 | 실시간 1대1 채팅 Android 앱
**2025.07.08 ~ 2025.08.21 | Android Developer**

- 얼굴 분석을 활용한 1대1 사용자 매칭 및 실시간 채팅 Android 앱 개발
- MVVM과 Repository 패턴 기반 Android 코드베이스와 데이터 계층 구성
- WebSocket과 OkHttp 기반 실시간 메시지 송수신 구현
- DataStore를 활용한 로그인 세션 및 토큰 관리
- Paging3를 활용한 채팅 이력 페이징 처리
- **Tech:** Kotlin, Jetpack Compose, Hilt, Retrofit2, OkHttp, WebSocket, DataStore, Paging3, Firebase, ML Kit

---

### 싱싱과일 | 매장 주문·NFC 결제 플랫폼
**2025.05 | Android & Backend Developer**

- 비콘 감지와 GPS 위치 확인을 연동해 매장 내 모바일 주문 흐름 구현
- Android NFC API를 활용한 결제 시뮬레이션 개발
- XML UI와 ViewModel을 이용한 MVVM 구조 적용
- Spring Boot와 MyBatis 기반 백엔드 개발 및 AWS EC2 배포
- **Tech:** Kotlin, XML, MVVM, Beacon, GPS, NFC, Java, Spring Boot, MyBatis, AWS EC2

---

### 따숨 | 환경 공공데이터 활용 친환경 실천 Android 앱
**2025.04 ~ 2025.05 | Android Developer**

- 환경부 공공데이터를 활용한 친환경 실천 유도 Android 앱 개발
- 사용량 기반 친환경 보일러 추천, AI 컨설팅 챗봇, 환경 실천 커뮤니티, 자가 사용량 검침 기능 개발
- 멀티모듈 구조로 모듈 간 의존성과 코드 재사용 관리
- Hilt 의존성 주입과 MVVM 기반 ViewModel 구조 적용
- **Tech:** Java, XML, ViewModel, Hilt

---

### AI 심리 상담사 앱 | AI 해커톤
**2024.07.15 ~ 2024.07.26 | Android Developer**

- AI가 상담을 진행하고 상담 결과를 제공하는 모바일 앱 개발
- Android 채팅 UI 및 비즈니스 로직 담당

---

### 카본풋풋 | 졸업 프로젝트
**2023.09.04 ~ 2023.11.16 | Android Frontend**

- 음식 사진을 촬영하면 음식의 탄소 발자국을 알려주는 온디바이스 AI Android 앱 개발
- Android 프론트엔드 전반 담당
- Figma로 UI, 화면 흐름, 데이터 방향과 API 연동 지점을 시각화
- 비대면 환경에서 정기 화상회의를 진행하며 Android 파트 완성

---

## Certifications & Language

- **SQLD** | 한국데이터산업진흥원 | 2025.09.19
- **정보처리기사** | 한국산업인력공단 | 2024.06.18
- **한국사능력검정시험 2급** | 국사편찬위원회 | 2026.06.05
- **TOEIC Speaking IH (140)** | ETS | 2026.09.06 | 유효기간 2028.09.06

---

## Awards & Activities

### AI Worker 해커톤 최우수상(2등)
**2022 | 4인 팀**

- Arduino와 HuskyLens를 활용한 자동화 기기 개발
- HuskyLens 기반 색상 인식 로직 구현
- 코드 병합 및 버전 관리, 하드웨어·소프트웨어 통합 협업 담당

### CS 스터디 | 조장
**2025.02.10 ~ 2025.05.23**

- Computer Science 주제를 분담해 학습하고 발표 및 질의응답을 진행하는 스터디 운영