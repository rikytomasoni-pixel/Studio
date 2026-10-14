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

# Forma Trigonometrica ed Esponenziale

Sia $z=x+iy\in\mathbb{C}$, con $x=\operatorname{Re}z$, $y=\operatorname{Im}z$, $\rho=|z|$, $\theta=\arg z$.

![[numero-complesso-modulo-argomento-II-quadrante.png]]

**Argomento principale** di $z\in\mathbb{C}\setminus\{0\}$: l'unico argomento di $z$ in $[0,2\pi)$ oppure in $[-\pi,\pi)$, a seconda delle convenzioni.

**Definizione.** Dato $z=x+iy$:
- $z=x+iy$ è la **forma algebrica**;
- $z=\rho(\cos\theta+i\sin\theta)$ è la **forma trigonometrica**.

Qui $x,y\in\mathbb{R}$, $\rho\in[0,\infty)$, $\theta\in\mathbb{R}$.

**Esempio.** $z=-1=-1+i0$.
- $-1\,(\cos0+i\sin0)$ è algebricamente corretta, ma **NON** è forma trigonometrica (il modulo deve essere $\ge0$).
- $1\,(\cos\pi+i\sin\pi)$ **sì**: $1=|-1|$ e $\pi=\arg(-1)$.

**Forma esponenziale.**
$$z=x+iy=\rho(\cos\theta+i\sin\theta)=\rho\,e^{i\theta}.$$

> **Formula di Eulero.** $\forall\theta\in\mathbb{R}:\ e^{i\theta}=\cos\theta+i\sin\theta$. In particolare $e^{i\pi}+1=0$.

---
Precedente: [[Modulo e Argomento]] · Successivo: [[Formule di de Moivre]]
