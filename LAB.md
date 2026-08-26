# 실습 B-4 — Evaluator-Optimizer 완성형 함께 읽기

## 함께 확인할 결과

강사가 1차 결과, 평가 피드백, 수정 결과를 순서대로 보여 줍니다. 수강생은 평가 이유가 다음 수정 입력으로 전달되고, 반복 한도에 도달하면 사람 검토로 끝나는 과정을 확인합니다.

## 강사와 함께 확인

1. 완성된 Generator 출력과 Evaluator 출력의 항목을 비교합니다.
2. 네 가지 평가 기준이 `pass` 또는 `revise`로 표시되는지 확인합니다.
3. `revise` 이유가 다음 Generator 입력에 들어가는 위치를 확인합니다.
4. 최대 2회 후에도 통과하지 못하면 사람 검토로 끝나는 Trace를 확인합니다.

## 함께 확인을 마치는 기준

- 단순 거절이 아니라 수정 이유가 다음 입력으로 전달됩니다.
- 최대 반복 횟수와 실패 후 행동이 있습니다.

## Codex로 완성 예시 실행하기

### 정상 입력

```text
AGENTS.md, knowledge/index.md, .agents/skills/evaluator-optimizer/SKILL.md를 확인하세요. examples/input-normal.md의 초안을 평가 기준으로 검사하고, revise 이유를 반영한 수정 결과를 templates/result.md 형식으로 work/normal-result.md에 작성하세요. 최대 반복 횟수는 2회입니다.
```

### 정보 부족·실패 입력

```text
examples/input-failure.md를 처리해 work/failure-result.md를 작성하세요. 근거 없는 수치를 새 근거 없이 고치거나 통과시키지 말고, 반복 한도 이후 사람 확인으로 끝내세요.
```

### 결과에서 확인할 것

평가 이유가 다음 수정 입력으로 이어집니다. 근거가 없는 수치는 반복해도 자동 통과하지 않으며 한도 후 사람 확인으로 끝납니다.
