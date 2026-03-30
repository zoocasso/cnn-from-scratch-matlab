# 🧠 CNN from Scratch (MATLAB)
> **No Libraries, No Frameworks — Pure Mathematical Implementation**

외부 딥러닝 라이브러리(Deep Learning Toolbox 등)나 프레임워크를 전혀 사용하지 않고, **MATLAB만을 이용하여 바닥부터 구현한 합성곱 신경망(CNN)** 프로젝트입니다.

---

## 📋 프로젝트 개요 (Project Overview)
추상화된 함수 뒤에 숨겨진 CNN의 수학적 원리와 역전파(Backpropagation) 메커니즘을 완벽히 이해하기 위해 진행한 프로젝트입니다. 행렬 연산만을 이용하여 직접 레이어를 설계하고 학습 프로세스를 구축했습니다.

* **역할:** 개인 프로젝트 (Sole Developer)
* **핵심 목표:** 라이브러리 없이 CNN의 순전파(Forward) 및 역전파(Backward) 알고리즘 완벽 구현

## 🛠 기술 스택 (Tech Stack)
* **Language:** MATLAB
* **Tool:** Pure Matrix Operations (No Toolboxes)

## ✨ 주요 구현 특징 (Key Implementations)

### 1. 합성곱 계층 (Convolutional Layer)
* **Manual Kernel Operation:** 가이트 이미지 필터링 원리를 응용하여 스트라이드(Stride)와 패딩(Padding)을 고려한 커널 연산을 직접 구현했습니다.
* **Feature Map Generation:** 다중 채널 입력을 처리하고 특성 맵을 생성하는 로직을 행렬 연산 최적화를 통해 구성했습니다.

### 2. 활성화 함수 및 풀링 (Activation & Pooling)
* **ReLU / Sigmoid:** 비선형 활성화 함수와 그 도함수(Derivative)를 직접 정의하여 역전파 시 기울기 소실 문제를 제어했습니다.
* **Max/Average Pooling:** 정보 손실을 최소화하면서 차원을 축소하는 풀링 레이어를 함수화했습니다.

### 3. 역전파 알고리즘 (Backpropagation from Scratch)
* **Chain Rule Implementation:** 편미분을 이용한 체인 룰을 코드로 옮겨, 가중치(Weights)와 편향(Bias)이 학습 데이터에 따라 업데이트되는 최적화 과정을 구현했습니다.
* **Optimizer:** 기본적인 경사하강법(Gradient Descent)을 통해 오차를 최소화하도록 설계했습니다.

## 💡 인사이트 (Insights)
* **수학적 원리 이해:** 딥러닝 프레임워크가 내부적으로 데이터를 어떻게 처리하는지 구조적으로 이해하게 되었습니다.
* **행렬 연산 최적화:** MATLAB의 강점인 행렬 연산을 활용하여 루프를 최소화하고 연산 속도를 높이는 최적화 기법을 익혔습니다.

---
