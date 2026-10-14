---
created: 2026-09-30
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Prodotto di una Matrice per uno Scalare

$$
\cdot : \mathbb{K} \times M_{\mathbb{K}}(m,n) \to M_{\mathbb{K}}(m,n), \qquad (\lambda, A) \longmapsto \lambda A
$$

($\lambda$ è la lettera greca *lambda* minuscola.) Con $A = [a_{ij}]$:

$$
\lambda A = [\lambda a_{ij}]
$$

**Esempio** ($\lambda = 2$):

$$
2 \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}
= \begin{bmatrix} 2\cdot 1 & 2\cdot 2 & 2\cdot 3 \\ 2\cdot 4 & 2\cdot 5 & 2\cdot 6 \end{bmatrix}
= \begin{bmatrix} 2 & 4 & 6 \\ 8 & 10 & 12 \end{bmatrix}
$$

### Proprietà (ereditate dal prodotto nel campo $\mathbb{K}$)

- **Distributiva a destra**: $\forall \lambda \in \mathbb{K}$, $\forall A,B \in M_{\mathbb{K}}(m,n)$: $\lambda(A+B) = \lambda A + \lambda B$.
- **Distributiva a sinistra**: $\forall \lambda,\mu \in \mathbb{K}$ ($\mu$ = *mu* minuscola), $\forall A \in M_{\mathbb{K}}(m,n)$: $(\lambda+\mu)A = \lambda A + \mu A$.
- **Associativa**: $\forall \lambda,\mu \in \mathbb{K}$, $\forall A$: $(\lambda\mu)A = \mu(\lambda A) = \lambda(\mu A)$.
- **Esistenza dell'elemento neutro**: $\forall A$: $1A = A$ (dove $1$ è l'elemento $1$ di $\mathbb{K}$).

> **Osservazione**: potremmo anche definire un prodotto tra due matrici posizione per posizione, ma questa operazione non ha grande utilità.

---
Precedente: [[Somma tra Matrici]] · Successivo: [[Efficienza Computazionale]]
