# 강사 진행안

1. Generator와 Evaluator의 출력 책임을 구분합니다.
2. 1차 초안에서 누락된 기준을 먼저 찾습니다.
3. Evaluator 피드백이 2차 Generator 입력으로 실제 전달됐는지 비교합니다.
4. pass 조건과 최대 2회 한도를 확인합니다.
5. 단순 Verifier와 달리 피드백을 다음 생성에 사용하는 점을 설명합니다.

핵심 질문: 평가 결과를 다시 생성에 사용하지 않는다면 Evaluator-Optimizer라고 부를 수 있는가?
