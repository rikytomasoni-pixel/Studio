---
created: 2026-10-07
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/eliminazione_di_gauss
aliases: []
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# Operazioni Elementari sulle Righe

- **Input**: $A \in M_{\mathbb{K}}(m,n)$ qualsiasi.
- **Output**: $U \in M_{\mathbb{K}}(m,n)$ «con informazione concentrata nella parte in alto a destra» (se $m=n$, l'output sono triangolari superiori).

Per passare da input a output posso usare una sequenza di **3 operazioni elementari**:

1. scambio di due righe;
2. moltiplicazione di una riga per uno scalare $\neq 0$;
3. sostituzione di una riga con la somma della riga sostituita con un multiplo di un'altra riga.

**Scambio**: $\begin{bmatrix} 0 & 0 & 1 \\ 2 & 3 & 7 \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} 2 & 3 & 7 \\ 0 & 0 & 1 \end{bmatrix}$

**Moltiplicazione di una riga per uno scalare $\neq 0$**: $\begin{bmatrix} 1 & 2 & 3 \\ \tfrac{1}{10^8} & 4 & 7 \end{bmatrix} \xrightarrow{\ 10^4\,\mathrm{II} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ \tfrac{1}{10^4} & 4\cdot 10^4 & 7\cdot 10^4 \end{bmatrix}$

**Sostituzione di una riga con la sua somma con un multiplo di un'altra**: $\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} \xrightarrow{\ \mathrm{II} - 4\,\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix}$ (dove $4 = \frac{4}{1}$ è il rapporto tra i due elementi della prima colonna).

---
Successivo: [[Metodo di Eliminazione di Gauss]]
