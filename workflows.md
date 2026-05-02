# 워크플로 예시 (Codex CLI)

## 1) 버그 수정 루프 (표준)

```bash
# 1) 관련 코드 찾기
rg "에러키워드|함수명|로그" .

# 2) 필요한 구간만 읽기
sed -n '1,220p' path/to/file.ts

# 3) 최소 패치 적용
# (Codex가 apply_patch로 수정)

# 4) 가장 좁은 검증부터
npm test -- path/to/related.test.ts
```

커밋:

```bash
git commit -m "fix: handle <case>" -m "AI-Assistant: Codex"
```

## 2) 문서 추가/수정

권장 흐름:
- 템플릿 선택 → 내용 채우기 → 명령/예제 실행 가능성 점검 → 링크/목차 정리

템플릿:
- `templates/change-request.md`
- `templates/debug-runbook.md`

## 3) 리팩터링(조심스럽게)

원칙:
- 기능 변경과 구조 변경 분리
- 단계별로 테스트/검증 포인트 포함

복붙용 프롬프트:
- `agents/refactor-planner.md`

