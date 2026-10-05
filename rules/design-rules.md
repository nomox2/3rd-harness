# 디자인 규칙 SSOT
출처: docs/design.md

판정자 에이전트가 각 항목을 YES / NO로 체크한다.
모든 항목이 YES여야 S3 통과.

---

## 색상

| # | 규칙 | 판정 기준 |
|---|---|---|
| C1 | 배경은 흰색만 사용 | canvas = #ffffff |
| C2 | 텍스트·CTA는 잉크 블랙만 사용 | ink = #141414 |
| C3 | 파란색은 상업적 신호(뱃지·할인 콜아웃)에만 사용 | accent = #0066ff, CTA에 사용 시 위반 |
| C4 | C1·C2·C3 외 다른 색상 없음 | 추가 색상 0개 |
| C5 | 그림자(drop shadow) 없음 | shadow 속성 0개 |

---

## 타이포그래피

| # | 규칙 | 판정 기준 |
|---|---|---|
| T1 | 폰트는 Pretendard만 사용 | 다른 폰트 0개 |
| T2 | 헤딩은 Bold 700, line-height 1.3–1.35 | weight=700, lh=1.3~1.35 |
| T3 | 본문은 Regular 400, line-height 1.5 | weight=400, lh=1.5 |
| T4 | 자간(letter-spacing) 0 | tracking=0 everywhere |
| T5 | 올캡스(all-caps) 없음 | text-transform: uppercase 0개 |

---

## 모양 (Border Radius)

| # | 규칙 | 판정 기준 |
|---|---|---|
| S1 | 버튼·뱃지·토글·내비게이션은 모두 pill | rounded.full (9999px) |
| S2 | 컨테이너·카드는 rounded.md | 24px |
| S3 | 미디어 타일·인풋은 rounded.sm | 16px |
| S4 | 풀블리드 미디어는 rounded.none | 0px |
| S5 | 허용된 radius 값: 0 / 16 / 24 / 9999px만 사용 | 그 외 값 0개 |

---

## 레이아웃

| # | 규칙 | 판정 기준 |
|---|---|---|
| L1 | 모바일 기준 프레임 390×844 | frame width=390 |
| L2 | 좌우 패딩 16px | side padding=16px |
| L3 | 간격은 8px 단위 (4px 허용) | spacing % 4 = 0 |

---

## 컴포넌트

| # | 규칙 | 판정 기준 |
|---|---|---|
| P1 | 인풋 기본 상태에 테두리 없음 | border=none at rest |
| P2 | 인풋 포커스 시 2px 잉크 링 | focus ring = 2px #141414 |
| P3 | 큐레이터·인물 사진은 흑백만 | grayscale=100% |
| P4 | 앱 아이콘은 30% squircle radius | icon radius=30% |
