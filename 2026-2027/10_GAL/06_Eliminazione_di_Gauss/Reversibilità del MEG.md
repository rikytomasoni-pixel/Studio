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

# Reversibilità del MEG

Da ieri: $A \overset{\text{MEG}}{\leadsto} U$, con $A$ arbitraria e $U$ a scala ([[Metodo di Eliminazione di Gauss]]).

> [!note] Osservazione (Commento 1)
> **COMMENTO 1:** il processo del MEG è reversibile.

> [!example] Scambio
> $$\begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix}$$

> [!example] Moltiplicazione per uno scalare $\neq 0$
> $$\begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{8}} & 3 & 7 \end{bmatrix} \xrightarrow{\ 10^{4}\,\mathrm{II} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{4}} & 3\cdot10^{4} & 7\cdot10^{4} \end{bmatrix} \xrightarrow{\ \frac{1}{10^{4}}\,\mathrm{II} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{8}} & 3 & 7 \end{bmatrix}$$
> [lettura incerta: nell'originale l'ultimo elemento in basso a sinistra appare scritto $\frac{1}{10^{4}}$; il valore coerente con le operazioni è $\frac{1}{10^{8}}$]

> [!example] Sostituzione
> $$\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} \xrightarrow{\ \mathrm{II} - 4\,\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix} \xrightarrow{\ \mathrm{II} + 4\,\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}$$

Il secondo commento è in [[Codifica del MEG con il Prodotto]].

---
Precedente: [[Pivot e Matrice a Scala]] · Successivo: [[Codifica del MEG con il Prodotto]]
