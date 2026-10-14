---
created: 2026-10-07
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/rango_e_determinante
aliases: []
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Determinante e Sviluppo di Laplace

### Definizione 6.4 (sviluppo di Laplace del determinante)

Il **determinante** è una funzione $\det : M_{\mathbb{K}}(n,n) \to \mathbb{K}$ definita come:

- ($n=1$) $\det([a_{11}]) = a_{11}$.
- ($n>1$)

$$
\det(A) = \sum_{j=1}^{n} (-1)^{i+j}\, a_{ij}\, \det(\hat{A}_{ij})
$$

dove: $i$ è un indice di riga (qualsiasi) fissato; $a_{ij}$ è l'elemento di $A$ sulla $i$-esima riga e $j$-esima colonna; $\hat{A}_{ij} \in M_{\mathbb{K}}(n-1,n-1)$ è ottenuta da $A$ eliminando la $i$-esima riga e la $j$-esima colonna.

In maniera equivalente (sviluppo lungo una colonna):

$$
\det(A) = \sum_{i=1}^{n} (-1)^{i+j}\, a_{ij}\, \det(\hat{A}_{ij})
$$

con $j$ indice di colonna (qualsiasi) fissato.

### Teorema di Laplace

«Il risultato non dipende dalla scelta di riga o colonna.»

### Caso $2\times 2$

Sviluppando lungo la colonna $j=1$:

$$
\det\begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}
= (-1)^{1+1}a_{11}\det([a_{22}]) + (-1)^{2+1}a_{21}\det([a_{12}])
= a_{11}a_{22} - a_{21}a_{12}
$$

### Esempio con sviluppo lungo la prima riga

$$
B = \begin{bmatrix} 9 & 2 & -2 \\ 2 & 2 & 0 \\ -2 & 0 & 2 \end{bmatrix}
$$

$$
\begin{aligned}
\det(B) &= \sum_{j=1}^{3}(-1)^{1+j}\,b_{1j}\det\hat{B}_{1j} \\
&= 9\det\begin{bmatrix} 2 & 0 \\ 0 & 2 \end{bmatrix} - 2\det\begin{bmatrix} 2 & 0 \\ -2 & 2 \end{bmatrix} + (-2)\det\begin{bmatrix} 2 & 2 \\ -2 & 0 \end{bmatrix} \\
&= 9(2\cdot 2 - 0\cdot 0) - 2(2\cdot 2 - (-2)\cdot 0) - 2(2\cdot 0 - (-2)\cdot 2) \\
&= 9\cdot 4 - 2\cdot 4 - 2\cdot 4 = (9-4)\cdot 4 = 20
\end{aligned}
$$

> **Idea**: sfruttare a nostro vantaggio la libertà di scegliere riga/colonna nel calcolo del determinante.

Sviluppando invece lungo la colonna $j=3$ (che contiene uno zero):

$$
\begin{aligned}
\det B &= \sum_{i=1}^{3}(-1)^{i+3}\,b_{i3}\det\hat{B}_{i3} \\
&= (-2)\det\hat{B}_{13} - 0\cdot\det\hat{B}_{23} + 2\det\hat{B}_{33} \\
&= -2\det\begin{bmatrix} 2 & 2 \\ -2 & 0 \end{bmatrix} + 2\det\begin{bmatrix} 9 & 2 \\ 2 & 2 \end{bmatrix} \\
&= -2(2\cdot 0 - (-2)\cdot 2) + 2(9\cdot 2 - 2\cdot 2) = -2\cdot 4 + 2\cdot 14 = 2(-4+14) = 20
\end{aligned}
$$

> **Obiettivo**: selezionare una riga/una colonna con più zeri possibile.

### Esempi

**(I)** Se $A \in M_{\mathbb{K}}(n,n)$ ha una riga o una colonna tutta di zeri $\Rightarrow$ $\det(A) = 0$.

---
Precedente: [[Rango e Probabilità Congiunta]] · Successivo: [[Matrici Triangolari]]
