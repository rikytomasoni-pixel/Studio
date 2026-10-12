---
tags: [GAL, matrici, MEG, prodotto-matriciale, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 63-64)"
---

# Codifica del MEG con il prodotto matriciale

> [!note] Osservazione (Commento 2)
> **COMMENTO 2:** il processo di riduzione con il MEG può essere codificato con il prodotto matriciale ([[41_Prodotto_Matriciale_Righe_per_Colonne]]).

> [!example] Scambio
> $$\begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix}$$
> Cerco $S$ tale che
> $$S \begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix}, \qquad S \in M_{\mathbb{R}}(2,2), \qquad S = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$$
> $$\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix} \begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix}$$

> [!example] Moltiplicazione
> $$\begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{8}} & 3 & 7 \end{bmatrix} \xrightarrow{\ 10^{4}\,\mathrm{II} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{4}} & 3\cdot10^{4} & 7\cdot10^{4} \end{bmatrix}$$
> $$\begin{bmatrix} 1 & 0 \\ 0 & 10^{4} \end{bmatrix} \begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{8}} & 3 & 7 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{4}} & 3\cdot10^{4} & 7\cdot10^{4} \end{bmatrix}$$

> [!example] Sostituzione
> $$\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} \xrightarrow{\ \mathrm{II} - 4\,\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix}$$
> $$\begin{bmatrix} 1 & 0 \\ -4 & 1 \end{bmatrix} \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix}$$

Domani a esercitazione maggiori dettagli.

> [!abstract] Teorema (Morale)
> $A \overset{\text{MEG}}{\leadsto} U$: esiste una matrice $T$ tale che $TA = U$.

Conseguenza (matrici inverse): [[72_Esistenza_della_Matrice_Inversa]].

## Note collegate
- [[70_Reversibilita_del_MEG]]
- [[72_Esistenza_della_Matrice_Inversa]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[67_Operazioni_Elementari_sulle_Righe]]
- [[74_Teorema_di_Binet]]
- Indice: [[08_Indice_Lezione_7]] · [[00_MOC_GAL]]
