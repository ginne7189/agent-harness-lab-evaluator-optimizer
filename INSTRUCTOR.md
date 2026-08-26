# 강사 진행안

1. Generator와 Evaluator의 출력 책임을 구분합니다.
2. 1차 초안에서 누락된 기준을 먼저 찾습니다.
3. Evaluator 피드백이 2차 Generator 입력으로 실제 전달됐는지 비교합니다.
4. pass 조건과 최대 2회 한도를 확인합니다.
5. 단순 Verifier와 달리 피드백을 다음 생성에 사용하는 점을 설명합니다.

핵심 질문: 평가 결과를 다시 생성에 사용하지 않는다면 Evaluator-Optimizer라고 부를 수 있는가?

## Codex 실행 진행 순서

1. Codespaces를 열고 `AGENTS.md`, `knowledge/index.md`, 해당 `SKILL.md`, `templates/result.md`를 차례로 보여 줍니다.
2. `LAB.md`의 정상 입력 프롬프트를 Codex 채팅에 입력합니다.
3. 생성된 `work/normal-result.md`에서 평가 피드백과 반복 한도를 설명합니다.
4. `LAB.md`의 정보 부족·실패 입력 프롬프트를 실행합니다.
5. `work/failure-result.md`를 정상 결과와 나란히 놓고, 추측하지 않고 멈춘 위치를 확인합니다.
6. 파일을 직접 수정하는 활동은 하지 않고, 개인 프로젝트에서 어느 파일을 바꿀지 연결합니다.

## 실행이 정상인지 확인하는 기준

- 결과가 `templates/result.md`의 항목을 모두 사용합니다.
- `examples/`에 없는 정보는 새 사실처럼 만들어지지 않습니다.
- `policies/`의 중단·금지·사람 확인 조건이 결과에 드러납니다.
- 결과 파일이 `work/`에 생성됩니다.
