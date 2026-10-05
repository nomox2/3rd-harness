# 하네스 산출물 정의

## 저장 위치
output/{화면이름}/

## 파일명 규칙
| 파일명 | 내용 |
|---|---|
| s1-references.md | 경쟁사 레퍼런스 수집본 |
| s2-analysis.md | 분석 결과 |
| s2-spec.md | 화면 설계 문서 |
| s2-keyscreen.md | 키스크린 2~3개 |
| s3-review.md | 가이드 위반 검토 결과 |

## 재개 규칙
- 해당 파일이 존재하면 그 단계는 완료로 간주
- 없는 파일의 첫 단계부터 재개

## 규칙 SSOT
- 경로: rules/design-rules.md
- 출처: design.md에서 기계가 셀 수 있는 항목만 추출
