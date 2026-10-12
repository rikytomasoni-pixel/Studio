---
tags:
  - AM1
  - numeri-complessi
  - equazioni
  - teorema-fondamentale-dell-algebra
data: 2026-09-18
fonte: Lezione 3 e Lezione 4
---

# Equazioni in campo complesso

## Esempio di equazione con parte reale, parte immaginaria e coniugato

**Esempio.** Risolvere in $\mathbb{C}$:
$$z^2+2\operatorname{Re} z - i\operatorname{Im} z + \overline{z} = 0$$

Poniamo $z=x+iy\in\mathbb{C}$, $x,y\in\mathbb{R}$:
$$(x+iy)^2+2x-iy+x-iy = 0$$
$$x^2+2xyi-y^2+2x-iy+x-iy=0$$
$$\left(x^2-y^2+3x\right) + i\left(2xy-2y\right) = 0+i0$$

$$\begin{cases} x^2-y^2+3x=0 & \operatorname{Re}(\cdots)=\operatorname{Re} 0 = 0 \\[4pt] 2xy-2y=0 & \operatorname{Im}(\cdots)=\operatorname{Im} 0 = 0 \end{cases}$$

**Un'equazione in $\mathbb{C}$ in una variabile complessa $z\in\mathbb{C}$ equivale a un sistema di due equazioni nelle variabili reali $(x,y)\in\mathbb{R}^2$.**

Dalla seconda equazione: $2y(x-1)=0 \Rightarrow y=0$ oppure $x=1$.

$$\begin{cases} x=0 \\ y=0 \end{cases} \quad \lor \quad \begin{cases} x=-3 \\ y=0 \end{cases} \quad \lor \quad \begin{cases} y=2 \\ x=1 \end{cases} \quad \lor \quad \begin{cases} y=-2 \\ x=1 \end{cases}$$

$$\Rightarrow \quad z_0=0, \quad z_1=-3, \quad z_2=1+2i, \quad z_3=1-2i$$

**Osservazione.** In questo sistema $x,y\in\mathbb{R}$.

## Equazioni di secondo grado in $\mathbb{C}$

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

### Note collegate
- [[00_MOC_A1]]
- [[13_Numeri_Complessi]] — forma algebrica, parte reale e immaginaria
- [[14_Piano_di_Argand_Gauss]] — coniugato e modulo
- [[17_Radici_Complesse]] — radici quadrate complesse di $\Delta$