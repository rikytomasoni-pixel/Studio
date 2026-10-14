---
created: 2026-09-30
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
origine: UpdateVault
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Definizione di Matrice

**Caratteristiche comuni**
- Abbiamo studiato funzioni con dominio un prodotto cartesiano di insiemi finiti ([[Matrici come Rappresentazione di Funzioni]]).
- Il codominio delle funzioni è sempre stato un insieme di numeri (campo: vedi [[Il Campo F2]]).

Notazione:
$[m] = \{1, 2, \dots, m\}$, $[n] = \{1, 2, \dots, n\}$
$$[m] \times [n] = \{(1,1),(1,2),\dots,(1,n),\ (2,1),(2,2),\dots,(2,n),\ \dots,\ (m,1),(m,2),\dots,(m,n)\}$$

> [!warning] Def. 3.1 Matrice
> Una **matrice** $A$ è una funzione
> $$A : [m] \times [n] \to \mathbb{K}$$
> dove $\mathbb{K}$ è un campo arbitrario ($\mathbb{Q}, \mathbb{R}, \mathbb{C}, \mathbb{F}_2, \dots$).
> Ovvero $A$ è una tabella con $m$ righe e $n$ colonne contenente valori in $\mathbb{K}$:
> $$\begin{bmatrix} A(1,1) & A(1,2) & \cdots & A(1,n) \\ \vdots & & & \vdots \\ A(m,1) & \cdots & \cdots & A(m,n) \end{bmatrix} = \begin{bmatrix} a_{11} & a_{12} & a_{13} & \cdots & a_{1n} \\ \vdots & & & & \\ a_{m1} & a_{m2} & \cdots & \cdots & a_{mn} \end{bmatrix}$$
> $a_{ij} = A(i,j)$, $i$ indice di riga, $j$ indice di colonna.

---
Precedente: [[Il Campo F2]] · Successivo: [[Casi Speciali di Matrici]]
