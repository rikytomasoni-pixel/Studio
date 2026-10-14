---
created: 2026-10-08
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/eliminazione_di_gauss
aliases: []
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# Reversibilità del MEG

Ciascuna delle tre operazioni elementari si può annullare con un'operazione dello stesso tipo.

- **Scambio**: $\begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} \xrightarrow{\mathrm{I}\leftrightarrow\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix} \xrightarrow{\mathrm{I}\leftrightarrow\mathrm{II}} \begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix}$
- **Moltiplicazione per uno scalare $\neq 0$**: $\begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^8} & 3 & 7 \end{bmatrix} \xrightarrow{10^4\,\mathrm{II}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^4} & 3\cdot 10^4 & 7\cdot 10^4 \end{bmatrix} \xrightarrow{\frac{1}{10^4}\,\mathrm{II}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^8} & 3 & 7 \end{bmatrix}$
- **Sostituzione**: $\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} \xrightarrow{\mathrm{II}-4\mathrm{I}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix} \xrightarrow{\mathrm{II}+4\mathrm{I}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}$

---
Precedente: [[Pivot e Matrice a Scala]] · Successivo: [[Codifica del MEG con il Prodotto]]
