---
tags: [GAL, matrici, rango, definizione, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 48-49)"
---

# Rango di una matrice

> [!warning] Def. 6.3 Rango
> Sia $A \in M_{\mathbb{K}}(m,n)$. Il **rango** di $A$ è
> $$r(A) = \min\left\{\, r \in \mathbb{N} \ \Big|\ A = \sum_{i=1}^{r} C_i R_i \,\right\}$$
> $C_i$ colonna $\in M_{\mathbb{K}}(m,1)$ ([[33_Matrici_Casi_Speciali]]), $R_i$ riga $\in M_{\mathbb{K}}(1,n)$.

> [!example] Esempi
> $$A = \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & 0 & 0 \end{bmatrix} + \begin{bmatrix} 0 & 0 & 0 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix} \begin{bmatrix} 1 & 2 & 3 \end{bmatrix} + \begin{bmatrix} 0 \\ 1 \end{bmatrix} \begin{bmatrix} 4 & 5 & 6 \end{bmatrix}$$
> N.B. $r(A) \leq 2$
>
> $$\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 4 & 0 & 0 \end{bmatrix} + \begin{bmatrix} 0 & 2 & 0 \\ 0 & 5 & 0 \end{bmatrix} + \begin{bmatrix} 0 & 0 & 3 \\ 0 & 0 & 6 \end{bmatrix} = \begin{bmatrix} 1 \\ 4 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \end{bmatrix} + \begin{bmatrix} 2 \\ 5 \end{bmatrix} \begin{bmatrix} 0 & 1 & 0 \end{bmatrix} + \begin{bmatrix} 3 \\ 6 \end{bmatrix} \begin{bmatrix} 0 & 0 & 1 \end{bmatrix}$$
> N.B. $r(A) \leq 3$

> [!note] Osservazione
> $A \in M_{\mathbb{K}}(m,n)$: $\quad 0 \leq r(A) \leq \min(m,n)$
> $$r(A) = 0 \iff A = \begin{bmatrix} 0 & \cdots & 0 \\ \vdots & & \vdots \\ 0 & \cdots & 0 \end{bmatrix}$$

Esempio con la matrice di probabilità congiunta: [[64_Rango_e_Matrice_di_Probabilita_Congiunta]]. Calcolo efficiente del rango: [[73_MEG_e_Rango]].

## Note collegate
- [[62_Non_Commutativita_del_Prodotto_Matriciale]]
- [[64_Rango_e_Matrice_di_Probabilita_Congiunta]]
- [[73_MEG_e_Rango]]
- [[33_Matrici_Casi_Speciali]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]
