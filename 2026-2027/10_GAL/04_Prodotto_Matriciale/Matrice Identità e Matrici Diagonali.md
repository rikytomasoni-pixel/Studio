---
created: 2026-10-01
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/prodotto_matriciale
aliases: []
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Matrice Identità e Matrici Diagonali

### Definizione

La **matrice identità** di tipo $(k,k)$ è la matrice

$$
\mathrm{Id}_k = \begin{bmatrix} 1 & 0 & \cdots & 0 \\ 0 & 1 & & \vdots \\ \vdots & & \ddots & 0 \\ 0 & \cdots & 0 & 1 \end{bmatrix} \in M_{\mathbb{K}}(k,k),
\qquad
(\mathrm{Id}_k)_{ij} = \begin{cases} 1 & i = j \\ 0 & i \neq j \end{cases}
$$

$\Rightarrow$ $N_D = \mathrm{Id}_n$ e $N_S = \mathrm{Id}_m$.

## Diagonale principale e matrici diagonali

### Definizione

Gli elementi che occupano le posizioni $(i,i)$ formano la **diagonale principale** di una matrice. Le matrici quadrate in cui tutte le entrate della matrice fuori dalla diagonale principale sono nulle si dicono **matrici diagonali**.

**Esempio**

$$
\begin{bmatrix} * & 0 & \cdots & 0 \\ 0 & * & & \vdots \\ \vdots & & \ddots & 0 \\ 0 & \cdots & 0 & * \end{bmatrix}
$$

dove i simboli $*$ (sulla diagonale principale) sono valori qualsiasi.

- $\mathrm{Id}_n$ è diagonale;
- la matrice nulla quadrata è diagonale;
- $\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$ **non è** una matrice diagonale (gli 1 sono sulla diagonale secondaria).

---
Precedente: [[Proprietà del Prodotto Matriciale]] · Successivo: [[Matrice Invertibile]]
