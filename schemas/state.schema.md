# State Schema

| 필드 | 필수 | 설명 |
|---|---|---|
| `area` | 예 | Energy, Business, Brand, Learning, Risk, Leverage 중 하나 |
| `state_id` | 예 | 예: `B1` |
| `label` | 예 | 사람이 읽는 상태명 |
| `evidence` | 예 | 상태를 뒷받침하는 관찰·수치·사실 |
| `bottleneck` | 예 | 현재 가장 큰 제한 요소 |
| `next_transition` | 예 | 다음 상태로 가기 위한 검증 조건 |
| `owner` | 예 | 사용자 또는 담당 Agent |
| `review_date` | 예 | 다음 검토일 `TBD` |
| `status` | 예 | Active, Hold, Parked, Complete |
