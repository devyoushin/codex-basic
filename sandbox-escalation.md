# 샌드박스/승인(에스컬레이션) 가이드

Codex CLI 환경에선 “로컬 파일 읽기/편집”은 가능하지만, **네트워크**나 **시스템 영향이 큰 작업**은 승인(에스컬레이션)이 필요할 수 있습니다.

## 자주 승인이 필요한 작업

- `git push`, `git pull` 등 원격 접근
- 패키지 설치/다운로드(`npm install`, `pip install`, `go get` 등)
- 외부 API 호출, 원격 리소스 접근

## 승인을 요청할 때 원칙

- “왜 필요한지”를 1문장으로 명확히
- 가능한 경우 **좁은 prefix**로 승인 범위를 제한(예: `git push`)
- 파괴적 명령은 prefix rule 요청하지 않기

## 안전 장치(권장)

- 원격 작업 전: `git status --porcelain=v1`, `git diff --stat`로 변경 범위 확인
- 푸시 전: 브랜치 확인 `git rev-parse --abbrev-ref HEAD`

