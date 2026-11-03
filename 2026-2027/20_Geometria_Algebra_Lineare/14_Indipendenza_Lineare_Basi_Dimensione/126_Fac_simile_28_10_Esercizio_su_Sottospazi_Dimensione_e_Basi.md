---
tags: [GAL, esercizio, fac-simile, sottospazi, dimensione, base, lezione-15]
data: 2026-10-28
lezione: esercizi
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (fac-simile, pag. 12-15 del PDF)"
---

# Fac-simile del 28-10-2026: sottospazi, dimensione e basi

Fac-simile di prova scritta (Scuola di Ingegneria Industriale e dell'Informazione, GAL A.A. 2026-2027) allegato alla Lezione 15, con svolgimento a mano.

> [!question] Esercizio
> Nello spazio vettoriale $M_{\mathbb{R}}(2,2)$ dotato della base canonica
> $$\left\{E_{11}=\begin{bmatrix}1&0\\0&0\end{bmatrix},\ E_{12}=\begin{bmatrix}0&1\\0&0\end{bmatrix},\ E_{21}=\begin{bmatrix}0&0\\1&0\end{bmatrix},\ E_{22}=\begin{bmatrix}0&0\\0&1\end{bmatrix}\right\}$$
> considera la matrice $B=\begin{bmatrix}1&2\\3&6\end{bmatrix}$.
>
> **(i)** Dimostra che il sottoinsieme
> $$V=\left\{A\in M_{\mathbb{R}}(2,2)\ \middle|\ BA=\begin{bmatrix}0&0\\0&0\end{bmatrix}\right\}$$
> è un sottospazio vettoriale di $M_{\mathbb{R}}(2,2)$.
>
> **(ii)** Determina dimensione e basi per gli spazi vettoriali $V$ e $W=\operatorname{Span}(BE_{11},BE_{12},BE_{21},BE_{22})$.
>
> **(iii)** È possibile ottenere la matrice identità $\mathrm{Id}_2$ come somma di una matrice appartenente a $V$ e di una matrice appartenente a $W$? In caso affermativo, esibire $A_1\in V$ e $A_2\in W$ tali che $A_1+A_2=\mathrm{Id}_2$.

## Risultati

| Punto | Risultato | Nota |
|---|---|---|
| (i) | $V$ è sottospazio (due strategie: definizione, oppure insieme delle soluzioni di un sistema omogeneo) | [[127_Fac_simile_i_V_e_un_Sottospazio_Due_Strategie]] |
| (ii) | $\dim V=2$, base $\left\{\begin{bmatrix}-2&0\\1&0\end{bmatrix},\begin{bmatrix}0&-2\\0&1\end{bmatrix}\right\}$; $\dim W=2$, base $\left\{\begin{bmatrix}1&0\\3&0\end{bmatrix},\begin{bmatrix}0&1\\0&3\end{bmatrix}\right\}$ | [[128_Fac_simile_ii_Dimensione_e_Basi_di_V_e_W]] |
| (iii) | Sì: $A_1=-\tfrac37\begin{bmatrix}-2&0\\1&0\end{bmatrix}+\tfrac17\begin{bmatrix}0&-2\\0&1\end{bmatrix}\in V$, $A_2=\tfrac17\begin{bmatrix}1&0\\3&0\end{bmatrix}+\tfrac27\begin{bmatrix}0&1\\0&3\end{bmatrix}\in W$ | [[129_Fac_simile_iii_Identita_come_Somma_di_un_Elemento_di_V_e_di_W]] |

## Note collegate
- [[94_Sottospazi_Vettoriali]]
- [[121_Basi_Canoniche]]
- [[102_Dimensione_di_uno_Spazio_Vettoriale]]
- [[125_Completamento_ad_una_Base]] (lezione precedente nel PDF)
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/esercizi/fac-simile-28-10
