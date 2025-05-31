# Balancing-VM-Allocation-using-DRL

![NumPy](https://img.shields.io/badge/numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![PyTorch](https://img.shields.io/badge/pytorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![SQLite3](https://img.shields.io/badge/sqlite3-003B57?style=for-the-badge&logo=sqlite&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)

---

# RL_VM_Allocation

강화학습(Deep Reinforcement Learning, DRL) 기반의 VM(가상머신) 할당 및 밸런싱 실험 프로젝트입니다.
데이터센터 환경에서 VM을 효율적으로 할당하여 자원 활용률을 높이고, 서버 부하를 균형 있게 분산시키는 것을 목표로 합니다.

---

## 프로젝트 소개

- 다양한 DRL 알고리즘(Q-learning, DQN, Actor-Critic 등)을 활용해 VM 할당 정책을 학습합니다.
- VM의 자원 요구량, 서버 상태 등 환경 정보를 바탕으로 에이전트가 최적의 할당 결정을 내립니다.
- 실험 결과는 자원 활용률, 부하 밸런싱, 에너지 효율성 등의 지표로 분석합니다.

---

## 개발 환경

- **Python 3.7+**
- 주요 라이브러리: `numpy`, `pandas`, `matplotlib`, `torch` 또는 `tensorflow` (알고리즘별 상이)
- 버전 및 이슈관리: GitHub
- 협업 툴: GitHub Issues, GitHub Projects, Notion

---

## 폴더 및 파일 구조

```
RL_VM_Allocation/
├── Allocation_AC.py           # Actor-Critic 기반 에이전트 및 학습
├── Allocation_Q.py            # Q-learning/DQN 기반 에이전트 및 학습
├── VM_allocation.py           # VM 할당 환경 및 에이전트-환경 상호작용(메인 루프)
├── VmResult.py                # 실험 결과 기록 및 시각화
├── Vmallocation_Q_GPU.py      # GPU 환경에서 Q-learning 실험용 스크립트
└── README.md                  # 프로젝트 설명 및 사용법
```


---

## 주요 파일 설명

- **Allocation_AC.py**
Actor-Critic 방식의 DRL 에이전트 클래스 및 학습 루프 구현
- **Allocation_Q.py**
Q-learning 또는 DQN 방식의 DRL 에이전트 클래스 및 학습 루프 구현
- **VM_allocation.py**
VM 할당 환경(Environment) 정의 및 에이전트와의 상호작용 관리
- **VmResult.py**
실험 결과(자원 사용률, 서버 부하, 누적 보상 등) 저장 및 시각화
- **Vmallocation_Q_GPU.py**
GPU 환경에서 Q-learning 기반 실험을 실행하는 스크립트

---

## 역할 분담

| 이름 | 주요 역할 |
| :-- | :-- |
| 안현준 | Actor-Critic 알고리즘 구현 |
| 최윤수 | 논문 작성, 발표 준비|
| 전진우 | 프로젝트 기획, 설계|


---

## 작업 관리

- GitHub Projects와 Issues를 사용하여 진행 상황을 공유합니다.
- 주간 회의를 통해 작업 순서와 방향성을 논의하고, Notion에 회의 내용을 기록합니다.

---

## 사용 예시

```bash
# Actor-Critic 에이전트로 VM 할당 학습
python Allocation_AC.py

# Q-learning 에이전트로 VM 할당 학습
python Allocation_Q.py
```


---

## 신경 쓴 부분

- 코드 컨벤션: PEP8 및 팀 내 규칙 준수
- 실험 재현성: random seed 고정, 주요 파라미터 config화
- 결과 시각화: 다양한 지표로 실험 결과 분석 및 그래프 제공

---

## 라이선스

MIT License

---

## 문의

이슈 또는 PR로 문의/기여해 주세요!

---

## Contributors

- @user1
- @user2
- @user3
- @user4

---

**© 2025 RL_VM_Allocation Team**

<div style="text-align: center">⁂</div>

[^1]: image.jpg

[^2]: image.jpg

[^3]: paste-3.txt

