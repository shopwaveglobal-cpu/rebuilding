# State Machine

상태는 단순한 선형 등급이 아니라 `현재 상태 + 병목 + 증거`로 판단합니다. 상태 정의와 승급 조건은 이 문서를 정본으로 둡니다.

## Business State

```text
B0 Thesis
  ↓
B1 Problem
  ↓
B2 Offer
  ↓
B3 Repeat Sales
  ↓
B4 0.5S
  ↓
B5 1S
  ↓
B6 2S
  ↓
B7 3S
  ↓
B8 3S × 6 Months
  ↓
Freedom Candidate
```

### 판정 원칙

- 각 상태는 숫자만으로 승급하지 않고 증거를 요구합니다.
- 증거의 구체 형식은 상태별로 `TBD`이며, 첫 검증 주기에 정합니다.
- 매월 `PASS`, `HOLD`, `PIVOT`, `KILL`, `EXPAND` 중 하나를 선택합니다.
- State를 바꾸는 결정과 실행 방법을 바꾸는 결정은 분리합니다.

## Mission State

- `Proposed`: 아이디어 또는 후보
- `Active`: 현재 90-Day Mission에 포함
- `Blocked`: 외부 조건·지식·결정 때문에 진행 중단
- `Review`: 주간 또는 월간 검토 대상
- `Complete`: 정의된 완료 조건 충족
- `Parked`: 지금 실행하지 않음
- `Killed`: 중단하고 재개 조건도 없음

## 전이 규칙

1. 아이디어는 기본적으로 `Proposed`로 수집합니다.
2. 현재 병목과 직접 연결되고 Capacity가 있을 때만 `Active`로 승격합니다.
3. Active Mission은 기본 최대 2개입니다.
4. Blocked 상태에서 필요한 최소 학습 또는 지원만 추가합니다.
5. 새 프로젝트를 추가하려면 기존 Mission 하나를 Parked 또는 Killed로 내려야 합니다.
