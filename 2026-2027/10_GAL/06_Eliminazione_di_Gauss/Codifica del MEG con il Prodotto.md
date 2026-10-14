---
created: 2026-10-08
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/eliminazione_di_gauss
aliases: []
origine: UpdateVault
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# Codifica del MEG con il Prodotto

> [!note] Osservazione (Commento 2)
> **COMMENTO 2:** il processo di riduzione con il MEG può essere codificato con il prodotto matriciale ([[Prodotto Righe per Colonne]]).

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

Conseguenza (matrici inverse): [[Esistenza della Matrice Inversa]].

---
Precedente: [[Reversibilità del MEG]] · Successivo: [[Esistenza della Matrice Inversa]]
