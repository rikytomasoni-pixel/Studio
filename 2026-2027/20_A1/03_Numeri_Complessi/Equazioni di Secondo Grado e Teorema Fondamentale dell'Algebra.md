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

# Equazioni di Secondo Grado e Teorema Fondamentale dell'Algebra

Se $a,b,c\in\mathbb{C}$, $a\neq0$, l'equazione $az^2+bz+c=0$ ha **2 soluzioni** (con molteplicità) in $\mathbb{C}$. Si può sempre risolvere ponendo $z=x+iy$ con $x,y\in\mathbb{R}$ e passando al sistema equivalente di due equazioni reali in due variabili reali. In alternativa, posto
$$\Delta=b^2-4ac\in\mathbb{C},$$
le due soluzioni sono
$$z_{0},z_1=\frac{-b+\sqrt\Delta}{2a},$$
dove $\sqrt\Delta$ indica le **due radici quadrate complesse** di $\Delta$ (due valori opposti in segno). Vale
$$az^2+bz+c=a(z-z_0)(z-z_1).$$

## 5. Teorema fondamentale dell'algebra

> **Teorema.** Una equazione polinomiale
> $$a_nz^n+a_{n-1}z^{n-1}+\dots+a_1z+a_0=0,\qquad a_i\in\mathbb{C},\ a_n\neq0,\ n\ge1,$$
> ha **esattamente $n$ soluzioni (radici) in $\mathbb{C}$**, se ciascuna è contata con la dovuta **molteplicità** (le $n$ soluzioni potrebbero non essere tutte distinte). Dette $z_0,\dots,z_{n-1}$ le soluzioni, $\forall z\in\mathbb{C}$:
> $$a_nz^n+\dots+a_0=a_n(z-z_0)(z-z_1)\cdots(z-z_{n-1}).$$

**Esempio.** $18(z-i)^4z^5(z-7i+4)^{18}=0$ ha $27$ soluzioni in $\mathbb{C}$, pari al grado: $i$ contato 4 volte, $0$ contato 5 volte, $-4+7i$ contato 18 volte.

**Esempio (non polinomiale).** $z-\bar z=0$ **non** è un'equazione polinomiale in $z$. Con $z=x+iy$: $0=x+iy-(x-iy)=2iy\Rightarrow y=\operatorname{Im}z=0$, quindi $z=x+i0\in\mathbb{R}$ per ogni $x\in\mathbb{R}$: **infinite soluzioni**, tutti i complessi con parte immaginaria nulla, cioè i punti dell'asse reale.

---
Precedente: [[Radici n-esime Complesse]]
