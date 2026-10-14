---
created: 2026-10-08
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/rango_e_determinante
aliases: []
origine: UpdateVault
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Teorema di Binet

> [!abstract] Teorema (Teorema di Binet)
> $A, B \in M_{\mathbb{K}}(n,n)$ $\quad (AB \in M_{\mathbb{K}}(n,n))$
> $$\det(AB) = \det(A)\det(B)$$
> [annotazioni: $\det(AB)$ — prodotto matriciale; $\det(A)\det(B)$ — prodotto tra numeri di $\mathbb{K}$]

## Conseguenze
- In generale $AB \neq BA$ (prodotto NON è commutativo, vedi [[Non Commutatività del Prodotto]]):
$$\det(AB) \overset{\text{TEO. BINET}}{=} \det(A)\det(B) \overset{\text{prodotto in } \mathbb{K} \text{ è commutativo}}{=} \det(B)\det(A) \overset{\text{TEO. BINET}}{=} \det(BA)$$

- $A \in M_{\mathbb{K}}(n,n)$, $B \in M_{\mathbb{K}}(n,n)$ ottenuta da $A$ con una sequenza di operazioni elementari ([[Codifica del MEG con il Prodotto]]):
$$\exists\, T \in M_{\mathbb{K}}(n,n) \text{ tale che } B = TA, \qquad \exists\, Z \in M_{\mathbb{K}}(n,n) \text{ tale che } A = ZB$$
Per il teorema di Binet:
  - (I) $\det(B) = \det(TA) = \det(T)\det(A)$
  - (II) $\det(A) = \det(ZB) = \det(Z)\det(B)$

  (I) $\det(A) = 0 \Rightarrow \det(B) = 0$
  (II) $\det(B) = 0 \Rightarrow \det(A) = 0$

$$\det(A) = 0 \iff \det(B) = 0$$
equivalentemente
$$\det(A) \neq 0 \iff \det(B) \neq 0$$

Applicazione al calcolo con il MEG: [[Calcolo del Determinante con il MEG]].

---
Precedente: [[Matrici Triangolari]] · Successivo: [[Calcolo del Determinante con il MEG]]
