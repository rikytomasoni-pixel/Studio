---
tags: [GAL, esercizio, rango, prodotto-matriciale, colonna-per-riga]
data: 2026-10-09
lezione: esercizi
fonte: "esempio.pdf (pag. 1) — EE1, somma di matrici di rango 1"
---

# EE1: $A$ come somma di tre matrici di rango 1

Da $A=(PL)\,U$ ([[110_EE1_Fattorizzazione_con_Matrici_Elementari]]) si scrive il prodotto come somma di prodotti **colonna per riga**: colonna $i$ di $PL$ per riga $i$ di $U$. La quarta riga di $U$ è nulla, quindi gli addendi sono $3$.

$$A=\begin{bmatrix}0&2&1&0\\1&0&0&0\\2&1&0&0\\1&2&-3&1\end{bmatrix}\begin{bmatrix}1&1&1\\0&1&-1\\0&0&-1\\0&0&0\end{bmatrix}$$

$$A=\underbrace{\begin{bmatrix}0\\1\\2\\1\end{bmatrix}\begin{bmatrix}1&1&1\end{bmatrix}}_{\begin{bmatrix}0&0&0\\1&1&1\\2&2&2\\1&1&1\end{bmatrix}}+\underbrace{\begin{bmatrix}2\\0\\1\\2\end{bmatrix}\begin{bmatrix}0&1&-1\end{bmatrix}}_{\begin{bmatrix}0&2&-2\\0&0&0\\0&1&-1\\0&2&-2\end{bmatrix}}+\underbrace{\begin{bmatrix}1\\0\\0\\-3\end{bmatrix}\begin{bmatrix}0&0&-1\end{bmatrix}}_{\begin{bmatrix}0&0&-1\\0&0&0\\0&0&0\\0&0&3\end{bmatrix}}$$

> [!warning] Differenza rispetto al quaderno
> Nel quaderno la terza colonna di $PL$ ha $-1$ in ultima posizione e l'ultimo addendo ha $+1$ in posizione $(4,3)$. Con il valore corretto $-3$ l'addendo è $+3$ in quella posizione.

> [!tip] Verifica
> Sommando i tre addendi si ottiene
> $$\begin{bmatrix}0&2&-3\\1&1&1\\2&3&1\\1&3&2\end{bmatrix}=A$$
> (la riga $4$: $(1,1,1)+(0,2,-2)+(0,0,3)=(1,3,2)$). Con $+1$ invece di $+3$ la riga $4$ verrebbe $(1,3,0)$, sbagliata.

## Perché $r=3$ è il minimo
Ogni addendo è una matrice di rango $1$ (colonna per riga non nulle). Per la [[63_Rango_di_una_Matrice]], $r(A)$ è il **minimo** numero di addendi di questo tipo, e per [[73_MEG_e_Rango]] $r(A)=r(U)=3$. Quindi la scomposizione trovata è la più corta possibile.

> [!note] Osservazione (non presente negli appunti)
> In generale, se $A=PLU$ con $U$ a scala di rango $r$, le prime $r$ colonne di $PL$ e le $r$ righe non nulle di $U$ danno $A=\sum_{i=1}^{r}C_iR_i$: è lo stesso schema dell'esempio $\begin{bmatrix}1&1\\1&1\end{bmatrix}$ in [[73_MEG_e_Rango]], dove la matrice $\begin{bmatrix}1&0\\1&1\end{bmatrix}$ moltiplica la colonna $\begin{bmatrix}1\\0\end{bmatrix}$.

## Note collegate
- [[108_Esercizio_EE1_Somma_di_Matrici_di_Rango_1]]
- [[110_EE1_Fattorizzazione_con_Matrici_Elementari]]
- [[63_Rango_di_una_Matrice]]
- [[73_MEG_e_Rango]]
- [[00_MOC_GAL]]

#GAL/rango/ee1-somma-di-tre-matrici-di-rango-1
