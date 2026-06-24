# Knowledge Base Schema

Create or update `knowledge-base/work-knowledge-base.md` with this structure.

```markdown
# 업무 지식베이스

## 1. 한 줄 정의

## 2. 업무 목적

## 3. 근거 문서 목록

## 4. 연간 흐름

| month | 해야 할 일 | 근거 | 확인 필요 |
| --- | --- | --- | --- |

## 5. 월별 체크리스트

## 6. 필요한 서식

| form | when used | source | notes |
| --- | --- | --- | --- |

## 7. 관련 부서와 역할

## 8. 작년 운영 방식

## 9. 교육청 매뉴얼 기준

## 10. 매뉴얼과 작년 방식의 차이

## 11. 위험과 누락 가능성

## 12. 확인해야 할 질문

## 13. 출처
```

## Extraction Rules

- Separate official requirements from last year's local practice.
- Keep dates exact when the source gives exact dates.
- If the source gives only a month or sequence, mark it as approximate.
- Use `source path + section/title/page if available` for evidence.
- Do not invent a 담당자. If the document only implies a role, write "추정" and explain why.

## Conflict Handling

When two sources disagree:

1. Prefer current official manuals over older local practice for compliance.
2. Preserve last year's practice as operational context.
3. Add the conflict to `handover-package/manual-vs-practice-diff.md`.
4. Add a verification question for the responsible department.
