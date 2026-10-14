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

# Modulo e Argomento

Per individuare $z\in\mathbb{C}$ si possono assegnare $\operatorname{Re}z,\operatorname{Im}z$, oppure, alternativamente, il **modulo** $\rho=|z|=\sqrt{x^2+y^2}$ (distanza da $O$) e l'**argomento** $\theta=\arg z$, l'angolo formato dal semiasse $x>0$ e dalla semiretta uscente da $O$ e passante per $z$ (positivo in senso antiorario, negativo in senso orario).

![[modulo-e-argomento.png]]

Luoghi: $|z|=\rho$ costante è una circonferenza centrata in $O$; $\arg z=\theta$ costante è una **semiretta** uscente da $O$ (esclusa $O$) che forma l'angolo orientato $\theta$ con il semiasse $x>0$.

![[luoghi-modulo-argomento-costanti.png]]

### Osservazioni
- $\arg0$ **non è ben definito**.
- L'argomento di $z\neq0$ è definito **a meno di multipli interi di $2\pi$**: se $\theta=\arg z$, anche $\theta+2k\pi$ ($k\in\mathbb{Z}$) è argomento di $z$.
- Con $\rho\ge0$, $\theta\in\mathbb{R}$:
$$\rho=\sqrt{x^2+y^2},\qquad\begin{cases}x=\rho\cos\theta\\ y=\rho\sin\theta\end{cases}$$
e per $z\neq0$:
$$\cos\theta=\frac{x}{\sqrt{x^2+y^2}}=\frac x\rho,\qquad \sin\theta=\frac{y}{\sqrt{x^2+y^2}}=\frac y\rho,\qquad \tan\theta=\frac yx\ \ (x\neq0).$$

> [!warning] Attenzione
> **Non sempre** $\theta=\arccos\frac{x}{\sqrt{x^2+y^2}}$, né $\theta=\arcsin\frac{y}{\sqrt{x^2+y^2}}$, né $\theta=\arctan\frac yx$: dipende dal **quadrante** in cui si trova $z$.

Per l'arcotangente:
$$\theta=\begin{cases}\arctan\dfrac yx & z\in\text{I, IV quadrante}\\[2mm] \arctan\dfrac yx+\pi & z\in\text{II, III quadrante}\end{cases}$$

**Esempio.** $z=-1-i$ (III quadrante): $\operatorname{Re}z=\operatorname{Im}z=-1$, $\rho=|z|=\sqrt2$, $\arctan\frac{-1}{-1}=\arctan1=\frac\pi4$, quindi
$$\theta=\arg z=\arctan\frac{\operatorname{Im}z}{\operatorname{Re}z}+\pi=\frac54\pi.$$

![[esempio-argomento-meno1-meno-i.png]]

---
Precedente: [[Equazioni in C]] · Successivo: [[Forma Trigonometrica ed Esponenziale]]
