# Evaluator-Optimizer Workflow

> 강사와 함께 1차 초안, 평가 피드백, 수정 결과, 반복 한도 도달을 순서대로 확인하는 공통 실습입니다.

```text
요구사항 → Generator 초안 → Evaluator 검사
                              ├─ pass → 완료
                              └─ revise → 피드백 반영 → 재검사
```

단순 Verifier는 통과와 거절에서 끝날 수 있지만, Evaluator-Optimizer는 평가 피드백을 다음 생성 입력으로 사용합니다. 무한 반복을 막기 위해 재시도 횟수와 실패 후 행동을 정합니다.

## Harness 구조를 보는 순서

1. `AGENTS.md`: 모든 역할이 지켜야 할 공통 목표와 금지 행동
2. `knowledge/index.md`: 이 패턴을 사용하는 조건과 사용하지 않을 조건
3. `roles/`: 역할별 책임과 하지 않을 일
4. `contracts/`: 다음 단계에 넘기는 값과 필수 형식
5. `policies/`: 재시도·중단·사람 확인 경계
6. `.agents/skills/evaluator-optimizer/SKILL.md`: 실제 처리 순서와 완료 조건
7. `examples/`: 정상 요청과 실패 요청의 기대 결과
8. `work/`: 개인 프로젝트 결과를 저장할 위치

공통 실습에서는 완성된 파일을 강사와 함께 읽습니다. 각 파일을 자신의 업무로 바꾸는 활동은 개인 프로젝트에서 진행합니다.
