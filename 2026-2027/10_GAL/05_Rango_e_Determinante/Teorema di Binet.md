---
created: 2026-10-08
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/rango_e_determinante
aliases: []
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Teorema di Binet

Siano $A,B \in M_{\mathbb{K}}(n,n)$ (quindi $AB \in M_{\mathbb{K}}(n,n)$):

$$
\det(AB) = \det(A)\,\det(B)
$$

(a sinistra il prodotto matriciale; a destra il prodotto tra numeri di $\mathbb{K}$).

## Conseguenze

- In generale $AB \neq BA$ (il prodotto **non** è commutativo), ma

  $$
  \det(AB) \overset{\text{Binet}}{=} \det(A)\det(B) = \det(B)\det(A) \overset{\text{Binet}}{=} \det(BA)
  $$

  perché il prodotto in $\mathbb{K}$ è commutativo.
- Sia $A \in M_{\mathbb{K}}(n,n)$ e $B \in M_{\mathbb{K}}(n,n)$ ottenuta da $A$ con una sequenza di operazioni elementari. Allora esistono $T,Z \in M_{\mathbb{K}}(n,n)$ tali che $B = TA$ e $A = ZB$. Per il teorema di Binet:

  - (I) $\det(B) = \det(TA) = \det(T)\det(A)$
  - (II) $\det(A) = \det(ZB) = \det(Z)\det(B)$

  Da (I): $\det(A) = 0 \Rightarrow \det(B) = 0$. Da (II): $\det(B) = 0 \Rightarrow \det(A) = 0$. Quindi

  $$
  \det(A) = 0 \iff \det(B) = 0, \qquad \text{equivalentemente} \qquad \det(A) \neq 0 \iff \det(B) \neq 0
  $$

---
Precedente: [[Matrici Triangolari]] · Successivo: [[Calcolo del Determinante con il MEG]]
