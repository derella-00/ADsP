# 통계분석의 이해

## 1. 통계

- 통계: 특정집단을 대상으로 수행한 조사나 실험을 통해 나온 결과에 대한 요약된 형태의 표현
</br></br>

## 2. 통계자료의 획득 방법

총 조사(census)와 표본조사(sampling)

### 표본 추출 방법

1. 단순랜덤추출(simple random sampling):

    각 샘플에 번호를 부여하여 임의의 n개를 추출하는 방법, 각 샘플은 선택될 확률이 동일(비복원, 복원 추출)
    </br></br>
2. 계통추출법(systematic sampling)

    단순랜덤추출법의 변형된 방식, 번호를 부여한 샘플을 나열하여 K개씩(N/n) n개의 구간으로 나누고 첫 구간(1, 2, ・・・, K)에서 하나를 임의로 선택한 후에 K개씩 띄어서 n개의 표본을 

    ![](../_images/Statistics/통계분석_01.jpeg)
</br></br>

1. 집락추출법(cluster sampling)

    군집을 구분하고 군집별로 단순랜덤 추출법을 수행한 후, 모든 자료를 활용하거나 샘플링하는 방법(지역표본추출, 다단계표본추출)

    ![](../_images/Statistics/통계분석_02.jpeg)
</br></br>

1. 층화추출법(stratified random sampling)

    이질적인 원소들로 구성된 모집단에서 각 계층을 고루 대표할 수 있도록 표본을 추출하는 방법으로, 유사한 원소끼리 몇 개의 층(stratum)으로 나누어 각 층에서 랜덤 추출하는 방법(비례층화추출법, 불비례층화추출법)

    ![](../_images/Statistics/통계분석_03.jpeg)
</br></br>

### 자료의 측정 방법


- 명목척도`(질적 척도)`
  
  측정 대상이 어느 집단에 속하는지 분류할 때 사용(성별, 출생지 구분)단순한 번호로 차례의 의미 ❌ 
- 순서척도`(질적 척도)`
  
  측정 대상의 서열관계를 관측하는 척도(만족도, 선호도, 학년, 신용등급) 순서가 의미를 가짐

- 구간척도(등간척도)`(양적 척도)`
  
    측정 대상이 갖고 있는 속성의 양을 측정하는 것으로 구간이나 구간 사이의 간격이 의미가 있는 자료. 순서와 그 간격에도 의미가 있다.

- 비율척도`(양적 척도)`
  
  간격(차이)에 대한 비율이 의미를 가지는 자료, 절대적 기준인 0이 존재하고 사칙연산이 가능하며 제일 많은 정보를 가지는 척도(무게, 나이, 시간, 거리)

</br></br>

### 표본조사

- 표본오차: 모집단을 대표할 수 있는 포본 단위들이 조사대상으로 추출되지 못함으로서 발생하는 오차를 말한다.

- 표본편의: 모수를 작게 또는 크게 할 때 추정하는 것과 같이 표본추출방법에서 기인하는 오차를 의미한다. 표본추출 과정에서 특정 대상이 다른 대상에 비해 우선적으로 추출될 때 생기는 오차. ‘확률화’에 의해 최소화하거나 없앨 수 있다.
    - 확률화: 모집단으로부터 편의되지 않은 표본을 추출하는 절차, 확률화 절차에 의해 추출된 표본을 확률표본이라 한다.

- 비표본오차: 표본오차를 제외한 모든 오차로서 조사 과정에서 발생하는 모든 부주의나 실수, 알 수 없는 원인 등 모든 오차를 의미하며 조사대상이 증가하면 오차가 커진다.

- 응답오차, 유도질문 등은 표본조사에서 유의할 점이다.
</br></br>

## 3. 통계분석

### 기술통계(descriptive statistic)

- 주어진 자료로부터 어떠한 판단이나 예측과 같은 주관이 섞일 수 있는 과정을 배제하여 통계집단들의 여러 특성을 수량화하여 객관적인 데이터로 나타내는 통계분석 방법론이다.

- 평균, 표준편차, 중위수, 최빈값, 그래프

### 통계적 추론(statistical inference)

- 수집된 자료를 이용해 대상 집단(모집단)에 대한 의사결정을 하는 것으로 sample을 통해 모집단을 추정하는 것을 의미한다.
  
    - 모수추정: 표본집단으로부터 **모집단의 특성인 모수(평균, 분산 등)를 분석**하여 모집단을 추론한다.
  
    - 가설검정: 대상집단에 대해 특정한 가설을 설정한 후에 그 가설이 **옳은지 그른지에 대한 채택여부를 결정**하는 방법론이다.
  
    - 예측: 미래의 **불확실성을 해결해 효율적인 의사결정**을 하기 위해 활용한다.(회귀분석, 시계열분석 등)

</br></br>

## 4. 확률 및 확률 분포

### 확률

표본공간 S에 부분집합인 각 사상에 대해 실수값을 가지는 함수의 확률값이 0과 1사이에 있고, 전체 확률의 합이 1인 것을 의미한다. 표본공간 Ω의 부분집합인 사건 E의 확률은 표본공간의 원소의 개수에 대한 사건 E의 개수의 비율로 확률을 P(E)라고 할 때, 다음과 같이 정의한다.

$P(E) = n(E)/n(Ω)$
</br></br>

### 확률변수(random variable)

- 특정값이 나타날 가능성이 확률적으로 주어지는 변수이다.
- **정의역(domain)이 표본공간(Ω), 치역(range)이 실수값(0<y<1)인 함수**
- 0이 아닌 확률을 갖는 실수값의 형태에 따라 이산형 확률변수와 연속형 확률변수로 구분된다.

> 확률변수의 기대값
확률변수 X의 기대값(expectation, excepted value)
> 
> - 이산(범주)형 변수인 경우 : $E(X) =\sum x_if(x_i)$ → 합
> - 연속형 변수인 경우: $E(X) =\int xf(x)dx$ → 미분

- 이산형(범주)형 변수
    - 고정된 수의 고유값만 가질 수 있고 고유한 순서가 없는 통계 변수 유형
    - 값은 계산에 의해 얻어진다.
    - 별개 또는 별개의 값

- 연속형 변수
    - 가능한 모든 값을 가정하는 임의의 변수
    - 주어진 범우 내에서 어떤 값도 취할 수 있다.
    - 값은 측정을 통해 얻어지며 계산 불가능한 값 집합을 취할 수 있다.

- 덧셈정리(`배반이 아닐 때`):
  
    사건 $A$와 사건 $B$가 동시에 일어날 수 있을 때(교집합이 성립할 때), 일어날 확률 $P(A 또는 B)$는 $P(A\cup B)=P(A)+P(B)-P(A\cap B)$로 표현된다. 사건 B가 주어졌을 때 사건 A의 조건부 확률은 $P(A\mid B)=\frac {P(A\cap B)}{P(B)}$로 표현된다.


- 덧셈정리(`배반사건일 때`):
  
    사건 $A$와 사건 $B$가 동시에 일어나지 않을 때, 즉 사건 $A$ 또는 사건 $B$ 중 어느 한 쪽만 일어날 확률은 $P(A∪B) = P(A) + P(B)$로 표현된다.

- 곱셈정리: 사건 $A$와 $B$가 서로 무관하게 나타날 때, 즉 독립사건일 때 $A$와 $B$가 동시에 나타날 확률 $P(A와 B)$는 $P(A∩B)=P(A)×P(B)$로 표현되고, 사건 B가 주어졌을 때 사건 $A$의 조건부 확률은 $P(A|B)=P(A)$로 표현된다.

</br></br>

### 확률분포

#### 이산형 확률분포(discrete distribution)

0이 아닌 확률값을 갖는 확률 변수를 셀 수 있는 경우(확률질량함수)

$$E(X) =\sum x_if(x_i)$$

**(1) 베르누이분포**

- 결과가 2개만 나오는 경우(예시: 동전 던지기, 시험의 합격/불합격 등)

$$
P=(X=x)=p^z\cdot p(1-p)^{1-x}\\ (x=1\ or\ 0),\ E(x)=p,\ var(x)=p(1-p)
$$


**(2) 이항분포**

- 베르누이 시행을 n번 반복했을 때 k번 성공할 확률

$$
P(X=k)=_{n}\mathrm{C}_{k}P^k(1-p)^{n-k},\ _{n}\mathrm{C}_{k}=\frac{n!}{k!(n-k)!}\\x\sim~B(n,p),\ E(x)=np, \ var(x)=np(1-p)
$$

- 성공할 확률 p가 0이나 1에 가깝지 않고 n이 충분히 크면 이항분포는 정규분포에 가까워진다. 성공할 확률 p가 1/2에 가까우면 종모양이 된다.
    
    ![](../_images/Statistics/통계분석_04.jpeg)
    1의 주사위를 10회, 20회, 30회, 50회 던졌을 때 그 눈이 x회 나올 확률을 그래프로 나타낸 것
    

**(3) 기하분포**

- 성공확률이 p인 베르누이 시행에서 첫번째 성공이 있기까지 x번 실패할 확률
    
- 타자가 오늘 경기에서 5번 타석에 들어와서 3번째 타석에서 안타칠 확률은 기하분포를 따른다.
    

**(4) 다항분포**

- 이항분포를 확장한 것으로 세가지 이상의 결과를 가지는 반복 시행에서 발생하는 확률 분포

    ![](../_images/Statistics/통계분석_05.jpeg)
    

**(5) 포아송 분포**

- 시간과 공간 내에서 발생하는 사건의 발생횟수에 대한 확률분포
(예: 책에 오타가 5page 당 10개씩 나온다고 할 때, 한 페이지에 오타가 3개 이상 나올 학률)
- $\lambda$  = 정해진 시간 안에 어떤 사건이 일어날 횟수에 대한 기댓값, y = 사건이 일어난 수

    ![](../_images/Statistics/통계분석_06.jpeg)

</br></br>

#### 연속형 확률분포(continuous distribution)

가능한 값이 실수의 어느 특정구간 전체에 해당하는 확률변수(확률밀도함수)

$$
f(x)\ge0\quad \int_{-\infty}^\infty f(x)dx=1
$$

![](../_images/Statistics/통계분석_07.jpeg)

</br></br>

**(1) 균일분포(일양분포, Uniform distribution)**

- 모든 확률변수 X가 균일한 확률을 가지는 확률분포(다트의 확률분포)

    ![](../_images/Statistics/통계분석_08.jpeg)


**(2) 정규분포(Normal distribution)**

- 평균이 $\mu$이고, 표준편차가 $\sigma$인 $x$의 확률밀도 함수
- 표준편차가 클 경우 퍼져보이는 그래프가 나타난다.

    ![](../_images/Statistics/통계분석_09.jpeg)![](../_images/Statistics/통계분석_10.jpeg)

**(3) 지수분포(Exponential distribution)**

- 어떤 사건이 발생할 때까지 경과 시간에 대한 연속확률분포이다.
ex) 전자레인지의 수명시간, 콜센터에 전화가 걸려올 때까지의 시간, 은행에 고객이 내방하는데 걸리는 시간, 정류소에서 버스가 올 때까지의 시간

    ![](../_images/Statistics/통계분석_11.jpeg)

(4) **t-분포**

- 표준정규분포와 같이 평균이 0을 중심으로 좌우가 동일한 분포를 따른다.
- 표본의 크기가 적을 때는 표준정규분포를 위에서 눌러 높은 것과 같은 형태를 보이지만 표본이 커져서(30개 이상) 자유도가 증가하면 표준정규분포와 거의 같은 분포가 된다.
- 데이터가 연속형일 경우 활용한다.
- **두 집단의 평균이 동일한지 알고자 할 때 검정통계량으로 활용된다.**

    ![](../_images/Statistics/통계분석_12.jpeg)


(5) **$x^2$-분포**(카이제곱 분포, chi-square distribution)

- 모평균과 모분산이 알려지지 않은 모집단의 모분산에 대한 가설 검정에 사용되는 분포이다.
- 정규모집단으로부터 n개를 단순임의 추출한 표본의 분산은 자유도가 n-1인 카이제곱분산을 따른다.
- 두 집단 간의 동질성 검정에 활용된다.(범주형 자료에 대해 얻어진 관측값과 기대값의 차이를 보는 적합성 검정에 활용)

    ![](../_images/Statistics/통계분석_13.jpeg)

(6) **F분포**(F-distribution)

- **두 집단간 분산의 동일성 검정**에 사용되는 검정 통계량의 분포이다.
- 이 표본에 의한 분산비 검정은 두 표본의 분산이 동일한지를 비교하는 검정으로 검정통계량은 F분포를 따른다.
- 확률변수는 항상 양의 값만을 갖고 $x^2$-분포와 달리 자유도를 2개 가지고 있으며 자유도가 커질수록 정규분포에 가까워진다.

    ![](../_images/Statistics/통계분석_14.jpeg)

</br></br>

## 5. 추정 및 가설검정

### 가. 추정의 개요

**1) 확률표본**

- 특정한 확률분포로부터 독립적으로 반복해 표본을 추출하는 것)
- 각 관찰값들은 서로 독립적이며 동일한 분포를 갖는다.

**2) 추정: 표본으로부터 미지의 모수를 측정하는 것**

#### 점추정(point estimation)

- ‘**모수가 특정한 값일 것**’이라고 추정하는 것.
- 평균, 표준편차, 중앙값 등을 추정
- 점추정 조건
    
    - **불편성(unbiasedness)**: 모든 가능한 표본에서 얻은 추정량의 기댓값은 모집단의 모수와 편의(차이)가 없다.
    - **효율성(efficiency)**: 추정량의 분산이 적을수록 좋다
    - **일치성(consistency)**: 표본의 크기가 아주 커지면, 추정량이 모수와 거의 같아진다.
    - **충족성(sufficient)**: 추정량은 모수에 대하여 모든 정보를 제공한다.
    
    - **표본평균(Sample mean)**: 모집단의 평균(모평균)을 추정하기 위한 추정량. 확률표본의 평균값
    
    - **표본분산(Sample variance)**: 모집단의 분산(모분산)을 추정하기 위한 추정량(표본의 분산은 카이제곱 분포를 따른다)
    
    </aside>
    

**구간추정(interval estimation**

- 점추정을 보완하기 위해 모수가 특정 구간에 있을 것이라고 추정하는 것.(모수의 참값이 포함되어 있다고 추정되는 구간을 결정하는 것)
- 항상 추정량의 분포에 대한 전제가 주어져야 하고, 구해진 구간 안에 모수가 있을 가능성의 크기(신뢰수준)가 주어져야 한다.
- 모분산을 알거나 대표본의 경우 표준정규분포 활용, 모분산을 모르거나 소표본의 경우 t분포 활용.

### 가설검정

- 모집단에 대한 가설을 설정한 뒤, 그 가설의 채택여부를 결정하는 방법
- 표본 관찰 또는 실험을 통해 귀무가설과 대립가설 중에서 하나를 선택하는 과정이다.
- 귀무가설이 옳다는 전제하에 검정통계량 값을 구한 후에 이 값이 나타날 가능성의 크기에 의해 귀무가설의 채택여부를 결정한다.

- **귀무가설**(null hypothesis, 𝘏₀) : **'비교하는 값과 차이가 없다, 동일하다’**를 기본 개념으로 하는 가설
- **대립가설**(alternative hypothesis, 𝘏₁) : **뚜렷한 증거가 있을 때 주장하는 가설**
- 검정통계량: 관찰된 표본으로부터 구하는 통계량, 검정 시 가설의 진위를 판단하는 기준
- 유의수준 : 귀무가설을 기각하게 되는 확률의 크기로 ‘귀무가설이 옳은데도 이를 기각하는 확률의 크기’

- 1종 오류(Type l Error): 귀무가설 𝘏₀가 옳은데도 귀무가설을 기각하게 되는 오류
이때 내린 판정이 잘못되었을 때 실제 확률 $p-value$
- 2종 오류(Type ll Error): 귀무가설 𝘏₀가 옳지 않은데도 귀무가설을 채택하게 되는 오류
    
    
    |  | 𝘏₀가 사실이라고 판정 | 𝘏₀가 사실이 아니라고 판정 |
    | --- | --- | --- |
    | 𝘏₀가 사실임 | 옳은 결정 | 제 1종 오류(𝜶) |
    | 𝘏₀가 사실이 아님 | 제 2종 오류(𝜷) | 옳은 결정 |
- 1종 오류의 크기를 0.1, 0.05, 0.01로 고정시키고 2종 오류가 최소가 되도록 기각역을 설정

</br></br>

## 5. 비모수 검정

통계적 검정에서 모집단의 모수에 대한 검정은 모수적 검정과 비모수적 검정으로 구분한다.

#### 모수적 방법

검정하고자 하는 **모집단의 분포에 대한 가정**을 하고, 그 가정하에서 검정통계량과 검정통계량의 분포를 유도해 검정을 실시하는 방법이다.

#### 비모수적 방법

자료가 **추출된 모집단의 분포에 대한 아무 제약을 가하지 않고 검정을 실시**하는 방법이다.

#### 모수적검정과 비모수검정의 차이점

- 가설 설정 방법: ‘분포의 형태가 동일하다’, ‘분포의 형태가 동일하지 않다’ 라는 식으로 **분포의 형태에 대해 설정**
- 검정 방법: 순위나 두 관측값 차이의 부호를 이용해 검정
- 예 :
    - 부호검정(sign test)
    - 윌콕슨의 순위합검정(rank sum test)
    - 윌콕슨의 부호순위합검정(Wilcoxon signed rank test)
    - 만-위트니의 U 검정
    - 런검정(run test)
    - 스피어만의 순위상관계수
