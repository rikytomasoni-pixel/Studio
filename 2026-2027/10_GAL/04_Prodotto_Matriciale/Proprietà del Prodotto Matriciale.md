---
created: 2026-10-01
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/prodotto_matriciale
aliases: []
origine: UpdateVault
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Proprietà del Prodotto Matriciale

> [!abstract] Teorema (Proprietà)
> $M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(n,p) \to M_{\mathbb{K}}(m,p)$ ([[Prodotto Righe per Colonne]])
>
> - **Proprietà distributiva a destra** $\forall A \in M_{\mathbb{K}}(m,n)$, $\forall B, C \in M_{\mathbb{K}}(n,p)$:
> $$A(B+C) = AB + AC$$
> ($B+C \in M_{\mathbb{K}}(n,p)$; $AB, AC \in M_{\mathbb{K}}(m,p)$)

**Attenzione all'efficienza computazionale:** ([[Efficienza Computazionale]])


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
> Chi sono $N_D$ e $N_S$? → [[Matrice Identità e Matrici Diagonali]]

---
Precedente: [[PageRank e Matrice di Google]] · Successivo: [[Matrice Identità e Matrici Diagonali]]
