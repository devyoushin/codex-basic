# Codex CLI 치트시트 (레포 작업)

## 탐색(읽기)

```bash
# 키워드/에러/심볼 검색
rg "keyword" .

# 파일 찾기
find . -maxdepth 4 -type f -name "*keyword*"

# 파일 일부만 보기
sed -n '1,200p' path/to/file

# 최근 변경/히스토리
git status --porcelain=v1
git log --oneline -n 20
git blame -n path/to/file
```

## 변경(쓰기)

- 파일 수정은 `apply_patch`로 “작게, 한 의도씩”
- 새 파일은 템플릿부터(`templates/`)

## 검증(테스트)

원칙: “가장 좁은 것 → 넓게”

```bash
# 예시(프로젝트에 맞게)
npm test -- path/to/test
pytest -k test_name
go test ./...
```

## git (커밋/푸시)

```bash
git add -A
git commit -m "feat: <subject>" -m "AI-Assistant: Codex"
git push
```

## 자주 쓰는 프롬프트(복붙)

- 버그 수정 루프: `agents/bugfixer.md`
- 문서 작성: `agents/doc-writer.md`
- 리팩터링 계획: `agents/refactor-planner.md`
- 테스트 작성: `agents/test-writer.md`

