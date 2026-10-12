---
tags: [GAL, matrici, determinante, proprieta, alternanza, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 69-70)"
---

# Determinante normalizzato e alternante

## Proprietà del determinante

> [!abstract] Teorema (Proprietà — il determinante è normalizzato)
> $$\det \mathrm{Id}_n = \det \begin{bmatrix} 1 & & 0 \\ & \ddots & \\ 0 & & 1 \end{bmatrix} = 1 \cdots 1 = 1$$
> [annotazioni: $\mathrm{Id}_n$ = elemento neutro del prodotto matriciale; $1$ = elemento neutro del prodotto in $\mathbb{K}$]

> [!abstract] Teorema (Proprietà — il determinante è alternante)
> $A \overset{\text{scambio di righe}}{\leadsto} B \Rightarrow \det(B) = -\det(A)$

> [!example] Esempio
> $$A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } B = \begin{bmatrix} c & d \\ a & b \end{bmatrix}$$
> $\det(A) = ad - bc$, $\qquad \det(B) = cb - ad = -(ad - bc)$

Una conseguenza dell'alternanza è in [[79_Determinante_con_Righe_Uguali]].

## Note collegate
- [[77_Determinante_Multilineare]]
- [[78_Determinante_e_Sostituzione]]
- [[79_Determinante_con_Righe_Uguali]]
- [[65_Determinante_Sviluppo_di_Laplace]]
- Indice: [[08_Indice_Lezione_7]] · [[00_MOC_GAL]]
