---
tags: [GAL, matrici, determinante, proprieta, alternanza, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 72)"
---

# Determinante con righe uguali

> [!abstract] Teorema (Proprietà)
> Se una matrice ha due righe (o due colonne) uguali allora il determinante è $0$.

> [!example] Esempio (caso $2 \times 2$)
> $$B = \begin{bmatrix} a & b \\ a & b \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} a & b \\ a & b \end{bmatrix} = B'$$
> $B = B'$ (perché le righe sono uguali).
> (ALTERNANZA, [[07_Determinante_Normalizzato_e_Alternante]]) $\quad \det(B') = -\det(B)$
> $$\left.\begin{matrix} B = B' \\ \det(B') = -\det(B) \end{matrix}\right\} \Rightarrow \det(B) = -\det(B) \Rightarrow 2\det(B) = 0 \Rightarrow \det(B) = 0$$

Uso nella proprietà di sostituzione: [[09_Determinante_e_Sostituzione]].

## Note collegate
- [[07_Determinante_Normalizzato_e_Alternante]]
- [[09_Determinante_e_Sostituzione]]
- [[08_Determinante_Multilineare]]
- [[06_Determinante_Sviluppo_di_Laplace]]
- Indice: [[00_Indice_Lezione_7]] · [[00_MOC_GAL]]
