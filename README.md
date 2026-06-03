# codex-basic

Codex CLI를 레포 작업에 안정적으로 적용하기 위한 개인 학습/운영 공간입니다.

핵심 흐름은 **분석 → 수정 → 검증 → 정리**입니다. 큰 레포에서도 빠르게 찾고(`rg`), 필요한 만큼만 고치고(`apply_patch`), 테스트로 확인하는 작업 습관을 정리합니다.

## 빠른 시작

- `CLAUDE.md` — Claude/Codex가 함께 참고할 기본 작업 규칙 원본
- `AGENTS.md -> CLAUDE.md` — Codex/agent 진입점 링크
- `INDEX.md` — 전체 문서 목차
- `docs/guides/codex-guide.md` — Codex CLI 핵심 개념과 표준 작업 흐름

## 폴더 구조

```text
codex-basic/
├── README.md
├── INDEX.md
├── CLAUDE.md
├── AGENTS.md -> CLAUDE.md
├── docs/
│   ├── guides/     # 학습/참고 문서
│   ├── rules/      # 작업 규칙
│   ├── templates/  # 반복 작업 템플릿
│   └── agents/     # 복붙용 역할 프롬프트
└── ops/            # 로그, 대시보드, 예산
```

## 문서 위치

- `docs/guides/` — 가이드, 워크플로, 치트시트, 패치 예제, 샌드박스/승인 가이드
- `docs/rules/` — 명령, 패치, 테스트, git, 커뮤니케이션, 안전 규칙
- `docs/templates/` — 변경 요청, 디버그 런북, 리뷰 체크리스트
- `docs/agents/` — 문서 작성, 버그 수정, 테스트 작성, 리팩터 계획용 프롬프트
- `ops/` — 세션 로그, 누적 현황, 작업량 예산
