---
tags: [GAL, matrici, composizione, funzioni, lezione-4]
data: 2026-10-01
lezione: 4
fonte: "GAL_2026-2027_-_20261001_-_LEZIONE_4.pdf (slide 38-39)"
---

# Il prodotto codifica la composizione di funzioni

> [!example] Esempio
> $F = \{\text{arancia, limone, lampone}\}$, $L = \{\text{"a", "b", "l"}\}$, $T = \{\text{vocale, consonante}\}$
> $A : F \to L$ ($\in F$ ha iniziale $\in L$), $\quad B : L \to T$ ($\in L$ è una $\in T$)
>
> $A$ (righe "a", "b", "l"; colonne arancia, limone, lampone) e $B$ (righe vocale, consonante; colonne "a", "b", "l"):
> $$A = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}, \qquad B = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}$$
> (matrici costruite come in [[30_Matrici_come_Rappresentazione_di_Funzioni]])
>
> **Posso moltiplicare $A$ e $B$? In che ordine?**
> - $A \cdot B$ non si può calcolare
> - $B \cdot A$ si può calcolare
> $$BA = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}$$
> con righe vocale, consonante e colonne arancia, limone, lampone.

**!!!** (disegno: tre insiemi $F \to L \to T$ con frecce blu ($A$) e verdi ($B$) e frecce rosse della composizione direttamente da $F$ a $T$)

> [!abstract] Teorema (Morale)
> Il prodotto matriciale ([[41_Prodotto_Matriciale_Righe_per_Colonne]]) è congeniale per poter **codificare la composizione funzionale**!!!

## Note collegate
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[16_Funzioni]]
- [[30_Matrici_come_Rappresentazione_di_Funzioni]]
- [[43_PageRank_e_Matrice_di_Google]]
- Indice: [[05_Indice_Lezione_4]] · [[00_MOC_GAL]]
