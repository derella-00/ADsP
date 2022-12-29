# 분류분석

## 1. 분류분석과 예측분석

### 가. 분류분석의 정의

- 데이터가 어떤 그룹에 속하는지 예측하는데 사용
- 클러스터링과 유사하지만 분류분석은 각 그룹이 정의되어 있다.
- 지도학습(supervised learning)에 해당하는 예측기법
- 데이터의 실체가 `어떤 그룹에 속하는지 예측`하는데 사용되는 기법

</br>

### 나. 예측분석의 정의

- 시계열분석처럼 **시간**에 따른 **값** 두 개만을 이용해 앞으로의 매출 또는 온도 등을 예측하는 것
- 모델링을 하는 입력 데이터가 어떤 것인지에 따라 특성이 다르다.
- 한 개의 설명변수

</br>

### 다. 분류분석, 예측분석의 공통점과 차이점

1. 공통점
    
- 레코드의 특성 속성의 값을 미리 알아맞히는 점
    
2. 차이점
    
- `분류`: 레코드(튜플)의 **범주형 속성**의 값을 맞힘(레코드의 특정 속성의 값이 범주형으로 정해져 있다)
  
  ex) 국영수 점수를 통해 내신등급을 알아맞히는 것, 회원의 가입 정보를 통해 1년 후 신용등급을 맞히는 것
    
- `예측`: 레코드(튜플)의 **연속형 속성**의 값을 맞힘
  
  ex) 학생의 여러 가지 정보를 통해 수능점수를 맞히는 것, 회원의 가입 정보를 통해 연 매출액을 예측하는 것
    
</br>

### 라. 분류 모델링

- 신용평가모형(우량, 불량)
- 사기방지모형(사기, 정상)
- 이탈모형(이탈, 유지)
- 고객세분화(등급)

### 마. 분류 기법

- 회귀분석, **로지스틱 회귀분석(Logistic Regression)**
- **의사결정나무(Decision Tree)**, CART(Classification and Regression Tree), C5.0
- `나이브 베이지안` 분류
- **인공신경망(ANN, Artificial Neural Network)**
- 지지도 벡터기계
- k 최근접 이웃
- 규칙기반의 분류와 사례기반추론