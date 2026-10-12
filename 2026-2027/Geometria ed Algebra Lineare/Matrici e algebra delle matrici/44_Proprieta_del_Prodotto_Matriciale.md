---
tags: [GAL, matrici, prodotto-matriciale, proprieta, lezione-4]
data: 2026-10-01
lezione: 4
fonte: "GAL_2026-2027_-_20261001_-_LEZIONE_4.pdf (slide 42-43)"
---

# Proprietà del prodotto matriciale

> [!abstract] Teorema (Proprietà)
> $M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(n,p) \to M_{\mathbb{K}}(m,p)$ ([[41_Prodotto_Matriciale_Righe_per_Colonne]])
>
> - **Proprietà distributiva a destra** $\forall A \in M_{\mathbb{K}}(m,n)$, $\forall B, C \in M_{\mathbb{K}}(n,p)$:
> $$A(B+C) = AB + AC$$
> ($B+C \in M_{\mathbb{K}}(n,p)$; $AB, AC \in M_{\mathbb{K}}(m,p)$)

**Attenzione all'efficienza computazionale:** ([[37_Efficienza_Computazionale]])


> [!abstract] Teorema (Proprietà)
> - **Proprietà distributiva a sinistra** $\forall A, B \in M_{\mathbb{K}}(m,n)$, $\forall C \in M_{\mathbb{K}}(n,p)$:
> $$(A+B)C = AC + BC$$
> - **Proprietà associativa** $\forall A \in M_{\mathbb{K}}(m,n)$, $\forall B \in M_{\mathbb{K}}(n,p)$, $\forall C \in M_{\mathbb{K}}(p,q)$:
> $$(AB)C = A(BC) = ABC$$
> con $AB \in M_{\mathbb{K}}(m,p)$ e $BC \in M_{\mathbb{K}}(n,q)$.
> - **Proprietà di omogeneità** $\forall \lambda \in \mathbb{K}$, $\forall A \in M_{\mathbb{K}}(m,n)$, $\forall B \in M_{\mathbb{K}}(n,p)$:
> $$\lambda(AB) = (\lambda A)B = A(\lambda B)$$
> - **Esistenza dell'elemento neutro** (rispetto al prodotto):
>   - *a destra:* $\exists\, N_D \in M_{\mathbb{K}}(n,n)$ t.c. $\forall A \in M_{\mathbb{K}}(m,n)$: $A N_D = A$
>   - *a sinistra:* $\exists\, N_S \in M_{\mathbb{K}}(m,m)$ t.c. $\forall A \in M_{\mathbb{K}}(m,n)$: $N_S A = A$

> [!note] Osservazione (Domanda)
> Chi sono $N_D$ e $N_S$? → [[45_Matrice_Identita_e_Matrici_Diagonali]]

## Note collegate
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[45_Matrice_Identita_e_Matrici_Diagonali]]
- [[37_Efficienza_Computazionale]]
- [[36_Prodotto_di_una_Matrice_per_uno_Scalare]]
- [[62_Non_Commutativita_del_Prodotto_Matriciale]]
- Indice: [[05_Indice_Lezione_4]] · [[00_MOC_GAL]]
