---
tags: [GAL, matrici, prodotto-matriciale, commutativita, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 48)"
---

# Non commutatività del prodotto matriciale

Non commutatività del prodotto matriciale ([[41_Prodotto_Matriciale_Righe_per_Colonne]]): in generale il prodotto $AB \neq BA$ anche quando ha senso calcolare entrambi i prodotti.

> [!example] Esempio
> $A \in M_{\mathbb{K}}(1,n)$, $\quad B \in M_{\mathbb{K}}(n,1)$
> $$AB = \begin{bmatrix} a_{11} & \cdots & a_{1n} \end{bmatrix} \begin{bmatrix} b_{11} \\ \vdots \\ b_{n1} \end{bmatrix} = \begin{bmatrix} a_{11}b_{11} + \cdots + a_{1n}b_{n1} \end{bmatrix} \in M_{\mathbb{K}}(1,1)$$
> $$BA = \begin{bmatrix} b_{11} \\ \vdots \\ b_{n1} \end{bmatrix} \begin{bmatrix} a_{11} & \cdots & a_{1n} \end{bmatrix} = \begin{bmatrix} b_{11}a_{11} & \cdots & b_{11}a_{1n} \\ b_{21}a_{11} & & \vdots \\ \vdots & & \\ b_{n1}a_{11} & \cdots & b_{n1}a_{1n} \end{bmatrix} \in M_{\mathbb{K}}(n,n)$$
> [annotazioni rosse: $2n$ elementi (i due fattori); $n^2$ elementi (il prodotto $BA$)]

**Obiettivo:** trovare un modo efficiente di descrivere le matrici → [[63_Rango_di_una_Matrice]].

## Note collegate
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[44_Proprieta_del_Prodotto_Matriciale]]
- [[63_Rango_di_una_Matrice]]
- [[74_Teorema_di_Binet]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]
