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

# Rango di una Matrice

Sia $A \in M_{\mathbb{K}}(m,n)$. Il **rango** di $A$ è

$$
r(A) = \min\left\{ r \in \mathbb{N} \ \middle|\ A = \sum_{i=1}^{r} C_i R_i \right\}
$$

dove $C_i \in M_{\mathbb{K}}(m,1)$ sono colonne e $R_i \in M_{\mathbb{K}}(1,n)$ sono righe.

## Esempi

$$
A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}
= \begin{bmatrix} 1 & 2 & 3 \\ 0 & 0 & 0 \end{bmatrix} + \begin{bmatrix} 0 & 0 & 0 \\ 4 & 5 & 6 \end{bmatrix}
= \begin{bmatrix} 1 \\ 0 \end{bmatrix}\begin{bmatrix} 1 & 2 & 3 \end{bmatrix} + \begin{bmatrix} 0 \\ 1 \end{bmatrix}\begin{bmatrix} 4 & 5 & 6 \end{bmatrix}
$$

N.B. $r(A) \le 2$. Allo stesso modo, scrivendola come somma di tre matrici con una sola colonna non nulla:

$$
\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}
= \begin{bmatrix} 1 \\ 4 \end{bmatrix}\begin{bmatrix} 1 & 0 & 0 \end{bmatrix} + \begin{bmatrix} 2 \\ 5 \end{bmatrix}\begin{bmatrix} 0 & 1 & 0 \end{bmatrix} + \begin{bmatrix} 3 \\ 6 \end{bmatrix}\begin{bmatrix} 0 & 0 & 1 \end{bmatrix}
$$

N.B. $r(A) \le 3$.

> **Osservazione**: per $A \in M_{\mathbb{K}}(m,n)$ vale $0 \le r(A) \le \min(m,n)$, e $r(A) = 0 \iff A$ è la matrice nulla.

---
Successivo: [[Rango e Probabilità Congiunta]]
