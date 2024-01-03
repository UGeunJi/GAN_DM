## Abstract


다루기 힘든 사후 분포에서의 연속적인 latent variable의 존재와 직접적인 확률 모델에서의 **학습과 추론을 어떻게 효율적으로 할 것인가?**

다루기 힘든 케이스에서도 약간 일반적으로 미분적으로 다루기 힘든 환경이나 큰 규모로 확장되는 데이터셋에서도 작동하는 **확률적 학습, 추론 모델을 소개**

First, 일반적인 확률적 강하 방법으로 variational lower bound의 재조정을 통해 최적화 할 수 있는 **lower bound estimator를 산출**

Second, **lower bound estimator로 근사 추론 모델을 맞춰줌으로써** 사후 추론에 특히 효율적으로 datapoint마다의 연속적인 latent variable의 데이터셋을 소개


```
## Mechanism ##
Stochastic gradient method ➔ lower bound estimator ➔ variational lower bound ➔ continuous latent variable
```

---

## Introduction

For the case of an i.i.d. dataset and continuous latent variables per datapoint,

다루기 힘든 사후 분포에서 continuous latent variables과 parameters를 어떻게 효율적으로 학습, 추론할 수 있겠는가?

Variational Bayesian (VB) 접근 방식이 다루기 힘든 사후 추론에서 근사치의 최적화를 한다.

일반적인 경우에서도 근사 사후 추론의 분석적 해결책을 요구한다.

우리가 lower bound에 대해 편향되지 않은 간단한 미분적인 추정을 산출해내는 variational lower bound의 재조정을 보여준다.   ➔   SGVB (Stochastic Gradient Variational Bayes)

Stochastic Gradient Variational Bayes (SGVB)는 continuous latent variables와 parameters의 모델에서 근사 사후 추론을 효율적으로 할 수 있게 해준다.

그리고 확률적 경사 상승법 기술로 최적화한다.

datapoint마다에서의 continuouss latent variables의 i.i.d. 데이터셋에서는 Auto-Encoding VB (AEVB) 알고리즘을 제안했다.

이 알고리즘은 datapoint마다의 큰 비용의 추론 방식을 사용하지 않으며 parameters를 학습하고 간단한 사전 샘플링을 통해 효율적인 근사 사후 추론을 하는 SGVB를 사용해 효율적인 학습과 추론을 한다. //// SGVB와 AEVB의 차이가 명확해야 할 것

이것이 variational auto-encoder가 되는 것이다.
