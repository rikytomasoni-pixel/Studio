---
tags: [GAL, rango, spazio-delle-righe, spazio-delle-colonne, definizione, esempio, lezione-16]
data: 2026-11-04
lezione: 16
fonte: "GAL 2026-2027 - 20261104 - LEZIONE 16.pdf (slide 135-137)"
---

# Spazio delle righe e spazio delle colonne

> [!abstract] Definizione 16.1
> Data una matrice $A\in M_{\mathbb{K}}(m,n)$, chiamiamo
> - **spazio delle righe** di $A$ il sottospazio vettoriale
> $$\operatorname{row}(A)=\operatorname{Span}\big(R_1(A),\dots,R_m(A)\big)\subseteq\mathbb{K}^n=M_{\mathbb{K}}(1,n)$$
> - **spazio delle colonne** di $A$ il sottospazio vettoriale
> $$\operatorname{col}(A)=\operatorname{Span}\big(C_1(A),\dots,C_n(A)\big)\subseteq\mathbb{K}^m=M_{\mathbb{K}}(m,1)$$

Per quanto visto, $r(A)=\dim\operatorname{row}(A)$ ([[130_Riepilogo_sulle_Definizioni_di_Rango]]).

## Quanto vale $\dim\operatorname{col}(A)$?
$\operatorname{col}(A)=\operatorname{Span}\big(C_1(A),\dots,C_n(A)\big)$ ha $n$ generatori.

**D.** Quanti generatori possiamo scartare?

Una combinazione lineare
$$\lambda_1C_1(A)+\dots+\lambda_nC_n(A)=\underline{0}\qquad\text{(oppure rappresentazione del I tipo)}$$
vale se e solo se $(\lambda_1,\dots,\lambda_n)$ è soluzione di $A\underline{x}=\underline{0}$ (oppure rappresentazione del II tipo).

> [!note] N.B.
> Ogni colonna corrispondente ad una variabile **indipendente** (libera) può essere espressa come combinazione lineare delle colonne corrispondenti alle variabili **dipendenti** (quelle con pivot).

**R.** Scarto tanti generatori quante sono le variabili indipendenti, cioè quanti sono i parametri liberi: $n-r(A)$. Quindi
$$\dim\operatorname{col}(A)=n-\big(n-r(A)\big)=r(A)\qquad\Longrightarrow\qquad r(A)=\dim\operatorname{col}(A)$$

> [!note] Osservazione (non presente negli appunti)
> Insieme a $r(A)=\dim\operatorname{row}(A)$ questo dice che $\dim\operatorname{row}(A)=\dim\operatorname{col}(A)$, cioè $r(A)=r(A^T)$: il rango per righe e il rango per colonne coincidono. Il numero di parametri liberi $n-r(A)$ è la dimensione di $\ker A$ ([[84_Nucleo_e_Sistema_Omogeneo_Associato]]).

## Esempio
$$A=\begin{bmatrix}1&-2&0&1\\0&1&1&-1\\0&0&1&2\end{bmatrix}\qquad\ker(A)=\operatorname{Span}\left(\begin{bmatrix}5\\3\\-2\\1\end{bmatrix}\right)$$
(pivot nelle prime tre colonne). Dal nucleo:
$$5\begin{bmatrix}1\\0\\0\end{bmatrix}+3\begin{bmatrix}-2\\1\\0\end{bmatrix}+(-2)\begin{bmatrix}0\\1\\1\end{bmatrix}+1\begin{bmatrix}1\\-1\\2\end{bmatrix}=\begin{bmatrix}0\\0\\0\end{bmatrix}
\ \Rightarrow\ 
\begin{bmatrix}1\\-1\\2\end{bmatrix}=-5\begin{bmatrix}1\\0\\0\end{bmatrix}-3\begin{bmatrix}-2\\1\\0\end{bmatrix}+2\begin{bmatrix}0\\1\\1\end{bmatrix}$$
Scrivo $A$ come somma di quattro matrici, una per colonna, e come somma di prodotti colonna·riga con $\underline{e}_1,\dots,\underline{e}_4$ (righe della base canonica):
$$A=C_1\,[1\ 0\ 0\ 0]+C_2\,[0\ 1\ 0\ 0]+C_3\,[0\ 0\ 1\ 0]+C_4\,[0\ 0\ 0\ 1]$$
Sostituendo $C_4=-5C_1-3C_2+2C_3$:
$$A=\begin{bmatrix}1\\0\\0\end{bmatrix}\big([1\,0\,0\,0]-5[0\,0\,0\,1]\big)+\begin{bmatrix}-2\\1\\0\end{bmatrix}\big([0\,1\,0\,0]-3[0\,0\,0\,1]\big)+\begin{bmatrix}0\\1\\1\end{bmatrix}\big([0\,0\,1\,0]+2[0\,0\,0\,1]\big)$$
Si ottiene così $A$ come somma di $r(A)=3$ prodotti colonna·riga con colonne indipendenti e righe indipendenti ([[130_Riepilogo_sulle_Definizioni_di_Rango]], punto 5).

> [!warning] DISEGNO NON RAPPRESENTABILE
> GAL L16 slide 136: nella matrice $A$ i tre pivot (in posizione (1,1), (2,2), (3,3)) sono cerchiati in azzurro.

## Note collegate
- [[130_Riepilogo_sulle_Definizioni_di_Rango]]
- [[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[85_Teorema_di_Struttura_delle_Soluzioni]]
- [[96_Insieme_di_Generatori]]
- [[111_EE1_Somma_di_Tre_Matrici_di_Rango_1]]
- Indice: [[17_Indice_Lezione_16]] · [[00_MOC_GAL]]

#GAL/rango/spazio-righe-colonne
