---
created: 2026-09-23
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/numeri_complessi
aliases: []
---
[[00_A1_Numeri_Complessi|⬅️ Torna a Numeri Complessi]]

# Formule di de Moivre

> **Teorema (prodotto e quoziente).** Siano $z=re^{i\theta}=r(\cos\theta+i\sin\theta)$ e $w=Re^{i\varphi}=R(\cos\varphi+i\sin\varphi)$. Allora
> $$w\cdot z=rR\,[\cos(\theta+\varphi)+i\sin(\theta+\varphi)]=rR\,e^{i(\theta+\varphi)},$$
> e se $w\neq0$
> $$\frac zw=\frac rR\,[\cos(\theta-\varphi)+i\sin(\theta-\varphi)]=\frac rR\,e^{i(\theta-\varphi)}.$$

**Dimostrazione (prodotto).**
$$z w=rR\big[(\cos\theta\cos\varphi-\sin\theta\sin\varphi)+i(\sin\theta\cos\varphi+\cos\theta\sin\varphi)\big]=rR[\cos(\theta+\varphi)+i\sin(\theta+\varphi)]$$
per le **identità trigonometriche** di addizione. Per il quoziente la dimostrazione è analoga, partendo da $\dfrac zw=\dfrac{z\bar w}{|w|^2}$. $\square$

### Conseguenze
- $|zw|=|z||w|$
- $\arg(zw)=\arg z+\arg w$
- $\left|\dfrac zw\right|=\dfrac{|z|}{|w|}\ (w\neq0)$
- $\arg\!\left(\dfrac zw\right)=\arg z-\arg w$
- Con $z=1=1\cdot e^{i0}$: se $w=Re^{i\varphi}\neq0$,
$$w^{-1}=\frac1w=\frac1R(\cos\varphi-i\sin\varphi)=\frac1R\,e^{-i\varphi}.$$

### Significato geometrico del prodotto
Moltiplicare $z$ per $w$ equivale a **ruotare** $z$ nel piano complesso di un angolo $\varphi=\arg w$ (positivo in senso antiorario) e a **dilatarlo** di un fattore $R=|w|$: una **roto-omotetia**.

![[prodotto-complessi-rotoomotetia.png]]

### Potenze
Se $z=re^{i\theta}=r(\cos\theta+i\sin\theta)$, per ogni $n\in\mathbb{N}$:
$$z^n=r^n(\cos n\theta+i\sin n\theta)=r^ne^{in\theta},$$
e se $z\neq0$:
$$z^{-n}=\frac1{r^n}(\cos n\theta-i\sin n\theta)=r^{-n}e^{-in\theta}.$$
Sono formule **coerenti con l'algebra degli esponenziali**, anche se coinvolgono numeri complessi.

**Esempio.** $z=-1-i\sqrt3$, $n=7$. Si ha $r=\sqrt{1+3}=2$, $\cos\theta=-\tfrac12$, $\sin\theta=-\tfrac{\sqrt3}2$, $\tan\theta=\sqrt3$, quindi (III quadrante)
$$\theta=\arctan\sqrt3+\pi=\frac\pi3+\pi=\frac43\pi,\qquad z=2e^{i\frac43\pi}.$$
$$z^7=2^7e^{i\frac{28}3\pi}=2^7e^{i\frac43\pi}=2^7\left(\cos\tfrac43\pi+i\sin\tfrac43\pi\right)=2^7\left(-\tfrac12-i\tfrac{\sqrt3}2\right)=-2^6-2^6\sqrt3\,i.$$
(Si è usato $\tfrac{28}3\pi=\tfrac43\pi+8\pi$.)

![[esempio-z-meno1-meno-i-radice3.png]]

---
Precedente: [[Forma Trigonometrica ed Esponenziale]] · Successivo: [[Radici n-esime Complesse]]
