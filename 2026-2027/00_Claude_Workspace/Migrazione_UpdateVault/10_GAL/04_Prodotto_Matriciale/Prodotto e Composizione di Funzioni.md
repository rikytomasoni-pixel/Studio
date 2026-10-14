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

# Prodotto e Composizione di Funzioni

> [!example] Esempio
> $F = \{\text{arancia, limone, lampone}\}$, $L = \{\text{"a", "b", "l"}\}$, $T = \{\text{vocale, consonante}\}$
> $A : F \to L$ ($\in F$ ha iniziale $\in L$), $\quad B : L \to T$ ($\in L$ è una $\in T$)
>
> $A$ (righe "a", "b", "l"; colonne arancia, limone, lampone) e $B$ (righe vocale, consonante; colonne "a", "b", "l"):
> $$A = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}, \qquad B = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}$$
> (matrici costruite come in [[Matrici come Rappresentazione di Funzioni]])
>
> **Posso moltiplicare $A$ e $B$? In che ordine?**
> - $A \cdot B$ non si può calcolare
> - $B \cdot A$ si può calcolare
> $$BA = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix} \begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}$$
> con righe vocale, consonante e colonne arancia, limone, lampone.

**DISEGNO NON RAPPRESENTABILE** (disegno: tre insiemi $F \to L \to T$ con frecce blu ($A$) e verdi ($B$) e frecce rosse della composizione direttamente da $F$ a $T$) *(dove cercarlo: GAL_2026-2027_-_20261001_-_LEZIONE_4.pdf (slide 38-39))*

> [!abstract] Teorema (Morale)
> Il prodotto matriciale ([[Prodotto Righe per Colonne]]) è congeniale per poter **codificare la composizione funzionale**!!!

---
Precedente: [[Prodotto Righe per Colonne]] · Successivo: [[PageRank e Matrice di Google]]
