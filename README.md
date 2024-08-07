# 회전기계 고장유형 AI 데이터셋 분석

<code><img  height = '400'
src = https://github.com/siilver94/AI-Analysis-of-Rotating-Machinery-Failure-Types/assets/57824945/182646ad-452f-41c2-8989-438ba2af0781></code>


## 소개
이 프로젝트는 **KAMP(한국산업지능화협회)** 에서 제공하는 '회전기계 고장유형 AI 데이터셋'을 활용하여 진행되었습니다. 이 데이터셋은 다양한 회전기계의 고장 데이터를 포함하고 있으며, 이를 통해 고장 유형을 분석하고 예측하는 모델을 개발하는 것이 목표입니다.

제조업에서는 회전기계의 고장은 생산성에 큰 영향을 미치며, 사전에 고장을 예측하고 예방하는 것이 매우 중요합니다. 해당 프로젝트는 이러한 배경에서 출발하여, 딥러닝 기법을 활용해 회전기계 고장을 예측하는 데 중점을 두고 있습니다.

<br/>

## 데이터셋 정보
- **데이터셋 이름**: 회전기계 고장유형 AI 데이터셋
- **출처**: [KAMP - 제조 데이터 분석](https://www.kamp-ai.kr/aidataDetail?AI_SEARCH=%ED%9A%8C%EC%A0%84&page=1&DATASET_SEQ=18&EQUIP_SEL=&GUBUN_SEL=&FILE_TYPE_SEL=&WDATE_SEL=)
- **데이터셋 설명**: 이 데이터셋은 다양한 회전기계의 고장 데이터를 포함하고 있으며, 각 기계의 다양한 센서 데이터와 고장 유형이 포함되어 있습니다. 데이터셋은 회전기계 고장 환경을 만들어 데이터를 구성하였고, 이는 현실적인 분석 및 예측이 가능합니다.

<br/>

## 분석 과정
### 1. 데이터 전처리
- **선형보간**: 센서로부터 계측된 데이터의 시간간격의 동일화를 위해 선형보간을 합니다.
- **데이터 정규화**: 데이터의 스케일링을 통해 모델 학습을 용이하게 합니다.
- **데이터 필터링**: 노이즈가 포함되어있는 데이터들을 AI 분석 모델 훈련을 위해 이동평균필터를 사용하여 필터링 합니다.

<br/>

### 2. 탐색적 데이터 분석 (EDA)
- **데이터 시각화**: 데이터 분포와 패턴을 이해하기 위해 다양한 시각화 기법을 사용합니다.
- **상관 분석**: 특성 간의 상관 관계를 분석하여 모델링에 유용한 인사이트를 도출합니다.

<br/>

### 3. 모델링
- **모델 선택**: 여러 머신러닝 알고리즘(CNN, RNN, DNN)을 비교하고 최적의 모델을 선택합니다.
- **모델 학습**: 학습 데이터를 사용하여 모델을 학습시킵니다.
- **모델 평가**: 테스트 데이터를 사용하여 모델의 성능을 평가하고, 평가 지표 **Accuracy** 를 사용하여 분석합니다.

<br/>

### 4. 결과 및 결론
- **결과 시각화**: 모델의 예측 결과를 시각화하여 쉽게 이해할 수 있도록 합니다.
- **인사이트 도출**: 분석 결과로부터 중요한 인사이트를 도출하고, 이를 통해 회전기계의 고장을 예측하고 예방할 수 있는 방안을 제시합니다.

<br/>

## 사용된 도구 및 라이브러리
- **프로그래밍 언어**: Python
- **라이브러리**: pandas, numpy, scikit-learn, matplotlib, seaborn

<br/>

## 출처
중소벤처기업부, Korea AI Manufacturing Platform(KAMP), 회전기계 고장유형 AI 데이터셋,

KAIST(기계공학과 이필승교수), 2021.12.27., www.kamp-ai.kr

<br/>

### 5. 회고 및 리뷰

이 프로젝트를 통해 여러 가지를 배울 수 있었습니다. 주니어 데이터 분석가로서 다음과 같은 점들을 느꼈습니다

#### 느낀 점과 배운 점
- 데이터 전처리의 중요성: 센서 데이터의 불규칙한 시간 간격을 맞추기 위해 선형 보간법을 사용하고, 이동평균필터로 노이즈를 제거하여 데이터 품질을 높이는 방법을 배웠습니다. 이를 통해 데이터의 일관성을 유지하는 것이 얼마나 중요한지 깨달았습니다.
  
- 탐색적 데이터 분석 (EDA): 데이터 시각화와 상관 분석을 통해 숨겨진 패턴을 발견하고, 모델링에 유용한 인사이트를 도출할 수 있었습니다. 다양한 시각화 기법을 사용하여 데이터의 분포와 패턴을 파악하는 것이 모델링 과정에서 매우 유용했습니다.


#### 어려움과 해결 방법

- 데이터 전처리: 불규칙한 시간 간격과 노이즈가 많은 데이터를 다루는 것이 어려웠지만, 선형 보간법과 이동평균필터를 사용하여 문제를 해결했습니다.
  
- 결과 해석: 모델의 예측 결과를 해석하고 유의미한 인사이트를 도출하는 것이 어려웠지만, 평가 지표를 다각도로 분석하고 결과를 시각화하여 쉽게 이해할 수 있도록 하였습니다.

  
이 프로젝트를 통해 데이터 전처리, 탐색적 데이터 분석, 모델링 및 평가의 중요성을 체감할 수 있었으며, 주니어 데이터 분석가로서 제조 데이터를 통해 많은 기술과 인사이트를 얻을 수 있었습니다.
