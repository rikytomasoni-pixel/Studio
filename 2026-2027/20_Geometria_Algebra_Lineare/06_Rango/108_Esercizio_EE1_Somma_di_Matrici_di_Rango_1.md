---
tags: [GAL, esercizio, rango, MEG, matrici-elementari, decomposizione]
data: 2026-10-09
lezione: esercizi
fonte: "esempio.pdf (pag. 1) — EE1, appunti del 9 ottobre 2026"
---

# Esercizio EE1: scrivere una matrice come somma di matrici di rango 1

> [!question] Testo (EE1)
> Scrivere la matrice
> $$A=\begin{bmatrix}0&2&-3\\1&1&1\\2&3&1\\1&3&2\end{bmatrix}$$
> come somma di $r$ matrici di rango $1$, dove $r=r(A)$.

## Idea dello svolgimento
Si usa la [[63_Rango_di_una_Matrice]] ($r(A)$ = minimo numero di addendi $C_iR_i$) insieme al [[68_Metodo_di_Eliminazione_di_Gauss]] e alla sua codifica con il prodotto ([[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]):

| Passo | Nota | Risultato |
|---|---|---|
| 1. Riduzione a scala con il MEG (due scambi di righe) | [[109_EE1_Riduzione_a_Scala_di_A]] | $U$ con $3$ pivot, quindi $r(A)=3$ |
| 2. Codifica con matrici elementari e riordino | [[110_EE1_Fattorizzazione_con_Matrici_Elementari]] | $A=PLU$ |
| 3. Prodotto colonna per riga | [[111_EE1_Somma_di_Tre_Matrici_di_Rango_1]] | $A=\sum_{i=1}^{3}C_iR_i$ |

> [!warning] Errore nel quaderno
> Nell'ultimo passo dell'eliminazione il quaderno riporta $-1$ al posto di $3$ (e quindi $L_{43}(-1)$ invece di $L_{43}(-3)$). Con $-1$ la somma finale darebbe l'ultima riga $(1,3,0)\neq(1,3,2)$. Nelle note ho usato i valori corretti e segnalato dove il quaderno differisce: dettagli in [[109_EE1_Riduzione_a_Scala_di_A]].

> [!note] Osservazione (non presente negli appunti)
> Questa è l'«esercitazione» annunciata alla fine della [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]] («Domani a esercitazione maggiori dettagli»): il MEG viene codificato con prodotti di matrici elementari. Il risultato $A=PLU$ è la cosiddetta fattorizzazione LU con permutazioni (il nome non compare negli appunti).

## Note collegate
- [[63_Rango_di_una_Matrice]]
- [[73_MEG_e_Rango]]
- [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]
- [[103_Esercizio_5_1_Calcolo_del_Determinante]] (altro esercizio del 09-10)
- [[00_MOC_GAL]]

#GAL/rango/esercizio-ee1-somma-di-matrici-di-rango-1
