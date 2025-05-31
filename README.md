# Balancing-VM-Allocation-using-DRL

1. 전체 코드 구조 설계도

RL_VM_Allocation/
│
├── Allocation_AC.py         # Actor-Critic 기반 에이전트 정의 및 학습
├── Allocation_Q.py          # Q-learning/DQN 기반 에이전트 정의 및 학습
├── VM_allocation.py         # 환경 시뮬레이션 및 에이전트-환경 상호작용(메인 루프)
├── VmResult.py              # 실험 결과 기록 및 시각화
├── Vmallocation_Q_GPU.py    # GPU 환경에서 Q-learning 실험용 스크립트
└── README.md                # 프로젝트 설명 및 사용법
2. 각 파일별 역할 및 상호작용
Allocation_AC.py

Actor-Critic 방식의 DRL 에이전트 클래스 및 학습 루프 구현

상태(state) → 액션(action) → 보상(reward) → 정책(policy) 업데이트

VM 할당 정책을 신경망 기반으로 학습

Allocation_Q.py

Q-learning 또는 DQN 방식의 DRL 에이전트 클래스 및 학습 루프 구현

상태-행동 가치함수(Q-table 또는 Q-network) 업데이트

VM 할당을 위한 최적 정책 탐색

VM_allocation.py

VM 할당 환경(Environment) 정의

상태: 각 VM의 요구사항, 각 서버의 자원 상태 등

액션: 특정 VM을 특정 서버에 할당

보상: 자원 활용률, 부하 균형, 에너지 효율 등

에이전트와 환경의 상호작용 관리 (학습/평가 루프)

실험 파라미터 설정 및 반복 실행

VmResult.py

실험 결과(자원 사용률, 서버 부하, 누적 보상 등) 저장 및 시각화

다양한 실험 결과를 비교/분석하는 기능

Vmallocation_Q_GPU.py

GPU 환경에서 Q-learning 기반 실험을 실행하는 별도 스크립트

대규모 실험 또는 고속 학습에 활용

README.md

프로젝트 개요, 환경 세팅, 실행 방법, 각 파일 설명, 참고 문헌 등 문서화

