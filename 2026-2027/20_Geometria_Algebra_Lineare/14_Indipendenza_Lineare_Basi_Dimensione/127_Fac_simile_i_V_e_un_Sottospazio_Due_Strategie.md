---
tags: [GAL, esercizio, fac-simile, sottospazi, dimostrazione, lezione-15]
data: 2026-10-28
lezione: esercizi
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (fac-simile, svolgimento pag. 2)"
---

# Fac-simile, punto (i): $V$ è un sottospazio vettoriale

Testo: [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]].
$$V=\left\{A\in M_{\mathbb{R}}(2,2)\ \middle|\ BA=\begin{bmatrix}0&0\\0&0\end{bmatrix}\right\},\qquad B=\begin{bmatrix}1&2\\3&6\end{bmatrix}$$

## Strategia 1: uso la definizione di sottospazio vettoriale
(Definizione in [[94_Sottospazi_Vettoriali]].)

- **Chiusura nella somma:** $\forall A_1,A_2\in V$ (cioè $BA_1=\underline{0}$, $BA_2=\underline{0}$)
$$B(A_1+A_2)=BA_1+BA_2=\underline{0}+\underline{0}=\underline{0}\iff A_1+A_2\in V$$
- **Chiusura nel prodotto per scalari:** $\forall A\in V$ (cioè $BA=\underline{0}$), $\forall\lambda\in\mathbb{R}$
$$B(\lambda A)=\lambda(BA)=\lambda\underline{0}=\underline{0}\ \Rightarrow\ \lambda A\in V$$

## Strategia 2: descrizione esplicita di $V$
Esplicito la descrizione di $V$ in modo da riconoscerlo come insieme delle soluzioni di un sistema omogeneo:
$$V=\left\{\begin{bmatrix}a&b\\c&d\end{bmatrix}\in M_{\mathbb{R}}(2,2)\ \middle|\ B\begin{bmatrix}a&b\\c&d\end{bmatrix}=\underline{0}\right\}$$
$$B\begin{bmatrix}a&b\\c&d\end{bmatrix}=\begin{bmatrix}1&2\\3&6\end{bmatrix}\begin{bmatrix}a&b\\c&d\end{bmatrix}=\begin{bmatrix}a+2c&b+2d\\3a+6c&3b+6d\end{bmatrix}=\begin{bmatrix}0&0\\0&0\end{bmatrix}$$
$$V=\left\{\begin{bmatrix}a&b\\c&d\end{bmatrix}\in M_{\mathbb{R}}(2,2)\ \middle|\ \begin{cases}a+2c=0\\ b+2d=0\\ 3a+6c=0\\ 3b+6d=0\end{cases}\right\}$$
Gli elementi di $V$ sono soluzioni di un **sistema omogeneo** (chiuse rispetto a somma e prodotto per scalari, vedi [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]), quindi $V$ è un sottospazio vettoriale.

> [!warning] Da controllare sul quaderno
> Nella frase iniziale della Strategia 2 la parola subito prima di «delle soluzioni di un sistema omogeneo» è di lettura incerta (letta «riconoscerlo come insieme»). Il senso è comunque chiaro dal seguito.

> [!note] Osservazione (non presente negli appunti)
> Le quattro equazioni si riducono a due indipendenti ($a+2c=0$ e $b+2d=0$; le altre due sono 3 volte le prime): è ciò che si vede in [[128_Fac_simile_ii_Dimensione_e_Basi_di_V_e_W]] con il MEG.

## Note collegate
- [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]]
- [[94_Sottospazi_Vettoriali]]
- [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- Successiva: [[128_Fac_simile_ii_Dimensione_e_Basi_di_V_e_W]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/esercizi/fac-simile-28-10
