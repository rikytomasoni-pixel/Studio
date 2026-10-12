---
tags: [GAL, matrici, operazioni-elementari, MEG, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 56-57)"
---

# Operazioni elementari sulle righe

Per passare da INPUT a OUTPUT del [[68_Metodo_di_Eliminazione_di_Gauss]] posso usare una sequenza di 3 operazioni elementari:
- scambio di due righe
- moltiplicazione di una riga per uno scalare $\neq 0$
- sostituzione di una riga con la somma della riga sostituita con un multiplo di un'altra riga

> [!example] Scambio
> $$\begin{bmatrix} 0 & 0 & 1 \\ 2 & 3 & 7 \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} 2 & 3 & 7 \\ 0 & 0 & 1 \end{bmatrix}$$

> [!example] Moltiplicazione di una riga per uno scalare $\neq 0$
> $$\begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{8}} & 4 & 7 \end{bmatrix} \xrightarrow{\ 10^{4}\,\mathrm{II} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ \frac{1}{10^{4}} & 4\cdot10^{4} & 7\cdot10^{4} \end{bmatrix}$$

> [!example] Sostituzione di una riga con la sua somma con un multiplo di un'altra
> $$\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} \xrightarrow{\ \mathrm{II} - 4\,\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix}$$
> [annotazione: il coefficiente $4$ è ottenuto come $\frac{4}{1}$ (elemento $4$ della seconda riga fratto elemento $1$ della prima)]

La reversibilità di queste operazioni è in [[70_Reversibilita_del_MEG]]; la loro codifica con il prodotto in [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]].

## Note collegate
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]
- [[70_Reversibilita_del_MEG]]
- [[36_Prodotto_di_una_Matrice_per_uno_Scalare]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]
