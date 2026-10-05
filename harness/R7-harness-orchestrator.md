# 하네스 오케스트레이터 정의

## 오케스트레이터
- 역할: Claude Code 메인 에이전트
- CLAUDE.md를 읽고 전체 흐름 지휘
- 각 에이전트 호출 순서: S1 → S2 → S3
- 게이트 통과 여부 판정자 에이전트에게 위임 후 결과 수신

## CLAUDE.md 구성 순서
1. 목적 (R2)
2. 파이프라인 (R3)
3. 산출물 규칙 (R4)
4. 게이트 (R5)
5. 역할 (R6)

## 참조 파일
- docs/story-service.md — 유저스토리·금지 규칙
- docs/story-work.md — 작업 흐름
- rules/design-rules.md — 판정 기준
