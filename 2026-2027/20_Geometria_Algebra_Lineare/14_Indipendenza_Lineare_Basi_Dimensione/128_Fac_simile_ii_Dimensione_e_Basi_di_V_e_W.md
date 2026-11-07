---
tags: [GAL, esercizio, fac-simile, dimensione, base, MEG, lezione-15]
data: 2026-10-28
lezione: esercizi
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (fac-simile, svolgimento pag. 2-3)"
---

# Fac-simile, punto (ii): dimensione e basi di $V$ e $W$

Testo: [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]]. Si usa la descrizione esplicita di $V$ vista in [[127_Fac_simile_i_V_e_un_Sottospazio_Due_Strategie]].

## Base e dimensione di $V$
Risolvo il sistema lineare che descrive le relazioni tra le entrate della matrice $A=\begin{bmatrix}a&b\\c&d\end{bmatrix}\in V$ (incognite nell'ordine $a,b,c,d$):
$$\left[\begin{array}{cccc|c}1&0&2&0&0\\0&1&0&2&0\\3&0&6&0&0\\0&3&0&6&0\end{array}\right]\xrightarrow[\ \mathrm{IV}-3\mathrm{II}\to\mathrm{IV}\ ]{\ \mathrm{III}-3\mathrm{I}\to\mathrm{III}\ }\left[\begin{array}{cccc|c}1&0&2&0&0\\0&1&0&2&0\\0&0&0&0&0\\0&0&0&0&0\end{array}\right]$$
Le variabili libere sono $c$ e $d$: aggiungo le righe $c=t_1$, $d=t_2$ (come in [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]]):
$$\left[\begin{array}{cccc|c}1&0&2&0&0\\0&1&0&2&0\\0&0&1&0&t_1\\0&0&0&1&t_2\end{array}\right]\xrightarrow[\ \mathrm{II}-2\mathrm{IV}\to\mathrm{II}\ ]{\ \mathrm{I}-2\mathrm{III}\to\mathrm{I}\ }\left[\begin{array}{cccc|c}1&0&0&0&-2t_1\\0&1&0&0&-2t_2\\0&0&1&0&t_1\\0&0&0&1&t_2\end{array}\right]$$
$$\begin{cases}a=-2t_1\\b=-2t_2\\c=t_1\\d=t_2\end{cases}\qquad\begin{bmatrix}a&b\\c&d\end{bmatrix}=\begin{bmatrix}-2t_1&-2t_2\\t_1&t_2\end{bmatrix}=t_1\begin{bmatrix}-2&0\\1&0\end{bmatrix}+t_2\begin{bmatrix}0&-2\\0&1\end{bmatrix}$$
$$\Rightarrow\ V=\operatorname{Span}\left(\begin{bmatrix}-2&0\\1&0\end{bmatrix},\begin{bmatrix}0&-2\\0&1\end{bmatrix}\right)$$
$$\boxed{\dim V=2\qquad\text{base di }V:\ \left\{\begin{bmatrix}-2&0\\1&0\end{bmatrix},\begin{bmatrix}0&-2\\0&1\end{bmatrix}\right\}}$$
(I due generatori sono indipendenti perché hanno entrate $(c,d)=(1,0)$ e $(0,1)$.)

## Generatori di $W$
$$BE_{11}=\begin{bmatrix}1&2\\3&6\end{bmatrix}\begin{bmatrix}1&0\\0&0\end{bmatrix}=\begin{bmatrix}1&0\\3&0\end{bmatrix}\qquad BE_{12}=\begin{bmatrix}1&2\\3&6\end{bmatrix}\begin{bmatrix}0&1\\0&0\end{bmatrix}=\begin{bmatrix}0&1\\0&3\end{bmatrix}$$
$$BE_{21}=\begin{bmatrix}1&2\\3&6\end{bmatrix}\begin{bmatrix}0&0\\1&0\end{bmatrix}=\begin{bmatrix}2&0\\6&0\end{bmatrix}\qquad BE_{22}=\begin{bmatrix}1&2\\3&6\end{bmatrix}\begin{bmatrix}0&0\\0&1\end{bmatrix}=\begin{bmatrix}0&2\\0&6\end{bmatrix}$$
$$W=\operatorname{Span}\left(\begin{bmatrix}1&0\\3&0\end{bmatrix},\begin{bmatrix}0&1\\0&3\end{bmatrix},\begin{bmatrix}2&0\\6&0\end{bmatrix},\begin{bmatrix}0&2\\0&6\end{bmatrix}\right)$$
Poiché $\begin{bmatrix}2&0\\6&0\end{bmatrix}=2\begin{bmatrix}1&0\\3&0\end{bmatrix}$ e $\begin{bmatrix}0&2\\0&6\end{bmatrix}=2\begin{bmatrix}0&1\\0&3\end{bmatrix}$ (vettori ridondanti, [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]]):
$$W=\operatorname{Span}\left(\begin{bmatrix}1&0\\3&0\end{bmatrix},\begin{bmatrix}0&1\\0&3\end{bmatrix}\right)$$
$$\boxed{\dim W=2\qquad\text{base di }W:\ \left\{\begin{bmatrix}1&0\\3&0\end{bmatrix},\begin{bmatrix}0&1\\0&3\end{bmatrix}\right\}}$$

> [!note] Osservazione (non presente negli appunti)
> L'indipendenza dei due generatori rimasti di $W$ è evidente: hanno entrate $(1,1)$ e $(1,2)$ pari a $(1,0)$ e $(0,1)$ rispettivamente. Il metodo usato è quello dell'estrazione per eliminazione dei vettori ridondanti ([[122_Estrazione_e_Completamento_Due_Problemi_Classici]]).

## Note collegate
- [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]]
- [[127_Fac_simile_i_V_e_un_Sottospazio_Due_Strategie]]
- [[121_Basi_Canoniche]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- Successiva: [[129_Fac_simile_iii_Identita_come_Somma_di_un_Elemento_di_V_e_di_W]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/esercizi/fac-simile-28-10
