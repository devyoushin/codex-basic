# Codex 학습 공간

> 목적: Codex CLI를 “안전하고 빠른 레포 작업자”로 쓰기 위한 규칙/템플릿/런북 축적

---

## 0. 먼저 볼 것

- `AGENTS.md` — 이 폴더에서 Codex가 따라야 하는 규칙(가장 중요)
- `docs/guides/codex-guide.md` — Codex CLI 개념 + 표준 작업 흐름

---

## 1. 가이드

- `docs/guides/codex-guide.md` — 핵심 개념/워크플로
- `docs/guides/workflows.md` — 작업 유형별 예시
- `docs/guides/dual-setup.md` — Claude/Codex 공존 운영
- `docs/guides/cheatsheet.md` — 명령/패턴 치트시트
- `docs/guides/patch-cookbook.md` — `apply_patch` 예제
- `docs/guides/sandbox-escalation.md` — 승인/권한 감각
- `docs/guides/advanced-techniques.md` — 고급 활용(속도/품질/안전)

---

## 2. 규칙

- `docs/rules/README.md` — 규칙 인덱스
- `docs/rules/command-rules.md` — 쉘 명령 원칙(`rg` 우선, 파괴적 명령 금지 등)
- `docs/rules/patch-rules.md` — `apply_patch` 사용 규칙(작고 안전한 패치)
- `docs/rules/testing-rules.md` — 테스트/검증 순서
- `docs/rules/repo-rules.md` — git/브랜치/커밋 메시지 규칙
- `docs/rules/communication-rules.md` — 사용자와의 커뮤니케이션 스타일(짧고 직접)
- `docs/rules/safety-rules.md` — 승인/권한/보안 주의사항

---

## 3. 템플릿

- `docs/templates/change-request.md` — 변경 요청 정리 템플릿
- `docs/templates/debug-runbook.md` — 재현/원인/수정/검증 런북
- `docs/templates/review-checklist.md` — PR/패치 리뷰 체크리스트

---

## 4. 에이전트 프롬프트

- `docs/agents/bugfixer.md` — 버그 수정 루프
- `docs/agents/doc-writer.md` — 문서 작성
- `docs/agents/refactor-planner.md` — 리팩터링 계획
- `docs/agents/test-writer.md` — 테스트 작성

---

## 5. Ops (선택)

- `ops/log.md` — 세션 로그(무엇을/어떻게/어떤 결과로)
- `ops/dashboard.md` — 누적 현황(월별/유형별)
- `ops/budget.md` — 시간/작업량 예산(토큰/비용은 선택)
