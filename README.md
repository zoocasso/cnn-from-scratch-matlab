<div align="center">

# 🧠 CNN from Scratch — Pure MATLAB

**No Libraries, No Toolboxes — Mathematics to Matrix Operations**

[![EN](https://img.shields.io/badge/Language-English-blue?style=flat-square)](#-english)
[![KR](https://img.shields.io/badge/언어-한국어-red?style=flat-square)](#-한국어)

</div>

---

## 🇺🇸 English

A Convolutional Neural Network implemented **from the ground up in pure MATLAB** — no Deep Learning Toolbox, no third-party frameworks, no prebuilt autograd. Every layer, every gradient, and every weight update is handwritten as matrix math.

### 📋 Project Overview

Built to internalize the mathematical machinery that deep learning frameworks normally hide behind high-level abstractions. Every forward pass, every backward pass, and every optimizer step was derived on paper and translated directly into matrix operations.

- **Role:** Sole developer — personal research project
- **Core Goal:** Fully implement CNN forward propagation, backpropagation, and gradient-based optimization **without any library assistance**

### 🛠 Tech Stack

| Layer | Technology |
|---|---|
| **Language** | MATLAB |
| **Tooling** | Pure matrix operations — no toolboxes |

### ✨ Key Implementations

#### 1. Convolutional Layer
- **Manual Kernel Operation** — Implemented stride- and padding-aware convolution directly from image-filtering principles, without any built-in `conv` helpers.
- **Multi-Channel Feature Maps** — Built multi-channel input handling and feature-map generation with vectorized matrix operations to minimize loop overhead.

#### 2. Activation & Pooling
- **ReLU / Sigmoid** — Hand-defined both the activation functions and their derivatives so that gradients flow correctly during backpropagation, including control over vanishing-gradient behavior.
- **Max / Average Pooling** — Encapsulated both pooling strategies as reusable functions designed to reduce dimensionality while preserving salient features.

#### 3. Backpropagation from Scratch
- **Chain-Rule Implementation** — Translated partial-derivative chain rules directly into MATLAB code, driving weight and bias updates from raw gradient computation.
- **Gradient Descent Optimizer** — Implemented a baseline gradient-descent loop that iteratively minimizes loss across training batches.

### 💡 Insights Gained

- **Mathematical Transparency** — Developed a structural understanding of how deep learning frameworks internally route tensors, accumulate gradients, and update parameters.
- **Matrix-Level Optimization** — Practiced leveraging MATLAB's matrix-native execution model to replace explicit loops with vectorized operations, measurably improving runtime.

<div align="right"><a href="#-한국어">🇰🇷 한국어로 보기 ↓</a></div>

---

## 🇰🇷 한국어

외부 딥러닝 라이브러리(Deep Learning Toolbox 등)나 프레임워크 없이, **순수 MATLAB의 행렬 연산만으로 바닥부터 구현한 합성곱 신경망(CNN)** 프로젝트입니다. 모든 레이어, 모든 gradient, 모든 weight 업데이트를 수식에서 직접 코드로 옮겼습니다.

### 📋 프로젝트 개요

딥러닝 프레임워크가 고수준 추상화 뒤에 숨기는 수학적 메커니즘을 내재화하기 위해 진행한 프로젝트입니다. 순전파, 역전파, 옵티마이저 스텝을 종이에 유도한 뒤 행렬 연산으로 직접 구현했습니다.

- **역할:** 1인 개발 (개인 연구 프로젝트)
- **핵심 목표:** 라이브러리 없이 CNN의 순전파(Forward), 역전파(Backward), 경사 기반 최적화를 **완전 구현**

### 🛠 기술 스택

| 계층 | 기술 |
|---|---|
| **언어** | MATLAB |
| **도구** | 순수 행렬 연산 — 외부 Toolbox 미사용 |

### ✨ 주요 구현

#### 1. 합성곱 계층 (Convolutional Layer)
- **수동 커널 연산** — 내장 `conv` 계열 함수를 사용하지 않고, 이미지 필터링 원리를 기반으로 Stride와 Padding을 고려한 합성곱을 직접 구현했습니다.
- **다중 채널 특성 맵** — 다채널 입력 처리와 특성 맵 생성 로직을 벡터화된 행렬 연산으로 구성하여 루프 오버헤드를 최소화했습니다.

#### 2. 활성화 함수 및 풀링 (Activation & Pooling)
- **ReLU / Sigmoid** — 활성화 함수와 그 도함수를 직접 정의하여 역전파 시 gradient가 올바르게 전파되도록 했고, 기울기 소실 동작까지 통제 가능하도록 구현했습니다.
- **Max / Average Pooling** — 두 풀링 전략을 재사용 가능한 함수로 캡슐화하여, 주요 특성은 보존하면서 차원을 축소하도록 설계했습니다.

#### 3. 밑바닥부터 구현한 역전파 (Backpropagation from Scratch)
- **체인 룰 구현** — 편미분 체인 룰을 MATLAB 코드로 옮겨, gradient 연산만으로 가중치(Weight)와 편향(Bias)이 업데이트되도록 구축했습니다.
- **Gradient Descent 옵티마이저** — 학습 배치 전반에 걸쳐 손실을 반복적으로 최소화하는 기본 경사하강법 루프를 구현했습니다.

### 💡 얻은 인사이트

- **수학적 투명성** — 딥러닝 프레임워크가 내부적으로 텐서를 어떻게 라우팅하고, gradient를 누적하며, 파라미터를 업데이트하는지 구조적으로 이해하게 되었습니다.
- **행렬 레벨 최적화** — MATLAB의 행렬 네이티브 실행 모델을 활용해 명시적 루프를 벡터화 연산으로 대체함으로써 실측 런타임 개선을 확인했습니다.

<div align="right"><a href="#-english">🇺🇸 View in English ↑</a></div>
