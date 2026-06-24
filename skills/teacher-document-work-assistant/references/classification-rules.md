# Classification Rules

Create `knowledge-base/source-inventory.md` before synthesis. Each row should classify one file and cite the evidence used for the classification.

## Categories

| Category | Meaning | Evidence Signals |
| --- | --- | --- |
| `manual` | 교육청, 교육지원청, 학교가 배포한 공식 절차 안내 | 목차, 절차, 법령/지침 근거, "매뉴얼", "지침" |
| `previous-year-approval` | 전년도 내부결재, 품의, 계획 결재 | 결재선, 시행일, 담당, 예산, 내부결재 |
| `form` | 사용자가 채워 넣는 서식 | 빈 칸, 제출 양식, 붙임, 신청서, 점검표 |
| `operation-result` | 실제 운영 후 결과, 정산, 보고, 반성 | 결과보고, 운영 결과, 참여 인원, 정산, 사진 목록 |
| `notice` | 공문, 안내문, 마감 공지 | 제출기한, 대상, 제출처, 공문 번호 |
| `meeting-note` | 협의록, 회의록, 인수인계 메모 | 참석자 역할, 논의 사항, 결정 사항 |
| `budget-evidence` | 예산, 지출, 영수증, 견적 관련 자료 | 산출내역, 품의, 지출, 증빙 |
| `unknown` | 근거가 부족해 분류 보류 | 제목만 있고 내용 근거 부족 |

## Inventory Columns

Use this table shape:

```markdown
| id | path | category | year/month | source owner | why classified this way | confidence | use in 업무비서 |
| --- | --- | --- | --- | --- | --- | --- | --- |
```

## Confidence

- `high`: title and content both support the category.
- `medium`: content supports the category but some metadata is missing.
- `low`: filename suggests a category but content is limited.

Flag low-confidence files in `knowledge-base/open-questions.md`.
