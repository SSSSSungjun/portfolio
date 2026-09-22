# Resume Style System

이 이력서는 CSS를 **Design Token + Component + Variant** 구조로 관리한다.

## 1. 수정 원칙

1. 새 숫자를 컴포넌트 selector에 바로 추가하지 않는다.
2. 크기·간격·색상을 바꾸려면 먼저 `:root`의 token을 수정한다.
3. 같은 역할의 요소는 반드시 같은 token을 사용한다.
4. 특정 섹션만 달라야 하면 selector override를 추가하지 말고 **component variable**을 덮어쓴다.
5. CSS 파일 맨 아래에 임시 override 블록을 누적하지 않는다.

## 2. 주요 Typography Token

- `--font-size-section-title`: Experience / Education / Tech Stack / Projects 등
- `--font-size-item-title`: 회사명 / 학교명 / 활동명
- `--font-size-project-title`: 프로젝트명
- `--font-size-skill-title`: Android / Backend & Data / Infra & Tools
- `--font-size-accent`: 학사 / 인턴 / Description / Contributions / Tech
- `--font-size-date`: 기간
- `--font-size-meta`: GitHub / 자격증 발급기관·날짜

## 3. 주요 Layout Token

- `--page-padding-x`: 페이지 전체 좌우 여백
- `--section-label-width`: 왼쪽 섹션 제목 컬럼 폭
- `--section-column-gap`: 섹션 제목과 본문 사이 간격
- `--section-padding-y`: 일반 섹션 위아래 여백
- `--section-padding-y-compact`: Tech Stack / Projects 위아래 여백
- `--project-block-gap`: Description / Contributions / Tech 사이 간격

## 4. Components

### .resume-section
모든 대분류 섹션 공통 레이아웃.

### .entry / .entry-head
Experience, Education, Awards에서 재사용.

### .skill-group
Tech Stack의 한 줄. 좌측 label + 우측 badge.

### .project
한 프로젝트 전체.

내부 구조:
- `.entry-head`: 프로젝트명 + 날짜
- `.project-label`: Description / Contributions / Tech
- `.project-description`: 프로젝트 소개
- `ul`: Contributions
- `.project-tech-list`: 기술 나열

### .simple-list
Certifications & Language.

## 5. Variants

### .tech-stack-section
일반 섹션보다 세로 padding을 줄이고 Tech Stack에 맞는 title offset 사용.

### .projects-section
일반 섹션보다 세로 padding을 줄이고 프로젝트 제목 크기에 맞춰 왼쪽 section title의 optical offset을 조정.

## 6. Alignment Rule

Projects / Bike-book처럼 글자 크기가 다른 두 제목은 top 좌표만 같게 두면 시각적으로 어긋난다.

따라서:
- 일반 섹션: `--section-title-offset-default`
- Tech Stack: `--section-title-offset-tech`
- Projects: `--section-title-offset-projects`

이 세 token으로 수직 중심을 보정한다.

## 7. 앞으로의 예

"프로젝트 제목 2px 키우기"
→ `--font-size-project-title`만 변경.

"전체 섹션 본문을 왼쪽으로 당기기"
→ `--section-label-width` 또는 `--section-column-gap`만 변경.

"Description / Contributions / Tech 간격 늘리기"
→ `--project-block-gap`만 변경.

"초록색 보조 텍스트 전체 크기 변경"
→ `--font-size-accent`만 변경.
