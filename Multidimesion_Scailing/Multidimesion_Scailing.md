# 다차원척도법

## 1. 다차원 척도법(Multidimensional Scaling)

- 객체간 `근접성(Proximity)`을 시각화하는 통계 기법
- 군집분석과 같이 개체들을 대상으로 변수들을 측정한 후에 개체들 사이의 `유사성/비유사성을 측정`하여 개체들을 2차원 공간상에 점으로 표현하는 분석 방법
- 개체들을 2차원 또는 3차원 공간상에 점으로 표현하여 개체들 사이의 집단화를 시각적으로 표현하는 분석 방법

</br>

## 2. 목적

- 데이터 속에 잠재해 있는 패턴, 구조를 찾아낸다.
- 그 구조를 소수 차원의 공간에 기하학적으로 표현
- 데이터 축소(Data Reduction)의 목적으로 다차원 척도법을 이용
- 즉, 데이터에 포함되는 정보를 끄집어내기 위해서 다차원척도법을 탐색수단으로 사용
- 다차원척도법으로 얻은 결과를, 데이터가 만들어진 현상이나 과정에 고유의 구조로서 의미를 부여
  
    > 데이터 속에 잠재한 패턴을 찾기 위해 복잡한 구조를 소수 차원의 공간에 기하학적으로 표현하는 것
    
</br>

## 3. 다차원척도법 방법

- `유클리드 거리행렬` : 개체들의 거리 계산
    
    $d_{ij}=\sqrt{(x_{il}-x_{il})^2+\cdots+(x_{iR}-x_{iR})^2}$
    
- 관측대상들의 상대적 거리의 정확도를 높이기 위해 적합 정도를 스트레스 값(Stress Value)으로 나타낸다.

- 최적모형의 적합은 부적합도를 최소로 하는 반복알고리즘을 이용하여, 이 값이 일정 수준 이하가 될 때 최종적으로 접합된 모형으로 제시

- 스트레스 값은 S
- Stress와 적합도 수준 M은 개체들을 공간상에 표현하기 위한 방법으로 STRESS나 S-STRESS를 부적합도 기준으로 사용

- 최적모형의 적합은 부적합도를 최소로 하는 방법으로 일정수준(0.05) 이하로 될 때까지 반복해서 수행
    
    ![](../_images/Multidimesion%20Scailing/MS_15.jpeg)
    
</br>

## 4. 다차원척도법 종류

### 가. 계량적 MDS(Metric MDS)

- 데이터가 `구간척도`나 `비율척도`인 경우 활용.

    ![](../_images/Multidimesion%20Scailing/MS_1.jpeg)
    ![](../_images/Multidimesion%20Scailing/MS_2.jpeg)

### 나. 비계량적 MDS(nonmetrix MDS)

- 데이터가 `순서척도`인 경우 활용

    ![](../_images/Multidimesion%20Scailing/MS_3.jpeg)
    ![](../_images/Multidimesion%20Scailing/MS_4.jpeg)
    ![](../_images/Multidimesion%20Scailing/MS_5.jpeg)
    ![](../_images/Multidimesion%20Scailing/MS_6.jpeg)