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

# Codifica del MEG con il Prodotto

**Scambio.** Esiste $S \in M_{\mathbb{R}}(2,2)$ tale che

$$
S \begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix}, \qquad
S = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

**Moltiplicazione.**

$$
\begin{bmatrix} 1 & 0 \\ 0 & 10^4 \end{bmatrix}\begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^8} & 3 & 7 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^4} & 3\cdot 10^4 & 7\cdot 10^4 \end{bmatrix}
$$

**Sostituzione.**

$$
\begin{bmatrix} 1 & 0 \\ -4 & 1 \end{bmatrix}\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix}
$$

(Domani: maggiori dettagli sull'esecuzione.)

> **Morale**: $A \overset{\text{MEG}}{\leadsto} U$ $\Rightarrow$ esiste una matrice $T$ tale che $TA = U$.

---
Precedente: [[Reversibilità del MEG]] · Successivo: [[Esistenza della Matrice Inversa]]
