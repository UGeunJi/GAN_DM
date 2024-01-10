# Synthesis with GAN

## Similar with mustGAN but Enhanced owing to weights

#### Common problem: high time consuming, expensive cost

```
** Multi-stream

one-to-one: Source's unique information
many-to-one: Source's shared information

Aggregate these informations

**feature concatenation**
```

---

<br>

## Specific Loss

```
* Loss

pixel-wise loss, gradient difference loss(GDL)

* Effect

Better than mustGAN
```

---

<br>

## Specific Advantages

1. 단순히 concat해서 여러 modalities의 valuable한 정보의 차이를 고려하지 않음
  ➔ 같은 scale에서의 feature를 결합해 가용 modalities에서의 더 관련있는 정보를 보조하며 각 down-sampling module에 적용
2. 각 scale에 다른 encoder로부터 modality 특징의 결합을 하는 gate mergence(GM)을 사용. **(weight를 자동으로 조정하여 입력으로 적용)
3. BRATS2015 dataset으로부터 SOTA의 성적을 냄.
