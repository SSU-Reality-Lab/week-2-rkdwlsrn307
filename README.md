[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/CwAYw1mA)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=20659797&assignment_repo_type=AssignmentRepo)
# 📘 프로젝트 : 확률과 시뮬레이션

이 프로젝트는 정규분포, 확률 계산, 몬테카를로 시뮬레이션, 다변량 정규분포를 다루는 과제입니다. `Week_2_Machine_learning_2025.ipynb` 노트북을 기반으로 하며, 각 Assignment는 통계적 개념을 코드로 실습하도록 구성되어 있습니다.

---

## ⚙️ 실습 환경 설정

과제 수행에 필요한 개발 환경을 설정합니다. `conda`를 사용하여 프로젝트별 가상 환경을 구성하는 것을 권장합니다.  
아래 환경으로 실습을 진행하면서 에러가 발생하면 조교에게 문의하세요.  
아래 환경을 따르지 않아 발생한 문제는 답변하지 않습니다.

1. **Conda 가상 환경 생성**
    ```bash
    conda create --name ml_2025 python=3.10 -y
    ```

2. **가상 환경 활성화**
    ```bash
    conda activate ml_2025
    ```

3. **필요한 라이브러리 설치**
    ```bash
    pip install ipykernel
    python -m ipykernel install --user --name=ml_2025 --display-name "Python (ml_2025)"
    ```

---

## 🎯 구현 목표

`Week_2_Machine_learning_2025.ipynb` 노트북 안에 포함된 4개의 Assignment를 완성하세요.  
AI 도구를 이용하기보다는 직접 코드를 작성하며 통계적 개념을 체득하는 것을 추천합니다.

- Assignment 1: 정규분포 비교  
- Assignment 2: 표준 정규분포 확률 계산  
- Assignment 3: Monte Carlo로 π 근사  
- Assignment 4: 다변량 정규분포 시각화
- Assignment 5: 정규화 계수가 모델의 복잡도와 일반화 성능에 미치는 영향을 분석하고 설명하기

---

## 🚀 실행 및 테스트 방법

1. **Jupyter Notebook 실행**
    ```bash
    jupyter notebook Week_2_Machine_learning_2025.ipynb
    ```

2. **각 Assignment 문제 풀이**
    - 지정된 셀 안의 코드를 완성합니다.  
    - 그래프나 수식 결과를 확인하세요.  

3. **출력 확인**
    - Assignment 1: 여러 정규분포 곡선이 한 그래프에 표시되는지 확인합니다.  
    - Assignment 2: \(P(-2<Z<2)\) 값이 올바르게 계산되는지 확인합니다.  
    - Assignment 3: Monte Carlo로 추정한 π 값이 3.14 근처에 수렴하는지 기록합니다.
    - Assignment 4: 분산 구조가 반영된 다변량 정규분포 시각화가 출력되는지 확인합니다.  
    - Assignment 5: 분산 구조가 반영된 다변량 정규분포 시각화가 출력되는지 확인합니다.  

---

## 📂 Assignment 세부 설명

### 📝 Assignment 1: 정규분포 비교
여러 개의 정규분포를 생성하여 그래프로 비교합니다.  
- 평균과 표준편차를 바꿔가며 곡선의 이동과 형태 변화를 관찰하세요.  
- 각 곡선은 다른 색상과 범례(legend)로 구분하세요.  

---

### 📝 Assignment 2: 표준 정규분포 확률 계산
표준 정규분포 \(Z \sim N(0,1)\)에서  
확률 \(P(-2 < Z < 2)\) 를 계산합니다.  
- `Normal().cdf` 함수만 사용 가능합니다.  
- 다른 함수 사용 시 0점 처리됩니다.  

---

### 📝 Assignment 3: Monte Carlo로 π 근사
몬테카를로 시뮬레이션으로 원주율 \(\pi\) 를 근사합니다.  
- 점의 개수(`number_of_drops`)를 점차 늘려가며 수렴 과정을 확인합니다.  
- π 값이 3.14 근처에 수렴하기 시작하는 지점을 기록하세요.  

---

### 📝 Assignment 4: 다변량 정규분포 시각화
2차원 다변량 정규분포를 생성하고 시각화합니다.  
- \(X\)의 분산 = 2  
- \(Y\)의 분산 = 4  
- 결과는 제시된 예시 이미지와 유사해야 합니다.  

---

### 📝 Assignment 5: 정규화 계수(Regularizer Strength)

모델 학습 과정에서 정규화 계수의 역할과 최적 선택 방법을 탐구하세요.

1. **정규화 계수 선택**  
   - 모델 학습에서 정규화 계수(regularizer strength)를 어떻게 선택하는 것이 최적일까요?  

2. **계수 크기에 따른 영향**  
   - 정규화 계수가 너무 작은 경우 모델에 어떤 영향을 줄까요?  
   - 정규화 계수가 너무 큰 경우 모델에 어떤 영향을 줄까요?  
 
---

## 📤 과제 제출

- 레포를 로컬에 pull 받은 후, 노트북의 각 Assignment 셀을 완성하세요.  
- 그래프와 계산 결과가 포함된 상태로 저장합니다.  
- push를 하면 자동으로 과제가 제출됩니다.  

---

## 🚨 주의사항
과제의 목표는 **직접 코드 구현을 통해 개념을 이해하는 것**입니다.  
따라서 다음과 같은 경우 0점 처리될 수 있습니다.  

- 고수준 라이브러리 함수를 사용하여 문제를 한 줄로 해결한 경우  
- 노트북에 코드 실행 결과나 그래프가 포함되지 않은 경우  

