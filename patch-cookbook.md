# `apply_patch` Cookbook

Codex에서 파일 수정은 `apply_patch`가 기본입니다. 실수/충돌을 줄이고 “변경 의도”를 명확히 남깁니다.

## 1) 새 파일 추가

```diff
*** Begin Patch
*** Add File: path/to/new-file.md
+# Title
+내용
*** End Patch
```

## 2) 기존 파일 수정

```diff
*** Begin Patch
*** Update File: path/to/file.md
@@
-old
+new
*** End Patch
```

## 3) 파일 삭제

```diff
*** Begin Patch
*** Delete File: path/to/obsolete.md
*** End Patch
```

## 4) 파일 이동(리네임)

```diff
*** Begin Patch
*** Update File: old/path.md
*** Move to: new/path.md
@@
 (필요하면 내용 수정도 같이)
*** End Patch
```

## 권장 패턴

- 큰 변경은 2~3개 패치로 분리(포맷/리팩터링/로직/테스트)
- “왜 필요한지”가 불명확한 변경은 하지 않기

