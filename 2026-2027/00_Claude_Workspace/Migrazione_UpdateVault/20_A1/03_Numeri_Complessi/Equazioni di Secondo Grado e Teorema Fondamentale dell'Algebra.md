---
created: 2026-09-23
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/numeri_complessi
aliases: []
origine: UpdateVault
---
[[00_A1_Numeri_Complessi|⬅️ Torna a Numeri Complessi]]

# Equazioni di Secondo Grado e Teorema Fondamentale dell'Algebra

Se $a,b,c\in\mathbb{C}$, $a\neq 0$
$$az^2+bz+c=0$$
ha 2 soluzioni (con molteplicità) in $\mathbb{C}$. Si può sempre risolvere scrivendo $z=x+iy$, con $x,y\in\mathbb{R}$, e scrivendo il sistema equivalente di 2 equazioni reali in due variabili reali.

Alternativamente, posto $\Delta=b^2-4ac \in\mathbb{C}$
le due soluzioni sono
$$z_0,z_1 = \dfrac{-b+\sqrt\Delta}{2a} \quad \in\mathbb{C}$$
dove $\Delta\in\mathbb{C}$, $\sqrt\Delta$ sono le 2 radici quadrate complesse di $\Delta$ (2 valori complessi, opposti in segno).

Vale
$$az^2+bz+c = a(z-z_0)(z-z_1)$$

> [!abstract] Teorema fondamentale dell'algebra
> Un'equazione polinomiale della forma
> $$a_n z^n+a_{n-1}z^{n-1}+\cdots+a_1 z+a_0=0$$
> con $a_n,a_{n-1},\dots,a_1,a_0\in\mathbb{C}$, $a_n\neq 0$, $n\in\mathbb{N}$, $n\geq 1$ ha esattamente $n$ soluzioni (radici) in $\mathbb{C}$, se ciascuna di esse è contata con la dovuta molteplicità (cioè le $n$ soluzioni potrebbero non essere tutte distinte).
>
> Dette $z_0,\dots,z_{n-1}\in\mathbb{C}$ le soluzioni, allora $\forall\, z\in\mathbb{C}$ vale
> $$a_n z^n+a_{n-1}z^{n-1}+\cdots+a_1 z+a_0 = a_n(z-z_0)(z-z_1)\cdots(z-z_{n-1})$$

**Es:** $18(z-i)^4\, z^5\, (z-7i+4)^{18}=0$
ha 27 soluzioni in $\mathbb{C}$, pari al grado:
- $i$ contato 4 volte
- $0$ contato 5 volte
- $-4+7i$ contato 18 volte

**Es:** $z-\overline{z}=0$
non è un'equazione polinomiale in $z$

$$z=x+iy, \qquad \overline{z}=x-iy$$
$$0 = (x+iy)-(x-iy) = 2iy$$
$$\Rightarrow \quad y=\operatorname{Im}z=0$$
$$\Rightarrow \quad z=x+i0\in\mathbb{R} \qquad \forall\, x\in\mathbb{R}$$
$$\Rightarrow \quad \text{infinite soluzioni, tutti i numeri complessi con parte immaginaria } 0\text{, cioè i punti dell'asse reale}$$

---
Precedente: [[Radici n-esime Complesse]]
