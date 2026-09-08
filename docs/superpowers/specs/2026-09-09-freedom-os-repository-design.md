# Freedom OS Repository Design

## 목적

Codex, Claude, ChatGPT, Hermes가 동일한 전략·상태·운영 규칙을 읽고 사용할 수 있는 Git 기반 Markdown 저장소를 만든다.

## 원칙

- Git 저장소의 Markdown은 전략과 규칙의 Source of Truth다.
- 실행 데이터는 향후 Notion이 담당한다.
- 장기 지식과 개인 메모는 Obsidian이 담당한다.
- 같은 정의를 여러 문서에 복사하지 않고, 각 문서가 기준 문서를 링크한다.
- 미정 값은 추측하지 않고 `TBD`로 남긴다.
- 초기 범위는 Skeleton이며, 앱·API·자동화 구현은 포함하지 않는다.

## 문서 경계

- `docs/FREEDOM_OS_SPEC.md`: 전체 시스템 개요와 문서 지도
- `docs/NORTH_STAR.md`: 목적, 삶의 목표, Freedom Gate
- `docs/LANDSCAPE_MAP.md`: 현재 상태와 미확정 영역
- `docs/STATE_MACHINE.md`: 상태, 전이, 판정 규칙
- `docs/TOOL_ARCHITECTURE.md`: 도구별 역할과 데이터 경계
- `docs/REVIEW_SYSTEM.md`: 검토 주기와 의사결정 권한
- `agents/`: 에이전트의 역할과 출력 계약
- `schemas/`: 데이터 구조와 필드 계약

## 향후 확장

Financial Deep Dive, Notion 연동, Hermes 자동화, 코드·API는 별도 변경으로 추가한다. 이 초기 커밋에서 개인 금융 수치나 민감한 운영 데이터는 저장하지 않는다.
