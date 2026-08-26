# Evaluator-Optimizer Workflow

```text
요구사항 → Generator 초안 → Evaluator 검사
                              ├─ pass → 완료
                              └─ revise → 피드백 반영 → 재검사
```

단순 Verifier는 통과와 거절에서 끝날 수 있지만, Evaluator-Optimizer는 평가 피드백을 다음 생성 입력으로 사용합니다. 무한 반복을 막기 위해 재시도 횟수와 실패 후 행동을 정합니다.
