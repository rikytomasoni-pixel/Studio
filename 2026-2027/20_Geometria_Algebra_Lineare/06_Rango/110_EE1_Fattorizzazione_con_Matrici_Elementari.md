---
tags: [GAL, esercizio, MEG, matrici-elementari, prodotto-matriciale, fattorizzazione]
data: 2026-10-09
lezione: esercizi
fonte: "esempio.pdf (pag. 1) — EE1, codifica del MEG con matrici elementari"
---

# EE1: codifica del MEG con matrici elementari e fattorizzazione $A=PLU$

Come in [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]], ogni operazione del MEG su $A$ ([[109_EE1_Riduzione_a_Scala_di_A]]) è un prodotto a sinistra per una matrice elementare. Notazione degli appunti: $S_{ij}$ per lo scambio e $L_{ij}(c)$ per la sostituzione.

> [!note] Osservazione (non presente negli appunti)
> Convenzione dedotta dai calcoli: $S_{ij}$ è l'identità con le righe $i,j$ scambiate; $L_{ij}(c)=I+c\,E_{ij}$ (identità con $c$ in posizione $(i,j)$), cioè $L_{ij}(c)\,M$ somma $c\cdot$(riga $j$) alla riga $i$. Quindi $L_{ij}(c)^{-1}=L_{ij}(-c)$ e $S_{ij}^{-1}=S_{ij}$.

## Riduzione codificata
Le mosse eseguite sono, nell'ordine: $S_{12},\ L_{31}(-2),\ L_{41}(-1),\ S_{23},\ L_{32}(-2),\ L_{42}(-2),\ L_{43}(3)$, e
$$L_{43}(3)\,L_{42}(-2)\,L_{32}(-2)\,S_{23}\,L_{41}(-1)\,L_{31}(-2)\,S_{12}\;A=U.$$
Per la [[70_Reversibilita_del_MEG]] si inverte ogni mossa (in ordine opposto):
$$A=S_{12}\,L_{31}(2)\,L_{41}(1)\,S_{23}\,L_{32}(2)\,L_{42}(2)\,L_{43}(-3)\,U$$

> [!warning] Differenza rispetto al quaderno
> Il quaderno scrive $L_{43}(-1)$ e nella matrice $L$ l'elemento $-1$ in posizione $(4,3)$; il valore corretto è $-3$ (vedi [[109_EE1_Riduzione_a_Scala_di_A]]).

## Riordino dei fattori
Gli scambi vengono spostati a sinistra. Sono evidenziati negli appunti due fatti:
1. $S_{23}$ commuta con $L_{41}(1)$ (agiscono su righe disgiunte: $S_{23}$ sulle righe $2,3$, $L_{41}(1)$ sulle righe $4,1$):
$$A=S_{12}\,L_{31}(2)\,S_{23}\,L_{41}(1)\,L_{32}(2)\,L_{42}(2)\,L_{43}(-3)\,U$$
2. Portando $S_{23}$ davanti a $L_{31}(2)$ questa diventa $L_{21}(2)$ (le righe $2$ e $3$ si sono scambiate): $L_{31}(2)\,S_{23}=S_{23}\,L_{21}(2)$, quindi
$$A=S_{12}\,S_{23}\,L_{21}(2)\,L_{41}(1)\,L_{32}(2)\,L_{42}(2)\,L_{43}(-3)\,U$$

Si ottiene $A=P\,L\,U$ con $P=S_{12}S_{23}$ e $L=L_{21}(2)L_{41}(1)L_{32}(2)L_{42}(2)L_{43}(-3)$:
$$P=\begin{bmatrix}e_3^{T}\\ e_1^{T}\\ e_2^{T}\\ e_4^{T}\end{bmatrix}=\begin{bmatrix}0&0&1&0\\1&0&0&0\\0&1&0&0\\0&0&0&1\end{bmatrix},\qquad L=\begin{bmatrix}1&0&0&0\\2&1&0&0\\0&2&1&0\\1&2&-3&1\end{bmatrix},\qquad U=\begin{bmatrix}1&1&1\\0&1&-1\\0&0&-1\\0&0&0\end{bmatrix}$$

Il prodotto $PL$ (permuta le righe di $L$) è
$$PL=\begin{bmatrix}0&2&1&0\\1&0&0&0\\2&1&0&0\\1&2&-3&1\end{bmatrix}$$
che è la matrice usata nel passo finale ([[111_EE1_Somma_di_Tre_Matrici_di_Rango_1]]).

> [!note] Osservazione (non presente negli appunti)
> $L$ è triangolare inferiore con diagonale $1$ e sotto la diagonale ci sono i moltiplicatori dell'eliminazione cambiati di segno ($2,\,1,\,2,\,2,\,-3$) ([[66_Matrici_Triangolari]]). Verifica: $PLU=A$ riga per riga.

## Note collegate
- [[108_Esercizio_EE1_Somma_di_Matrici_di_Rango_1]]
- [[109_EE1_Riduzione_a_Scala_di_A]]
- [[111_EE1_Somma_di_Tre_Matrici_di_Rango_1]]
- [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]
- [[70_Reversibilita_del_MEG]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[00_MOC_GAL]]

#GAL/metodo-di-eliminazione-di-gauss/ee1-fattorizzazione-con-matrici-elementari
