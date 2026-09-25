# 윤성준 | Android × Backend Portfolio

Kotlin과 Jetpack Compose로 사용자 경험을 만들고, 그 흐름이 네트워크·서버·데이터베이스까지 안정적으로 이어지는 방식을 고민해 온 개발자 윤성준의 포트폴리오입니다.

[포트폴리오 보기](https://sssssungjun.github.io/portfolio/portfolio/) · [이력서 보기](https://sssssungjun.github.io/portfolio/)

## Portfolio

기술 스택을 나열하기보다 각 프로젝트를 **문제 → 설계 판단 → 실제 구현 근거** 순서로 구성했습니다. Android 프로젝트에서는 데이터 수명과 화면 상태를, Backend 프로젝트에서는 정합성·동시성·실패 복구를 중심으로 설명합니다.

| 프로젝트 | 관점 | 핵심 내용 |
| --- | --- | --- |
| **Bike-book** | Backend × Android | 오프라인 반납, 재시도 큐, 멱등성, 예약 시간 충돌 방지 |
| **대나무숲** | Backend | 무가입 익명 참여, 세션 기반 소유권, 기능별 동시성 제어, 부하 검증 |
| **Mori** | Android | 멀티모듈 구조, 독립 API 병렬 호출, Canvas 기반 서버 지표 시각화 |
| **관:상견례 · FaceMeet** | Android | 소셜 로그인, 실시간 채팅, 읽음·안 읽음 상태, 나가기·신고·차단 |

### 관:상견례 · FaceMeet

관상 분석 결과가 소개로 끝나지 않고 **궁합 매칭과 1:1 대화로 이어지는 사용자 여정**을 보여줍니다. 실제 앱 화면과 함께 실시간 메시지, 과거 채팅 이력, 세션·토큰처럼 수명과 갱신 방식이 다른 데이터를 Android에서 어떻게 분리했는지 정리했습니다.

담당 기능:

- 카카오·네이버 소셜 로그인
- WebSocket 기반 실시간 채팅 송수신
- 메시지 읽음 처리와 안 읽은 메시지 수
- 채팅방 나가기
- 사용자 신고 및 차단

## Repository

```text
.
├─ index.html          # 이력서 진입 페이지
├─ style.css           # 이력서 스타일
├─ resume/             # 상세 이력서
└─ portfolio/          # 프로젝트 포트폴리오
   ├─ index.html
   ├─ style.css
   └─ assets/
```

## Local preview

저장소 루트에서 정적 서버를 실행한 뒤 포트폴리오 경로를 엽니다.

```bash
python -m http.server 4173
```

- Resume: `http://127.0.0.1:4173/`
- Portfolio: `http://127.0.0.1:4173/portfolio/`

## Links

- [GitHub](https://github.com/SSSSSungjun)
- [Portfolio repository](https://github.com/SSSSSungjun/portfolio)
