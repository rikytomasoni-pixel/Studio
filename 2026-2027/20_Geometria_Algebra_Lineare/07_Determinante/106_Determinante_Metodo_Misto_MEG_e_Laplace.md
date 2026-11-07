---
tags: [GAL, determinante, esercizio, MEG, laplace, metodo-misto]
data: 2026-10-09
lezione: esercizi
fonte: "esempideterminante.pdf (pag. 1) — Esercizio 5.1, matrice A, «Laplace (variante)»"
---

# Determinante: metodo misto MEG + Laplace

**Idea:** si fa solo il primo passo del MEG (azzerare la prima colonna sotto il pivot, con sostituzioni) e poi si sviluppa con Laplace lungo quella colonna.

## Svolgimento
Le sostituzioni non cambiano il determinante ([[78_Determinante_e_Sostituzione]]):
$$\begin{vmatrix}1&2&3\\2&4&1\\3&1&2\end{vmatrix}=\begin{vmatrix}1&2&3\\0&0&-5\\0&-5&-7\end{vmatrix}$$
La prima colonna ha un solo elemento non nullo (riquadrata negli appunti), quindi lo sviluppo lungo $j=1$ ha un solo addendo:
$$=1\cdot C_{11}=1\cdot(-1)^{1+1}\begin{vmatrix}0&-5\\-5&-7\end{vmatrix}=1\cdot1\cdot\big(0\cdot(-7)-(-5)(-5)\big)=-25$$

> [!note] Osservazione
> - È lo stesso ragionamento usato per le matrici triangolari ([[66_Matrici_Triangolari]]): sviluppo lungo la colonna $1$ con soli zeri sotto $t_{11}$.
> - Rispetto a [[104_Determinante_con_il_MEG_Esempio_con_Scambio_di_Righe]] qui **non serve lo scambio di righe**, quindi non c'è il segno $(-1)^s$ da tenere sotto controllo: si evita l'errore di segno più comune.
> - Per la scelta di righe/colonne con molti zeri vedi l'obiettivo in [[65_Determinante_Sviluppo_di_Laplace]].

## Note collegate
- [[103_Esercizio_5_1_Calcolo_del_Determinante]]
- [[65_Determinante_Sviluppo_di_Laplace]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[107_Confronto_Metodi_Calcolo_Determinante]]
- [[00_MOC_GAL]]

#GAL/determinante/determinante-metodo-misto-meg-e-laplace
