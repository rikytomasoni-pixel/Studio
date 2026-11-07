---
tags: [GAL, base, estrazione, MEG, righe, esempio, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 126-127)"
---

# Base per costruzione libera: MEG sulle righe

## Esempio (I): $V\subseteq\mathbb{R}^3$
$$V=\operatorname{Span}\left(\begin{bmatrix}1\\-1\\0\end{bmatrix},\begin{bmatrix}0\\1\\2\end{bmatrix},\begin{bmatrix}1\\0\\2\end{bmatrix}\right)$$
Scrivo i vettori come **righe** di una matrice $A$ e applico il [[68_Metodo_di_Eliminazione_di_Gauss|MEG]]:
$$A=\begin{bmatrix}1&-1&0\\0&1&2\\1&0&2\end{bmatrix}\xrightarrow{\ \mathrm{III}-\mathrm{I}\to\mathrm{III}\ }B=\begin{bmatrix}1&-1&0\\0&1&2\\0&1&2\end{bmatrix}\xrightarrow{\ \mathrm{III}-\mathrm{II}\to\mathrm{III}\ }C=\begin{bmatrix}1&-1&0\\0&1&2\\0&0&0\end{bmatrix}$$
con $R_3(B)=R_3(A)-R_1(A)$, $R_2(B)=R_2(A)$, $R_1(B)=R_1(A)$ e $R_3(C)=R_3(B)-R_2(B)$, $R_2(C)=R_2(B)$, $R_1(C)=R_1(B)$.

## Proprietà
> [!tip] Righe e MEG
> - Se $A\overset{\text{MEG}}{\leadsto}U$ allora
> $$\operatorname{Span}(R_1(A),\dots,R_m(A))=\operatorname{Span}(R_1(U),\dots,R_m(U))$$
> Nell'esempio:
> $$\operatorname{Span}\left(\begin{bmatrix}1\\-1\\0\end{bmatrix},\begin{bmatrix}0\\1\\2\end{bmatrix},\begin{bmatrix}1\\0\\2\end{bmatrix}\right)=\operatorname{Span}\left(\begin{bmatrix}1\\-1\\0\end{bmatrix},\begin{bmatrix}0\\1\\2\end{bmatrix},\begin{bmatrix}0\\0\\0\end{bmatrix}\right)$$
> (il vettore nullo si scarta).
> - Le righe non nulle di una matrice **a scala** sono linearmente indipendenti ([[69_Pivot_e_Matrice_a_Scala]]).

Quindi una base di $V$ è $\left\{\begin{bmatrix}1\\-1\\0\end{bmatrix},\begin{bmatrix}0\\1\\2\end{bmatrix}\right\}$ e $\dim V=2$.

> [!warning] N.B.
> Durante il MEG i vettori cambiano **non solo nei numeri, ma anche nelle posizioni** (scambi di righe)! Se voglio **conservare i vettori iniziali**, questo non è l'approccio migliore: vedi [[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]].

## Esempio (II): costruzione libera per $W$
$$W=\operatorname{Span}\left(\begin{bmatrix}0\\2\\1\end{bmatrix},\begin{bmatrix}4\\1\\2\end{bmatrix},\begin{bmatrix}4\\-3\\0\end{bmatrix}\right)$$
Vettori come righe:
$$\begin{bmatrix}0&2&1\\4&1&2\\4&-3&0\end{bmatrix}\xrightarrow{\ \mathrm{I}\leftrightarrow\mathrm{II}\ }\begin{bmatrix}4&1&2\\0&2&1\\4&-3&0\end{bmatrix}\xrightarrow{\ \mathrm{III}-\mathrm{I}\to\mathrm{III}\ }\begin{bmatrix}4&1&2\\0&2&1\\0&-4&-2\end{bmatrix}\xrightarrow{\ \mathrm{III}+2\mathrm{II}\to\mathrm{III}\ }\begin{bmatrix}4&1&2\\0&2&1\\0&0&0\end{bmatrix}$$
Base ottenuta (costruzione libera): $\left\{\begin{bmatrix}4\\1\\2\end{bmatrix},\begin{bmatrix}0\\2\\1\end{bmatrix}\right\}$, $\dim W=2$. Con l'estrazione si ottiene invece una base formata da vettori dati: [[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]].

> [!note] Osservazione (non presente negli appunti)
> La base trovata ha $\dim V=2<3$ elementi: il rango della matrice $A$ è $2$ ([[73_MEG_e_Rango]]). In generale la dimensione dello span delle righe di $A$ è $r(A)$.

## Note collegate
- [[122_Estrazione_e_Completamento_Due_Problemi_Classici]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[73_MEG_e_Rango]]
- [[69_Pivot_e_Matrice_a_Scala]]
- Successiva: [[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/base/costruzione-libera
