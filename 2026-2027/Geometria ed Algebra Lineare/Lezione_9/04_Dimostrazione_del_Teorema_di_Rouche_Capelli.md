---
tags: [GAL, sistemi-lineari, dimostrazione, rouche-capelli, MEG, lezione-9]
data: 2026-10-12
lezione: 9
fonte: "GAL 2026-2027 - 20261012 - LEZIONE 9.pdf (slide 78-81)"
---

# Dimostrazione del teorema di Rouché-Capelli

Enunciato: [[03_Teorema_di_Rouche_Capelli]].

## Tesi 1

$A\underline{x}=\underline{b}$ risolubile $\iff r(A)=r(A\,|\,\underline{b})$ è equivalente a dimostrare due casi:

- $A\underline{x}=\underline{b}$ risolubile $\Rightarrow$ $r(A)=r(A\,|\,\underline{b})$; equivalentemente $A\underline{x}=\underline{b}$ **non** risolubile $\Leftarrow$ $r(A)\neq r(A\,|\,\underline{b})$ (le slide scrivono questa seconda forma accanto alla prima);
- $r(A)=r(A\,|\,\underline{b})$ $\Rightarrow$ $A\underline{x}=\underline{b}$ risolubile.

Comincio a usare il MEG sulla rappresentazione matriciale del III tipo:
$$[A\,|\,\underline{b}]\ \overset{\text{MEG}}{\leadsto}\ [U\,|\,\underline{b}']$$
Per definizione di rango: $r=r(A)=r(U)=\#\text{pivot di }U$.

Considerando l'ultima colonna ci sono 2 possibilità:

1. **Nessun pivot nell'ultima colonna.** $[U\,|\,\underline{b}']$ ha $r$ righe non nulle in $U$ (pivot $p_1,\dots,p_r\neq0$), le righe successive sono nulle anche nella colonna $\underline{b}'$ (termini noti $b_1',\dots,b_r',0,\dots,0$):
$$r(A)=r(A\,|\,\underline{b})$$

2. **Pivot nell'ultima colonna.** Compare una riga $(0\ \cdots\ 0\,|\,b'_{r+1})$ con $b'_{r+1}\neq0$:
$$r(A\,|\,\underline{b})=r(A)+1\qquad(r(A)\neq r(A\,|\,\underline{b}))$$

Nel caso (2) l'equazione sulla riga $r+1$ dice
$$0=b'_{r+1}\neq0\ \Rightarrow\ A\underline{x}=\underline{b}\ \text{NON risolubile}$$

Resta il caso (1), che porta alla risolubilità.

## Tesi 2 (caso 1: ricerca delle soluzioni)

Nel caso (1) le ultime $m-r$ righe di $[U\,|\,\underline{b}']$ sono nulle (equazioni $0=0$, da eliminare).

**Variabili.** Divido le variabili in due gruppi:
- **variabili dipendenti**: corrispondono alle colonne contenenti i pivot ($r$ variabili);
- **variabili indipendenti**: corrispondono alle colonne non contenenti i pivot ($n-r$ variabili).

Suppongo, per semplicità, che le variabili dipendenti siano le **prime** $r$: la matrice ha $r$ equazioni, $r$ colonne di variabili dipendenti, $n-r$ colonne di variabili indipendenti e la colonna dei termini noti.

**Equazioni fittizie.** Aggiungo $n-r$ equazioni:
$$x_{r+1}=t_1,\ \dots,\ x_n=t_{n-r}\qquad t_i\in\mathbb{K}$$
Il sistema diventa, in forma matriciale: nelle prime $r$ righe la matrice a scala (pivot $p_1,\dots,p_r\neq0$), nelle ultime $n-r$ righe $[\,0\,|\,I_{n-r}\,|\,t\,]$ (zeri sulle colonne delle variabili dipendenti e matrice identità $n-r$ sulle colonne delle indipendenti), con termini noti $b_1',\dots,b_r',t_1,\dots,t_{n-r}$.

A questo punto ho un sistema con $n$ equazioni e $n$ incognite che risolvo per **sostituzione all'indietro**.

- **Step 1.** Si usano le ultime $n-r$ righe per sostituire le variabili indipendenti nelle prime $r$ righe: i termini noti diventano $b_i'+\sum_j c_{ij}t_j$ (i coefficienti delle variabili indipendenti passano a destra) e le variabili dipendenti restano a sinistra con la sola matrice a scala; le ultime righe restano $t_1,\dots,t_{n-r}$.
- **Step 2.** Sostituisco a ritroso anche tra le prime $r$ righe.

**Dove arrivo?** Alla matrice $[\,I_n\,|\,\text{termini noti}\,]$ (identità $n\times n$ a sinistra), con termini noti $v_{0i}+\sum_{j=1}^{n-r}v_{ji}\,t_j$ nelle prime $r$ righe e $t_1,\dots,t_{n-r}$ nelle ultime $n-r$; cioè
$$\begin{bmatrix} x_1\\ \vdots\\ x_n\end{bmatrix}=\begin{bmatrix} v_{01}+\sum_{i=1}^{n-r}v_{i1}t_i\\ \vdots\\ v_{0r}+\sum_{i=1}^{n-r}v_{ir}t_i\\ t_1\\ \vdots\\ t_{n-r}\end{bmatrix}=\underbrace{\begin{bmatrix} v_{01}\\ v_{02}\\ \vdots\\ v_{0r}\\ 0\\ \vdots\\ 0\end{bmatrix}}_{\underline{v}_0\ \text{(parte costante)}}+t_1\underbrace{\begin{bmatrix} v_{11}\\ \vdots\\ v_{1r}\\ 1\\ 0\\ \vdots\\ 0\end{bmatrix}}_{\underline{v}_1}+t_2\underbrace{\begin{bmatrix} v_{21}\\ \vdots\\ v_{2r}\\ 0\\ 1\\ \vdots\\ 0\end{bmatrix}}_{\underline{v}_2}+\cdots+t_{n-r}\underbrace{\begin{bmatrix} v_{n-r,1}\\ \vdots\\ v_{n-r,r}\\ 0\\ \vdots\\ 1\end{bmatrix}}_{\underline{v}_{n-r}}$$
$\blacksquare$

> [!warning] Da verificare sulle slide originali
> Le slide 79-81 contengono matrici disegnate a mano molto fitte; le ho trascritte a parole e con la notazione più semplice possibile. In particolare, nello **Step 1** (slide 80) i termini noti sono scritti nelle slide come "$b_1'+\sum t_i$" e "$b_n'+\sum c_it_i$" (con $c_i$ coefficienti), che qui ho reso come $b_i'+\sum_j c_{ij}t_j$; e i vettori $\underline{v}_0,\dots,\underline{v}_{n-r}$ a slide 81 hanno componenti indicate con $v_{ij}$ (indici letti in modo approssimativo). Il significato non cambia, ma controlla gli indici se li userai in una dimostrazione scritta.

### Note collegate
- [[00_Indice_Lezione_9]] · [[00_MOC_GAL]]
- [[03_Teorema_di_Rouche_Capelli]]
- [[10_Pivot_e_Matrice_a_Scala]] — pivot e rango $r(U)=\#$pivot
- [[04_Rango_di_una_Matrice]]
- [[09_Metodo_di_Eliminazione_di_Gauss]]
