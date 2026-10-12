---
tags: [GAL, matrici, determinante, binet, teorema, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 68-69)"
---

# Teorema di Binet

> [!abstract] Teorema (Teorema di Binet)
> $A, B \in M_{\mathbb{K}}(n,n)$ $\quad (AB \in M_{\mathbb{K}}(n,n))$
> $$\det(AB) = \det(A)\det(B)$$
> [annotazioni: $\det(AB)$ — prodotto matriciale; $\det(A)\det(B)$ — prodotto tra numeri di $\mathbb{K}$]

## Conseguenze
- In generale $AB \neq BA$ (prodotto NON è commutativo, vedi [[62_Non_Commutativita_del_Prodotto_Matriciale]]):
$$\det(AB) \overset{\text{TEO. BINET}}{=} \det(A)\det(B) \overset{\text{prodotto in } \mathbb{K} \text{ è commutativo}}{=} \det(B)\det(A) \overset{\text{TEO. BINET}}{=} \det(BA)$$

- $A \in M_{\mathbb{K}}(n,n)$, $B \in M_{\mathbb{K}}(n,n)$ ottenuta da $A$ con una sequenza di operazioni elementari ([[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]):
$$\exists\, T \in M_{\mathbb{K}}(n,n) \text{ tale che } B = TA, \qquad \exists\, Z \in M_{\mathbb{K}}(n,n) \text{ tale che } A = ZB$$
Per il teorema di Binet:
  - (I) $\det(B) = \det(TA) = \det(T)\det(A)$
  - (II) $\det(A) = \det(ZB) = \det(Z)\det(B)$

  (I) $\det(A) = 0 \Rightarrow \det(B) = 0$
  (II) $\det(B) = 0 \Rightarrow \det(A) = 0$

$$\det(A) = 0 \iff \det(B) = 0$$
equivalentemente
$$\det(A) \neq 0 \iff \det(B) \neq 0$$

Applicazione al calcolo con il MEG: [[75_Calcolo_del_Determinante_con_il_MEG]].

## Note collegate
- [[65_Determinante_Sviluppo_di_Laplace]]
- [[62_Non_Commutativita_del_Prodotto_Matriciale]]
- [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]
- [[75_Calcolo_del_Determinante_con_il_MEG]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- Indice: [[08_Indice_Lezione_7]] · [[00_MOC_GAL]]
