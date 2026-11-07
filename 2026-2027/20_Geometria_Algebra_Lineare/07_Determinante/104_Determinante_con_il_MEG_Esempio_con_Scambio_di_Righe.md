---
tags: [GAL, determinante, esercizio, MEG, triangolari, scambio-di-righe]
data: 2026-10-09
lezione: esercizi
fonte: "esempideterminante.pdf (pag. 1) — Esercizio 5.1, matrice A"
---

# Determinante con il MEG: esempio con scambio di righe

Calcolo di $\det(A)$ per $A=\begin{bmatrix}1&2&3\\2&4&1\\3&1&2\end{bmatrix}$ riducendola a scala ([[68_Metodo_di_Eliminazione_di_Gauss]]) e usando [[75_Calcolo_del_Determinante_con_il_MEG]].

## Riduzione passo passo
Il primo pivot è $1$ (cerchiato negli appunti). Si eliminano gli elementi sotto di lui con operazioni di sostituzione ([[67_Operazioni_Elementari_sulle_Righe]]):
$$\begin{bmatrix}1&2&3\\2&4&1\\3&1&2\end{bmatrix}\xrightarrow{\ \mathrm{II}-2\mathrm{I}\to\mathrm{II},\ \ \mathrm{III}-3\mathrm{I}\to\mathrm{III}\ }\begin{bmatrix}1&2&3\\0&0&-5\\0&-5&-7\end{bmatrix}$$
Nella seconda colonna l'elemento in posizione $(2,2)$ è $0$: il pivot è nella riga $3$, quindi serve uno **scambio di righe** (nel quaderno la freccia è segnata con «!»):
$$\begin{bmatrix}1&2&3\\0&0&-5\\0&-5&-7\end{bmatrix}\xrightarrow{\ \mathrm{II}\leftrightarrow\mathrm{III}\ }\begin{bmatrix}1&2&3\\0&-5&-7\\0&0&-5\end{bmatrix}=U$$
I pivot (cerchiati) sono $u_{11}=1,\ u_{22}=-5,\ u_{33}=-5$ e $U$ è triangolare superiore ([[66_Matrici_Triangolari]]).

## Formula e risultato
$$\det(A)=(-1)^{s}\prod_{i=1}^{3}u_{ii}=(-1)^{1}\cdot\big(1\cdot(-5)\cdot(-5)\big)=(-1)^1\cdot25=-25$$
dove $s$ è il numero di scambi di righe ($s=1$).

> [!note] Osservazione (non presente negli appunti)
> Il fattore $(-1)^s$ viene da:
> - la **sostituzione** $R_i+\lambda R_k\to R_i$ non cambia il determinante ([[78_Determinante_e_Sostituzione]]);
> - lo **scambio** di due righe lo moltiplica per $-1$ ([[76_Determinante_Normalizzato_e_Alternante]]).
>
> In termini della nota [[75_Calcolo_del_Determinante_con_il_MEG]]: $\det(A)=\det(Z)\,u_{11}\cdots u_{nn}$ con $\det(Z)=(-1)^s$ quando si usano solo scambi e sostituzioni (nessuna moltiplicazione di una riga per uno scalare).

> [!tip] Verifica
> Lo stesso valore si ottiene con Laplace: [[105_Determinante_Laplace_Esempio_3x3_Riga_3]].

## Note collegate
- [[103_Esercizio_5_1_Calcolo_del_Determinante]]
- [[75_Calcolo_del_Determinante_con_il_MEG]]
- [[107_Confronto_Metodi_Calcolo_Determinante]]
- [[00_MOC_GAL]]

#GAL/determinante/determinante-con-il-meg-esempio-con-scambio-di-righe
