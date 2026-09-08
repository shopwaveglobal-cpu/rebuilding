# Freedom OS / 1IM Life OS

AI, 시스템, 사람, 자본을 활용해 직접 해야 하는 일을 줄이고, 가족·경험·창작·사업에 쓸 시간을 확보하기 위한 개인 운영체계입니다.

## 빠른 시작

1. [전체 사양](docs/FREEDOM_OS_SPEC.md)을 먼저 읽습니다.
2. [North Star](docs/NORTH_STAR.md)에서 고정된 목표와 Freedom Gate를 확인합니다.
3. [Landscape Map](docs/LANDSCAPE_MAP.md)에서 현재 상태와 미정 사항을 확인합니다.
4. 작업을 추가하기 전에 [State Machine](docs/STATE_MACHINE.md)과 [Review System](docs/REVIEW_SYSTEM.md)을 확인합니다.

## Source of Truth

| 영역 | 기준 문서 또는 시스템 |
|---|---|
| 목표·가치·Freedom Gate | `docs/NORTH_STAR.md` |
| 현재 상태·Gap·Unknown | `docs/LANDSCAPE_MAP.md` |
| 상태·전이·승급 기준 | `docs/STATE_MACHINE.md` |
| 도구 역할·데이터 경계 | `docs/TOOL_ARCHITECTURE.md` |
| 검토 주기·결정 권한 | `docs/REVIEW_SYSTEM.md` |
| 에이전트 행동 규칙 | `agents/` |
| 데이터 필드 계약 | `schemas/` |
| 실행 데이터 | Notion — 별도 운영 DB |
| 장기 지식·메모 | Obsidian — 별도 지식 저장소 |

첨부 Seed Brief의 상세 Landscape Agent Briefs, Initial Landscape, Unknown Queue, Next Deep-Dive Order는 [`docs/SEED_BRIEF_LANDSCAPE.md`](docs/SEED_BRIEF_LANDSCAPE.md)에 보존합니다.

## 도구별 사용

- ChatGPT: 전략, 검토, 중요한 판단
- Claude: 장문 분석, 리서치, 비판적 검토
- Codex: 코드, 자동화, 통합, 테스트
- Hermes: 반복 운영, Inbox, 브리핑, 보고

## 상태 표기

- `TBD`: 아직 결정하지 않은 값
- `Hypothesis`: 검증 전 가설
- `Active`: 현재 실행 중인 항목
- `Parking Lot`: 아이디어이지만 지금 실행하지 않는 항목
- `Trigger`: 특정 조건에서만 활성화할 항목

## 변경 원칙

문서가 충돌하면 더 좁은 문서가 더 넓은 문서보다 우선하지 않습니다. 정의의 기준 문서를 수정하고, 다른 문서는 링크와 요약만 유지합니다. 주요 결정은 [Decision Log](changelog/DECISIONS.md)에 기록합니다.
