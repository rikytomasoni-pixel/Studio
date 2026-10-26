---
tags: [GAL, esercizio, rango, MEG, scambio-di-righe, pivot]
data: 2026-10-09
lezione: esercizi
fonte: "esempio.pdf (pag. 1) — EE1, riduzione di A"
---

# EE1: riduzione a scala di $A$ con il MEG

Si riduce $A$ ([[108_Esercizio_EE1_Somma_di_Matrici_di_Rango_1]]) con il [[68_Metodo_di_Eliminazione_di_Gauss]]. Poiché $a_{11}=0$, il primo passo è uno scambio di righe per portare in alto il pivot $1$ (cerchiato negli appunti).

$$A=\begin{bmatrix}0&2&-3\\1&1&1\\2&3&1\\1&3&2\end{bmatrix}\xrightarrow{\ \mathrm{I}\leftrightarrow\mathrm{II}\ }\begin{bmatrix}1&1&1\\0&2&-3\\2&3&1\\1&3&2\end{bmatrix}\xrightarrow{\ \mathrm{III}-2\mathrm{I}\to\mathrm{III},\ \ \mathrm{IV}-\mathrm{I}\to\mathrm{IV}\ }\begin{bmatrix}1&1&1\\0&2&-3\\0&1&-1\\0&2&1\end{bmatrix}$$

Il secondo pivot è cerchiato sul $1$ in posizione $(3,2)$: serve un secondo scambio.

$$\xrightarrow{\ \mathrm{II}\leftrightarrow\mathrm{III}\ }\begin{bmatrix}1&1&1\\0&1&-1\\0&2&-3\\0&2&1\end{bmatrix}\xrightarrow{\ \mathrm{III}-2\mathrm{II}\to\mathrm{III},\ \ \mathrm{IV}-2\mathrm{II}\to\mathrm{IV}\ }\begin{bmatrix}1&1&1\\0&1&-1\\0&0&-1\\0&0&3\end{bmatrix}\xrightarrow{\ \mathrm{IV}+3\,\mathrm{III}\to\mathrm{IV}\ }\begin{bmatrix}1&1&1\\0&1&-1\\0&0&-1\\0&0&0\end{bmatrix}=U$$

I pivot (cerchiati) sono $1,\ 1,\ -1$ ([[69_Pivot_e_Matrice_a_Scala]]).

> [!warning] Differenza rispetto al quaderno
> Nel quaderno la matrice prima dell'ultimo passo ha l'elemento $(4,3)$ scritto come $-1$ (e di conseguenza l'ultima operazione è $\mathrm{IV}-\mathrm{III}$). Il calcolo corretto è $1-2\cdot(-1)=3$, da cui $\mathrm{IV}+3\,\mathrm{III}\to\mathrm{IV}$. Tutte le note EE1 usano il valore corretto $3$. **Da controllare sul quaderno.**

## Conclusione sul rango
$U$ ha $3$ righe non nulle, cioè $3$ pivot, quindi per [[73_MEG_e_Rango]]
$$r(A)=r(U)=3.$$

> [!note] Osservazione (non presente negli appunti)
> Si sono usati $s=2$ scambi di righe e solo operazioni di sostituzione. Il rango non cambia perché il MEG è reversibile ([[70_Reversibilita_del_MEG]]).

## Note collegate
- [[108_Esercizio_EE1_Somma_di_Matrici_di_Rango_1]]
- [[110_EE1_Fattorizzazione_con_Matrici_Elementari]]
- [[67_Operazioni_Elementari_sulle_Righe]]
- [[73_MEG_e_Rango]]
- [[00_MOC_GAL]]

#GAL/rango/ee1-riduzione-a-scala-di-a
