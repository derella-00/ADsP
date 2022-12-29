# 데이터 마이닝 성과분석

## 가. 오분류에 대한 추정치

![](../_images/Data%20Minning/DM_1.jpeg)

1. 정분류율(혹은 `정확도`, `Accuracy`): 전체 중 맞은(True) 예측 비율

    $Accuracy=\frac{TP+TN}{TP+TN+FP+FN}$

2. `오분류율`(Error Rate): 전체 중 틀린(False) 예측 비율
    $1-Accuracy=\frac{FN+FP}{TN+TP+FN+FP}$

3. `특이도(Specificity)`: 실제 음성 판정 중 맞은(True) 음성 예측 비율

    $Specificity=\frac{TN}{TN+FP}$  (TNR: True Negative Rate)

4. `민감도(Sensitivity)` = `재현율(Recall)`: 실제 양성 판정 중 맞은(True) 양성 예측 비율

    $Sensitivity=\frac{TP}{TP+FN}$(TPR: True Positive Rate)

5. `정확도(Precision)`: 양성 예측 중 실제 양성 판정 비율
    $Precision=\frac{TP}{TP+FP}$

6. F1 Score
   
   $F_1=2\times\frac{Precision\times Recall}{Precision+Recall}$

    ![](../_images/Data%20Minning/DM_2.jpeg)

</br></br>

## 나. ROCR 패키지로 성과분석

### 1) ROC Curve(Receiver Operating Characteristic Curve)

- `ROC Curve`란 가로축을 **FPR**(False Positive Rate = **1 - 특이도**)값으로 두고, 세로축을 **TPR**(True Positive Rate, **민감도**) 값으로 두어 시각화한 그래프
  
- 2진 분류에서 모형의 성능을 평가하기 위해 많이 사용되는 척도

- 그래프가 **왼쪽 상단에 가깝게 그려질수록** 올바르게 예측한 비율은 높고, 잘못 예측한 비율은 낮음을 의미한다. 
  
- 따라서 **ROC곡선 아래의 면접을 의미하는 AUROC(Area Under ROC)** 값이 크면 클수록(1에 가까울수록) 모형의 성능이 좋다고 평가
    
    ![](../_images/Data%20Minning/DM_3.jpeg)

</br>

## 다. 이익도표(Lift Chart)

### 1) 이익도표의 개념

- 이익도표는 분류모형의 성능을 평가하기 위한 척도
- 분류된 관측치에 대해 얼마나 예측이 잘 이루어졌는지를 나타내기 위해 임의로 나눈 각 등급별 도표
- 반응검출율, 반응률, 리프드 등의 정보를 산출
- 이익도표의 각 등급은 예측확률에 따라 매겨진 순위, 상위 등급에서는 더 높은 반응률을 보이는 것이 좋은 모형이라고 평가할 수 있다.

### 2) 이익도표의 활용 예시

![](../_images/Data%20Minning/DM_9.jpeg)

- 전체 2000명 중 **381명** 구매 → **기본 향상도** = 381 / 2000 = 19.05%
- Frequency of “buy”: 2000명 중 실제로 구매한 사람
- % Captured Response: 반응검출율 = 해당 등급의 실제 구매자 / 전체 구매자
- % response: 반응률 = 해당 등급의 실제 구매자 / 200명
- Lift: 향상도 = 반응률 / 기본 향상도
    
    **→ 좋은 모델이라면 Lift가 빠른 속도로 감소해야 한다.**
    
    ![](../_images/Data%20Minning/DM_10.jpeg)

- 등급별로 향상도가 급격하게 변동할수록 좋은 모형이라고 할 수 있고, 들쭉날쭉하면 좋은 모형이라고 볼 수 없다.