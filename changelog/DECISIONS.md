# Decision Log

주요 구조·전략 결정만 기록합니다. 실행 데이터와 아이디어 목록은 이 파일에 저장하지 않습니다.

## 2026-09-09 — Git을 공통 Source of Truth로 채택

- 상태: Accepted
- 결정: Codex, Claude, ChatGPT, Hermes가 공통으로 읽는 기준을 Git Markdown으로 둡니다.
- 이유: 대화 기록과 도구별 메모의 분산을 줄이고 문서 변경을 추적하기 위해서입니다.
- 경계: Notion은 실행 DB, Obsidian은 장기 지식으로 유지합니다.

## 2026-09-09 — 초기 범위를 Skeleton으로 제한

- 상태: Accepted
- 결정: 초기 커밋에는 문서·계약·에이전트 지침만 넣고 자동화·앱·API는 추가하지 않습니다.
- 이유: Freedom OS 구축 자체가 생산적 미루기가 되는 것을 방지하기 위해서입니다.
