---
tags: [GAL, matrici, definizione, lezione-3]
data: 2026-09-30
lezione: 3
fonte: "GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 25, 27)"
---

# Definizione di matrice

**Caratteristiche comuni**
- Abbiamo studiato funzioni con dominio un prodotto cartesiano di insiemi finiti ([[30_Matrici_come_Rappresentazione_di_Funzioni]]).
- Il codominio delle funzioni è sempre stato un insieme di numeri (campo: vedi [[31_Il_Campo_F2]]).

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

## Note collegate
- [[30_Matrici_come_Rappresentazione_di_Funzioni]]
- [[31_Il_Campo_F2]]
- [[33_Matrici_Casi_Speciali]]
- [[34_Confronto_e_Uguaglianza_tra_Matrici]]
- Indice: [[04_Indice_Lezione_3]] · [[00_MOC_GAL]]
