# 딥러닝 입력 데이터 정규화(Normalizing Inputs)

학습을 수행하기 전에 값의 범위를 nomalization 하는 것은 중요

- 이유
- 입력을 `Standardization`하면 **학습을 더 빨리**하고 **지역 최적의 상태에 빠지게 될 가능성을 줄이**는 다양한 실용적인 이유
- 표준화 된 입력을 통해 `Gradient Descent` 및 `Bayesian estimation`을 보다 편리하게 수행



## Normalization(정규화)

수식 : (요소값 - 최소값) / (최대값 - 최소값)

> 설명 : **전체 구간을 `0~1`사이의 값으로 맞춰 준다.**

머신러닝 또는 딥러닝에서 정규화의 목표는 값 범위의 차이를 왜곡시키지 않고 데이터 세트를 공통 스케일로 변경하는 것.

**feature scaling**: 데이터 처리에 있어 각 특성의 스케일을 조정한다는 의미

흔히 스케일 조정 중 **Min-Max Scaler** 의 의미로 사용
$$
\frac{x−xmin}{xmax−xmin}
$$


## Regularization(정규화/일반화)

Generalization(일반화)과 의미가 혼동

규제라고도 번역하지만 페널티로 모델을 제어하는 방식에는 유효하지만 또 다른 방식에는 어색한 표현

**보통 모델의 설명도를 유지하면서 모델의 복잡도를 줄이는 방식**

- Early stopping
- Noisy input
- drop-out
- Pruning & feature selection
- emsemble 등



## Standardization(표준화)

수식 : (요소값 - 평균) / 표준편차

> 설명 : 기존 데이터를 평균 0, 표준 편차 1인 표준분포의 꼴 데이터로 만드는 것을 의미

**Standard Scaler** 또는 **z-score normalization** 을 의미

평균을 기준으로 얼마나 떨어져 있는지를 살펴볼 때 보통 사용

보통 데이터 분포가 가우시안 분포를 따를 때 유용
$$
\frac{x-x¯}{σ}
$$
표준화와 정규화는 경우에 따라 다르게 정의 -> 그렇기에 때에 따라 의미를 살펴보는 것이 좋음
<br/><br/><br/>

###### 참고 자료

<https://goodtogreate.tistory.com/entry/Neural-Network-%EC%A0%81%EC%9A%A9-%EC%A0%84%EC%97%90-Input-data%EB%A5%BC-Normalize-%ED%95%B4%EC%95%BC-%ED%95%98%EB%8A%94-%EC%9D%B4%EC%9C%A0>

<https://subinium.github.io/introduction-to-normalization/>
