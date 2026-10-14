---
created: 2026-10-07
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/prodotto_matriciale
aliases: []
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Non Commutatività del Prodotto

In generale il prodotto $AB \neq BA$, anche quando ha senso calcolare entrambi i prodotti.

Siano $A \in M_{\mathbb{K}}(1,n)$ e $B \in M_{\mathbb{K}}(n,1)$:

$$
AB = \begin{bmatrix} a_{11} & \cdots & a_{1n} \end{bmatrix}\begin{bmatrix} b_{11} \\ \vdots \\ b_{n1} \end{bmatrix} = \begin{bmatrix} a_{11}b_{11} + \dots + a_{1n}b_{n1} \end{bmatrix} \in M_{\mathbb{K}}(1,1)
$$

$$
BA = \begin{bmatrix} b_{11} \\ \vdots \\ b_{n1} \end{bmatrix}\begin{bmatrix} a_{11} & \cdots & a_{1n} \end{bmatrix} = \begin{bmatrix} b_{11}a_{11} & \cdots & b_{11}a_{1n} \\ \vdots & & \vdots \\ b_{n1}a_{11} & \cdots & b_{n1}a_{1n} \end{bmatrix} \in M_{\mathbb{K}}(n,n)
$$

$BA$ è descritta da $2n$ elementi (i due vettori) ma ha $n^2$ elementi.

> **Obiettivo**: trovare un modo efficiente di descrivere le matrici.

---
Precedente: [[Matrice Invertibile]]
