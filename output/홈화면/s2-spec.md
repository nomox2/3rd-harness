# 화면 설계 문서 — 홈 화면

유저스토리: 무료 학습자가 허들링의 공개 AI 실무 콘텐츠를 카테고리별로 둘러본다
프레임: 390×844 (mobile baseline)

---

## 화면 구조

### 1. 상단 내비게이션
- 컴포넌트: nav-pill (floating, horizontally centered)
- 좌: 로고 + 워드마크
- 우: "로그인" 버튼 (button-outline) + "무료 시작" (button-primary)
- 배경: canvas-soft (#f3f3f3), rounded.full

### 2. 히어로 섹션
- 헤딩: typography.display (32px, 700) — "AI 실무, 지금 바로 시작하세요"
- 서브: typography.body-lg (17px, 300) — 서비스 한 줄 소개
- CTA: button-primary "무료로 둘러보기"
- 배경: canvas (#ffffff)
- 하단 여백: spacing.section (48px)

### 3. 카테고리 필터
- 컴포넌트: 칩 (button-pill-soft, rounded.full)
- 항목: 전체 / AI 글쓰기 / 프롬프트 / 툴 활용 / 업무 자동화
- 선택 상태: canvas-soft fill → ink fill (반전)
- 가로 스크롤, 좌우 패딩 spacing.md (16px)

### 4. 콘텐츠 카드 목록
- 컴포넌트: 카드 (rounded.md, 1px hairline-soft 아웃라인)
- 카드 구성:
  - 썸네일: rounded.sm (16px), 16:9 비율
  - 카테고리 태그: badge-overlay
  - 제목: typography.heading-4 (18px, 700)
  - 설명: typography.body-sm (13px, 400, text-muted)
- 레이아웃: 1열 리스트, 카드 간격 spacing.sm (12px)
- 좌우 패딩: spacing.md (16px)

### 5. 유료 멤버십 업셀 배너
- 배경: ink (#141414), rounded.md, 좌우 패딩 spacing.md
- 텍스트: on-primary (흰색)
  - 헤딩: typography.heading-3 (20px, 700) — "더 많은 콘텐츠가 기다려요"
  - 서브: typography.body-sm — 유료 멤버 혜택 요약
- CTA: button-outline (흰색 테두리 버전) "멤버십 보기"

### 6. 푸터
- 컴포넌트: footer (ink fill, rounded.md 상단 모서리)
- 내용: 워드마크, 링크 2열, 저작권

---

## 규칙 체크 (design-rules.md 연동)

- [x] 배경 #ffffff
- [x] 텍스트 #141414
- [x] 버튼 rounded.full
- [x] 카드 rounded.md (24px)
- [x] 폰트 Pretendard, 헤딩 700
- [x] 그림자 없음
- [x] accent blue 미사용 (CTA 아님)
- [x] 좌우 패딩 16px
- [x] 간격 8px 단위
