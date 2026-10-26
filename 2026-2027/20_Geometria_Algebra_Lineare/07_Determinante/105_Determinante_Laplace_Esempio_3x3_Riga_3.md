---
tags: [GAL, determinante, esercizio, laplace, cofattori]
data: 2026-10-09
lezione: esercizi
fonte: "esempideterminante.pdf (pag. 1) — Esercizio 5.1, matrice A"
---

# Determinante: Laplace sulla riga 3 (esempio $3\times3$)

Calcolo di $\det(A)$, $A=\begin{bmatrix}1&2&3\\2&4&1\\3&1&2\end{bmatrix}$, con lo [[65_Determinante_Sviluppo_di_Laplace]] lungo la riga $i=3$ (elementi $3,\,1,\,2$):
$$\det(A)=3\,C_{31}+1\,C_{32}+2\,C_{33}$$
dove $C_{ij}=(-1)^{i+j}\det(\hat A_{ij})$ è il cofattore.

## Svolgimento
$$\det(A)=3\cdot(-1)^{3+1}\begin{vmatrix}2&3\\4&1\end{vmatrix}+1\cdot(-1)^{3+2}\begin{vmatrix}1&3\\2&1\end{vmatrix}+2\cdot(-1)^{3+3}\begin{vmatrix}1&2\\2&4\end{vmatrix}$$
$$=3\cdot1\cdot(-10)+1\cdot(-1)\cdot(-5)+2\cdot1\cdot0=-30+5+0=-25$$

I minori $2\times2$ si calcolano con [[28_Determinanti_2x2_e_3x3]]:
- $\begin{vmatrix}2&3\\4&1\end{vmatrix}=2\cdot1-3\cdot4=-10$
- $\begin{vmatrix}1&3\\2&1\end{vmatrix}=1\cdot1-3\cdot2=-5$
- $\begin{vmatrix}1&2\\2&4\end{vmatrix}=1\cdot4-2\cdot2=0$

> [!note] Osservazione
> $A$ non ha zeri: nessuna riga o colonna è più conveniente delle altre (vedi l'«obiettivo» di scegliere la riga con più zeri in [[65_Determinante_Sviluppo_di_Laplace]]). Qui il caso è fortunato perché $C_{33}=0$ elimina un addendo, ma i conti restano $3$ determinanti $2\times2$.
> I segni $(-1)^{i+j}$ seguono la scacchiera $\begin{bmatrix}+&-&+\\-&+&-\\+&-&+\end{bmatrix}$: sulla riga 3 sono $+,-,+$.

## Note collegate
- [[103_Esercizio_5_1_Calcolo_del_Determinante]]
- [[65_Determinante_Sviluppo_di_Laplace]]
- [[104_Determinante_con_il_MEG_Esempio_con_Scambio_di_Righe]] (stesso risultato col MEG)
- [[107_Confronto_Metodi_Calcolo_Determinante]]
- [[00_MOC_GAL]]

#GAL/determinante/determinante-laplace-esempio-3x3-riga-3
