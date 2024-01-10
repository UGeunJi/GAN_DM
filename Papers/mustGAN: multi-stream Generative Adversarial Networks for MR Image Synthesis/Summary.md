# Synthesis with GAN

```
** Multi-stream

one-to-one: Source's unique information
many-to-one: Source's shared information

Aggregate these informations

**feature concatenation**
```

## Many to One based on pix2pix

T1, T2, FLAIR(Fluid Attenuate Inverse Recover), PD-weighted ➔ One

healthy and glioma patients

---

<br>


## Specific Loss

```
* Loss

pixel-wise loss, cycle consistency loss


* Effect

reduce noise
improved sharpness
```

---

<br>

## Mechanism

concat features

Fusion block ➔ Joint network ➔ Adatively modify Fusion block's location ➔ Joint network ➔ ...

Same with registration
