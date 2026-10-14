---
created: 2026-09-18
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/numeri_complessi
aliases: []
---
[[00_A1_Numeri_Complessi|⬅️ Torna a Numeri Complessi]]

# Coniugato e Modulo

Dato $z=x+iy\in\mathbb{C}$:

- **Complesso coniugato**: $\bar z=x-iy$.
- **Modulo**: $|z|=\sqrt{x^2+y^2}$.

![[coniugato-e-modulo.png]]

Proprietà:

- $|z|=0\iff z=0$; $\ |z|\ge0\ \ \forall z$.
- $\bar z$ è il **simmetrico** di $z$ rispetto all'asse reale.
- $|z|$ è la **distanza** di $z$ da $O$ nel piano complesso (teorema di Pitagora). Più in generale $|z-w|$ è la distanza tra $z$ e $w$:
$$|z-w|=\sqrt{(x-a)^2+(y-b)^2}\qquad (z=x+iy,\ w=a+ib).$$
- $z=\bar z\iff z\in\mathbb{R}\ (\operatorname{Im}z=0)$.

### Luoghi notevoli
- $\operatorname{Im}z=\text{costante}$: **retta orizzontale**.
- $\operatorname{Re}z=\text{costante}$: **retta verticale**.
- $|z|=\rho\ge0$: **circonferenza** centrata in $O$ di raggio $\rho$.

![[luoghi-notevoli-piano-complesso.png]]

### Identità utili
- $z\bar z=(x+iy)(x-iy)=x^2+y^2=|z|^2$
- $|z|=|\bar z|$
- $z^{-1}=\dfrac1z\cdot\dfrac{\bar z}{\bar z}=\dfrac{\bar z}{|z|^2}=\dfrac{x-iy}{x^2+y^2}$ per $z\neq0$
- $\overline{w\cdot z}=\bar w\cdot\bar z$ e $\overline{w+z}=\bar w+\bar z$
- $\dfrac zw=\dfrac zw\cdot\dfrac{\bar w}{\bar w}=\dfrac{z\bar w}{|w|^2}$ per $w\neq0$

**Esempio.** $z=3-2i,\ w=1+7i$:
$$\frac zw=\frac{z\bar w}{|w|^2}=\frac{(3-2i)(1-7i)}{1+49}=\dots=-\frac{11}{50}-\frac{23}{50}i.$$

---
Precedente: [[Piano di Argand-Gauss]] · Successivo: [[Equazioni in C]]
