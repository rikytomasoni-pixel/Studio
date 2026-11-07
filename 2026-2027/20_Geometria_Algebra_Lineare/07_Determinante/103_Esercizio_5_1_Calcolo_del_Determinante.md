---
tags: [GAL, determinante, esercizio, MEG, laplace]
data: 2026-10-09
lezione: esercizi
fonte: "esempideterminante.pdf (pag. 1) — Esercizio 5.1, appunti del 9 ottobre 2026"
---

# Esercizio 5.1: calcolo del determinante

> [!question] Testo (Esercizio 5.1)
> Calcolare il determinante delle matrici seguenti riducendole a forma triangolare mediante mosse di Gauss.
> $$A=\begin{bmatrix}1&2&3\\2&4&1\\3&1&2\end{bmatrix},\qquad B=\begin{bmatrix}2&0&2&1\\1&3&2&1\\0&2&3&1\\3&1&2&1\end{bmatrix},\qquad C=\begin{bmatrix}4&0&0&1&1\\1&1&2&0&1\\0&2&1&1&0\\1&1&0&1&0\\1&1&0&0&1\end{bmatrix}$$

## Cosa è svolto negli appunti
Negli appunti è svolta **solo la matrice $A$** (punto 1), e viene calcolata in tre modi diversi: tutti danno $\det(A)=-25$.

| Metodo | Nota | Risultato |
|---|---|---|
| Riduzione di Gauss (MEG) + prodotto dei pivot | [[104_Determinante_con_il_MEG_Esempio_con_Scambio_di_Righe]] | $-25$ |
| Sviluppo di Laplace lungo la riga 3 | [[105_Determinante_Laplace_Esempio_3x3_Riga_3]] | $-25$ |
| Metodo misto: MEG parziale + Laplace sulla colonna 1 | [[106_Determinante_Metodo_Misto_MEG_e_Laplace]] | $-25$ |

Confronto e osservazioni: [[107_Confronto_Metodi_Calcolo_Determinante]].

> [!note] Osservazione
> Poiché $\det(A)=-25\neq0$, per il [[88_Teorema_sull_Invertibilita_della_Matrice]] la matrice $A$ è invertibile e ha rango $3$.

## Note collegate
- [[65_Determinante_Sviluppo_di_Laplace]]
- [[66_Matrici_Triangolari]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[75_Calcolo_del_Determinante_con_il_MEG]]
- [[107_Confronto_Metodi_Calcolo_Determinante]]
- [[00_MOC_GAL]]

#GAL/determinante/esercizio-5-1-calcolo-del-determinante
