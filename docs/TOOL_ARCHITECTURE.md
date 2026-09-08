# Tool Architecture

## 역할 분리

| 시스템 | 정식 역할 | 저장·처리 범위 |
|---|---|---|
| ChatGPT | Chief Strategist / Board | 전략, Monthly·Quarterly Review, 병목, 반대논리, 중요 판단 |
| Claude | Deep Work / Critic | 장문 자료, 리서치, Brand Bible, 비판과 통합 |
| Codex | System Builder | 코드, 자동화, API, Agent Infrastructure, Dashboard, Integration, Testing |
| Hermes | Personal COO | Daily Brief, Universal Inbox, 반복 작업, 주간·월간 보고, Agent Coordination |
| Git Markdown | 공통 기준 | 전략·규칙·계약·변경 이력 |
| Notion | Operational DB | States, Monthly Contract, KPI, Pipeline, Content, Customer, Projects |
| Obsidian | Long-Term Mind | Book Notes, 생각, 철학, Evergreen Notes, Insight |
| Calendar | 시간 실행 계층 | 반복 약속, Deep Work Block, 가족·운동 일정 |

## 데이터 흐름

```text
Capture → Classify → Prioritize → Schedule → Execute → Review
```

사용자는 방향 결정·실행·관계와 관련된 판단을 담당합니다. AI는 정리·수집·분석·리마인드·초안·일정 후보·보고를 담당합니다.

## 경계 규칙

- Git 문서는 실행 데이터의 일일 저장소가 아닙니다.
- Notion과 Obsidian에 같은 운영 정보를 이중 관리하지 않습니다.
- AI는 사업 선택, 퇴사, 투자, 가족의 삶을 최종 결정하지 않습니다.
- 새 아이디어는 현재 Mission과 직접 관련되지 않으면 Inbox 또는 Parking Lot으로 보냅니다.
