---
tags: [GAL, vettori, geometria, coordinate, riferimento, lezione-2]
data: 2026-09-17
lezione: 2
fonte: "GAL_2026-2027_-_20260917_-_LEZIONE_2.pdf (p. 3-4)"
---

# Sistemi di riferimento e coordinate

> [!warning] Def. Sistema di riferimento affine
> Un **sistema di riferimento affine** in $\mathbb{E}^3$ è assegnato da una successione di 4 punti non complanari $(O, B_1, B_2, B_3)$.

**!!!** (disegno: piano con origine $O$ e i punti $B_1, B_2$ nel piano; $B_3$ fuori dal piano, con le frecce $OB_1$, $OB_2$, $OB_3$)

Se i vettori $OB_1$, $OB_2$ e $OB_3$ sono ortogonali e i segmenti $OB_1$, $OB_2$ e $OB_3$ sono congruenti, diciamo che il riferimento è **cartesiano**.

> [!note] Osservazione
> Ogni riferimento affine induce una biiezione fra i punti di $\mathbb{E}^3$ e le terne di numeri reali (cioè gli elementi di $\mathbb{R}^3$, vedi [[19_Prodotto_Cartesiano_di_Piu_Insiemi]]).
>
> Preso $X \in \mathbb{E}^3$ consideriamo il piano passante per $X$ e parallelo al piano coordinato $OB_2B_3$; detto $P_1$ l'intersezione di questo piano con l'asse coordinato $OB_1$, la lunghezza di $OP_1$, rispetto all'unità di misura $OB_1$, è l'**ascissa** di $X$. **Ordinata** e **quota** sono definite in modo simile.

**!!!** (disegno: assi $OB_1, OB_2, OB_3$, piano coordinato $H$, punto $X$ con proiezioni tratteggiate e piano parallelo a $OB_2B_3$ passante per $X$)

> [!note] Osservazione
> Scelto un sistema di riferimento affine $(O, B_1, B_2, B_3)$, presi due vettori $u = [OA]$ e $v = [OB]$, se le coordinate di $A$ e $B$ rispetto al sistema di riferimento sono
> $$c(A) = \begin{pmatrix} a_1 \\ a_2 \\ a_3 \end{pmatrix}, \qquad c(B) = \begin{pmatrix} b_1 \\ b_2 \\ b_3 \end{pmatrix}$$
> allora
> - $O = \begin{pmatrix} 0 \\ 0 \\ 0 \end{pmatrix}$
> - $c(-A) = \begin{pmatrix} -a_1 \\ -a_2 \\ -a_3 \end{pmatrix}$
> - $c(A+B) = \begin{pmatrix} a_1+b_1 \\ a_2+b_2 \\ a_3+b_3 \end{pmatrix}$ [nell'originale la seconda componente è scritta $a_2+b_1$: svista evidente, corretta]
> - $c(tA) = \begin{pmatrix} ta_1 \\ ta_2 \\ ta_3 \end{pmatrix}$

## Note collegate
- [[22_Operazioni_tra_Vettori]]
- [[24_Proprieta_delle_Operazioni_tra_Vettori]]
- [[19_Prodotto_Cartesiano_di_Piu_Insiemi]]
- [[26_Prodotto_Interno_in_Coordinate]]
- Indice: [[03_Indice_Lezione_2]] · [[00_MOC_GAL]]
