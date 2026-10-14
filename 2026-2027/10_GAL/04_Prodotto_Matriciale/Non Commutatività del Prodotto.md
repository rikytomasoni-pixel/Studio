---
created: 2026-10-07
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/prodotto_matriciale
aliases: []
origine: UpdateVault
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Non Commutatività del Prodotto

Non commutatività del prodotto matriciale ([[Prodotto Righe per Colonne]]): in generale il prodotto $AB \neq BA$ anche quando ha senso calcolare entrambi i prodotti.

> [!example] Esempio
> $A \in M_{\mathbb{K}}(1,n)$, $\quad B \in M_{\mathbb{K}}(n,1)$
> $$AB = \begin{bmatrix} a_{11} & \cdots & a_{1n} \end{bmatrix} \begin{bmatrix} b_{11} \\ \vdots \\ b_{n1} \end{bmatrix} = \begin{bmatrix} a_{11}b_{11} + \cdots + a_{1n}b_{n1} \end{bmatrix} \in M_{\mathbb{K}}(1,1)$$
> $$BA = \begin{bmatrix} b_{11} \\ \vdots \\ b_{n1} \end{bmatrix} \begin{bmatrix} a_{11} & \cdots & a_{1n} \end{bmatrix} = \begin{bmatrix} b_{11}a_{11} & \cdots & b_{11}a_{1n} \\ b_{21}a_{11} & & \vdots \\ \vdots & & \\ b_{n1}a_{11} & \cdots & b_{n1}a_{1n} \end{bmatrix} \in M_{\mathbb{K}}(n,n)$$
> [annotazioni rosse: $2n$ elementi (i due fattori); $n^2$ elementi (il prodotto $BA$)]

**Obiettivo:** trovare un modo efficiente di descrivere le matrici → [[Rango di una Matrice]].

---
Precedente: [[Matrice Invertibile]]
