---
layout: post
title: ResNet Paper Review
tags: [Paper_Review]
excerpt_separator: <!--more-->
---  
Review: 
<!--more-->
# ResNet: Deep Residual Learning for Image Recognition
- References
	- He, Kaiming, et al. "Deep residual learning for image recognition." (2015). [[pdf]](https://arxiv.org/pdf/1512.03385.pdf)

## Abstract
- 깊은 신경망일수록 학습이 더 어렵다.
- 이전의 신경망보다 깊지만 학습은 더 쉬운 residual learning framework를 소개한다.
- 레이어의 입력에 관련하여 레이어가 residual function을 학습하도록 레이어를 재구성했다.
- 실증적인 증거를 바탕으로 residual network이 최적화하기 쉽고, 상당히 깊은 망에서도 정확도를 더 획득한다는 것을 보여준다.
- ImageNet 데이터셋에서 VGGNet보다 8배 정도 깊은, 152 layers의 깊이로 residual net을 쌓았지만, 여전히 상대적으로 덜 복잡한 구조를 유지했다. 
- ImageNet 2015 챌린지에서 1위.

## 1. Introduction
- 딥러닝 CNN이 이미지 분류에서 뛰어난 성과를 보임. 최근 연구들이 깊은 망의 모델들로 ImageNet 챌린지에서 높은 성과를 보여주며, 망 깊이의 중요성에 대한 보여줌.
- "레이어를 더 쌓으면 망이 학습을 더 잘하는가?"(아... 영어 이자식이 또?) 라는 질문을 가지게 됨.
- 이 질문에 답을 구하기 위해 vaanishing/exploding gradients 문제를 해결해야함. 
	- 이미 해결을 위해 normalized initialization, SGD와 back propagation을 통한 intermediate normalization layers 등이 논의됨.
- 더 깊은 망에서 수렴이 시작될 때, 학습 정확도에 degradation(성능저하)이 일어나기 시작함. 이런 정확도 저하가 overfitting으로 인함이 아니며, 레이어를 더할수록 training error가 더 높아지는 문제가 발견됨.
- 학습 중 정확도 저하는 

## 2. Related Work
**Residual Representations**   
- ...

**Shortcut Connections**   
- ...


## 3. Deep Residual Learning
### 3.1. Residual Learning
### 3.2. Identity Mapping by Shortcuts
### 3.3. Network Architectures
**Plain Network**   
- ...

**Residual Network**   
- ...

### 3.4. Implementation

## 4. Experiments
### 4.1. ImageNet Classification
**Plain Networks**   
- ...
**Residual Networks**   
- ...
**Identity vs. Projection Shortcuts**   
- ...
**Deeper Bottleneck Architectures**   
- 50-layer ResNet
- 101-layer and 152-layer ResNets
**Comparisions with State-of-the-art Methods**   
- ...

### 4.2. CIFAR-10 and Analysis
**Analysis of Layer Responses**   
- ...
**Exploring Over 1000 layers**   
- ...

### 4.3. Object Detection on PASCAL and MS COCO