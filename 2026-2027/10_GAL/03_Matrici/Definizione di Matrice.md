---
created: 2026-09-30
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Definizione di Matrice

### Definizione 3.1

Una **matrice** $A$ è una funzione

$$
A : [m] \times [n] \to \mathbb{K}
$$

dove $\mathbb{K}$ è un campo numerico ($\mathbb{Q}, \mathbb{R}, \mathbb{C}, \mathbb{F}_2, \dots$). Ovvero $A$ è una tabella con $m$ righe e $n$ colonne contenente valori in $\mathbb{K}$:

$$
A = \begin{bmatrix} A(1,1) & A(1,2) & \cdots & A(1,n) \\ \vdots & & & \vdots \\ A(m,1) & A(m,2) & \cdots & A(m,n) \end{bmatrix}
= \begin{bmatrix} a_{11} & a_{12} & a_{13} & \cdots & a_{1n} \\ \vdots & & & & \vdots \\ a_{m1} & a_{m2} & & \cdots & a_{mn} \end{bmatrix}
$$

con $a_{ij} = A(i,j)$, dove $i$ è l'**indice di riga** e $j$ l'**indice di colonna**.

---
Precedente: [[Il Campo F2]] · Successivo: [[Casi Speciali di Matrici]]
