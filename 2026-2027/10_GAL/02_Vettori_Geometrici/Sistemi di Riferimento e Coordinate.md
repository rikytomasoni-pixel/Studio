---
created: 2026-09-17
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/2
  - argomento/vettori_geometrici
aliases: []
---
[[00_GAL_Vettori_Geometrici|⬅️ Torna a Vettori Geometrici]]

# Sistemi di Riferimento e Coordinate

> **Definizione (riferimento affine).** Un **sistema di riferimento affine** in $\mathbb{E}^3$ è assegnato da 4 punti non complanari $(O,B_1,B_2,B_3)$.

Se i vettori $OB_1,OB_2,OB_3$ sono ortogonali e i segmenti $OB_1,OB_2,OB_3$ sono congruenti, il riferimento è **cartesiano**.

> Disegno: piano con origine $O$ e i punti $B_1,B_2$ nel piano, $B_3$ fuori dal piano, frecce $OB_1,OB_2,OB_3$.

**Osservazione.** Ogni riferimento affine induce una **biiezione** tra i punti di $\mathbb{E}^3$ e le terne di numeri reali, cioè gli elementi di $\mathbb{R}^3$ (vedi il [[2026-09-17 GAL Lezione 1|prodotto cartesiano di più insiemi]]). Preso $X\in\mathbb{E}^3$, si considera il piano per $X$ parallelo al piano coordinato $OB_2B_3$; detto $P_1$ il punto in cui incontra l'asse $OB_1$, la lunghezza di $OP_1$ rispetto all'unità $OB_1$ è l'**ascissa** di $X$. **Ordinata** e **quota** si definiscono in modo analogo.

> Disegno: assi $OB_1,OB_2,OB_3$, piano coordinato, punto $X$ con proiezioni tratteggiate e piano parallelo a $OB_2B_3$ passante per $X$.

**Osservazione (operazioni in coordinate).** Fissato un riferimento affine, se $c(A)=(a_1,a_2,a_3)^T$ e $c(B)=(b_1,b_2,b_3)^T$ allora
$$
c(O)=\begin{pmatrix}0\\0\\0\end{pmatrix},\quad
c(-A)=\begin{pmatrix}-a_1\\-a_2\\-a_3\end{pmatrix},\quad
c(A+B)=\begin{pmatrix}a_1+b_1\\a_2+b_2\\a_3+b_3\end{pmatrix},\quad
c(tA)=\begin{pmatrix}ta_1\\ta_2\\ta_3\end{pmatrix}.
$$
(Nell'originale la seconda componente di $c(A+B)$ è $a_2+b_1$: svista evidente, corretta.)

---
Precedente: [[Proprietà delle Operazioni tra Vettori]] · Successivo: [[Prodotto Interno e Ortogonalità]]
