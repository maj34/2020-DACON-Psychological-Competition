# 월간 데이콘 심리 성향 예측 AI 경진대회
2020-DACON-Psychological-Competition 

<br/>

## 1. 배경 & 목적

- 심리학 테스트의 범주가 넓어짐에 따라 해당 영역의 데이터 분석 방법 탐구
- 국가 선거 투표자/미투표자의 심리학적 성향을 분석
- 심리학 테스트 분석 알고리즘 개발
- 평가 지표: AUC

<br/>

## 2. 주최/주관 & 참가 대상 & 성과

- 주최/주관: DACON
- 후원: 이노베이션 아카데미
- 참가 대상: 일반인, 학생 등 누구나
- 성과: 상위 15%

<br/>

## 3. 대회 기간

- 제출마감: 2020년 11월 16일
- 코드 평가 마감 및 최종순위 발표: 2020년 11월 27일

<br/>

## 4. 내용

&nbsp;&nbsp;&nbsp;&nbsp; 다양한 개인정보 데이터와 몇 가지 질문 답변 데이터를 통해 ‘**작년(2019)에 국가 선거 투표 여부를 예측하는 이진 분류’** 문제이다. 변수를 크게 문자형 변수와 범주형 변수, 연속형 변수 3가지로 나누어 각각의 특성에 따라 **EDA 및 피처 엔지니어링**을 진행했다. 

&nbsp;&nbsp;&nbsp;&nbsp; 피처 생성 이후에는 그 안에서 의미 있는 데이터를 선정하고 가공하고자 다양한 전처리 방법을 거쳤다. 예측력을 방해할 수 있는 **다중공선성**을 제거하고 **주성분분석, 정규화, 표준화, 피처 셀렉션**을 거쳐서 최종적으로 피처를 선정하였다.

&nbsp;&nbsp;&nbsp;&nbsp; 모델링은 LR, RF, XGB, LGBM, ET, GBM, Adaboost 등 여러 가지 모델을 실험해 보았으며 Stacking 및 Meta Model Optimizing 앙상블 과정을 거쳤다. 그 과정에서 각 모델을 Bayesian Optimization을 통해 튜닝한 결과 성능이 가장 잘 나오는 **LGBM 모델 여러 개를 Averaging 앙상블 한 결과를 최종 모델**을 가지고 최종 서브미션을 구하도록 하였다.

<br/>

## 5. Process

### ch.1 Feature Engineering

- EDA
- Continuous Features
- Categorical Features

---

### ch.2 Preprocessing

- Feature Correlation
- PCA
- Normalization
- Standardization
- Feature Selection

---

### ch.3 Modeling

- Logistic Regression
- Random Forest
- XGB
- LGBM
- ExtraTree
- GBM
- Adaboost

---

### ch.4 Ensemble

- Stacking
- Meta Model Optimizing
- Averaging

<br/>

## 6. 참고자료

[월간 데이콘 심리 성향 예측 AI 경진대회 사이트](https://dacon.io/competitions/official/235647/overview/description)
