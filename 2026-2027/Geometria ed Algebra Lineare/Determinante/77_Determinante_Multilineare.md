---
tags: [GAL, matrici, determinante, proprieta, multilinearita, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 70-71)"
---

# Determinante multilineare

> [!abstract] Teorema (Proprietà — il determinante è multilineare)
> **MOLTIPLICAZIONE** — se moltiplico una riga di $A$ per $\lambda \neq 0 \in \mathbb{K}$:
> $A \overset{\text{moltiplico } R_i \text{ per } \lambda}{\leadsto} B$, allora
> $$\det(B) = \lambda \det(A)$$

> [!example] Esempio
> $$A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\ \lambda\,\mathrm{II} \to \mathrm{II}\ } \begin{bmatrix} a & b \\ \lambda c & \lambda d \end{bmatrix} = B$$
> $\det(A) = ad - bc$
> $\det(B) = a(\lambda d) - (\lambda c)b = \lambda(ad - bc) = \lambda \det A$

> [!note] Osservazione
> Anche se moltiplico una colonna per $\lambda \neq 0 \in \mathbb{K}$ il determinante viene moltiplicato per $\lambda$:
> $$\det\begin{bmatrix} \lambda a & b \\ \lambda c & d \end{bmatrix} = (\lambda a)d - (\lambda c)b = \lambda(ad - bc)$$

> [!note] Osservazione (Domanda)
> D. cosa succede se moltiplico tutta la matrice per $\lambda$?
> $$\det\left(\lambda \begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) = \det\left(\begin{bmatrix} \lambda a & \lambda b \\ \lambda c & \lambda d \end{bmatrix}\right)$$
> $$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow[\ \lambda\,\mathrm{II} \to \mathrm{II}\ ]{\ \lambda\,\mathrm{I} \to \mathrm{I}\ } \begin{bmatrix} \lambda a & \lambda b \\ \lambda c & \lambda d \end{bmatrix}$$
> $$\det\left(\lambda \begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) = \lambda^2 \det\left(\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right)$$
> $A \in M_{\mathbb{K}}(n,n)$: $\quad \det(\lambda A) = \lambda^{n}\det(A)$

## Note collegate
- [[76_Determinante_Normalizzato_e_Alternante]]
- [[78_Determinante_e_Sostituzione]]
- [[36_Prodotto_di_una_Matrice_per_uno_Scalare]]
- [[74_Teorema_di_Binet]]
- Indice: [[08_Indice_Lezione_7]] · [[00_MOC_GAL]]
