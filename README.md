# codex-basic

Codex CLI를 **레포 작업(분석 → 수정 → 검증 → 커밋/푸시)**에 안정적으로 적용하기 위한 개인 학습/운영 공간입니다.

목표:
- 큰 레포에서도 **빠르게 찾고(`rg`)**, **최소 변경으로 고치고(`apply_patch`)**, **테스트로 확인**하는 습관 만들기
- 안전한 명령 실행(샌드박스/승인/파괴적 명령 회피) 루틴 정착
- 작업 결과를 재사용 가능한 규칙/템플릿으로 축적

## 구성

- `AGENTS.md` — Codex가 따라야 할 작업 규칙(진입점)
- `INDEX.md` — 전체 목차
- `codex-guide.md` — Codex CLI 핵심 개념/워크플로
- `workflows.md` — 자주 쓰는 워크플로 예시(디버그/문서/리팩터)
- `dual-setup.md` — Claude/Codex 공존 세팅 가이드
- `advanced-techniques.md` — 고급 패턴(속도/안전/품질)
- `rules/` — 규칙 모음(명령/패치/테스트/커뮤니케이션)
- `templates/` — 반복 작업용 템플릿
- `codexops/` — 작업 로그/대시보드(선택)
- `agents/` — 자주 쓰는 프롬프트(복붙용)
