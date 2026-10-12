---
tags: [GAL, matrici, prodotto-per-scalare, proprieta, lezione-3]
data: 2026-09-30
lezione: 3
fonte: "GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 31-32)"
---

# Prodotto di una matrice per uno scalare

> [!warning] Def. Prodotto di una matrice per uno scalare (numero)
> $$\cdot : \mathbb{K} \times M_{\mathbb{K}}(m,n) \to M_{\mathbb{K}}(m,n),\qquad (\lambda, A) \mapsto \lambda A$$
> [annotazione: $\lambda$ = lambda minuscolo (alfabeto greco)]
> $A = [a_{ij}]$, $\quad \lambda A = [\lambda\, a_{ij}]$

> [!example] Esempio
> $$2 \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} 2\cdot1 & 2\cdot2 & 2\cdot3 \\ 2\cdot4 & 2\cdot5 & 2\cdot6 \end{bmatrix} = \begin{bmatrix} 2 & 4 & 6 \\ 8 & 10 & 12 \end{bmatrix}$$

> [!abstract] Teorema (Proprietà)
> (ereditate dal prodotto nel campo $\mathbb{K}$)
> - **Proprietà distributiva a destra** $\forall \lambda \in \mathbb{K}\ \forall A,B \in M_{\mathbb{K}}(m,n)$: $\lambda(A+B) = \lambda A + \lambda B$
> - **Proprietà distributiva a sinistra** $\forall \lambda, \mu \in \mathbb{K}\ \forall A \in M_{\mathbb{K}}(m,n)$ [$\mu$ = mu minuscola]: $(\lambda + \mu)A = \lambda A + \mu A$
> - **Proprietà associativa** $\forall \lambda, \mu \in \mathbb{K}\ \forall A \in M_{\mathbb{K}}(m,n)$: $(\lambda\mu)A = \mu(\lambda A) = \lambda(\mu A)$
> - **Esistenza dell'elemento neutro** $\forall A \in M_{\mathbb{K}}(m,n)$: $1A = A$ (l'elemento $1$ di $\mathbb{K}$)

> [!note] Osservazione
> Potremmo anche definire un prodotto tra due matrici posizione per posizione, ma questa operazione non ha grande utilità. Il prodotto utile è quello righe per colonne → [[44_Proprieta_del_Prodotto_Matriciale]].

## Note collegate
- [[35_Somma_tra_Matrici]]
- [[37_Efficienza_Computazionale]]
- [[24_Proprieta_delle_Operazioni_tra_Vettori]]
- [[44_Proprieta_del_Prodotto_Matriciale]]
- Indice: [[04_Indice_Lezione_3]] · [[00_MOC_GAL]]
