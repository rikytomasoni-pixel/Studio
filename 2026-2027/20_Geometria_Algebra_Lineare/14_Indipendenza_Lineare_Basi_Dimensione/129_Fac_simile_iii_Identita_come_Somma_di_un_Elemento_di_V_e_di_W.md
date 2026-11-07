---
tags: [GAL, esercizio, fac-simile, sistemi-lineari, MEG, lezione-15]
data: 2026-10-28
lezione: esercizi
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (fac-simile, svolgimento pag. 3-4)"
---

# Fac-simile, punto (iii): $\mathrm{Id}_2=A_1+A_2$ con $A_1\in V$, $A_2\in W$

Testo: [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]]. Basi di $V$ e $W$ da [[128_Fac_simile_ii_Dimensione_e_Basi_di_V_e_W]].

Un elemento di $V$ è una combinazione lineare della sua base, e lo stesso per $W$:
$$A_1\in V\iff A_1=\lambda_1\begin{bmatrix}-2&0\\1&0\end{bmatrix}+\lambda_2\begin{bmatrix}0&-2\\0&1\end{bmatrix}\qquad A_2\in W\iff A_2=\mu_1\begin{bmatrix}1&0\\3&0\end{bmatrix}+\mu_2\begin{bmatrix}0&1\\0&3\end{bmatrix}$$
$$A_1+A_2=\mathrm{Id}_2\iff\begin{bmatrix}-2\lambda_1+\mu_1&-2\lambda_2+\mu_2\\ \lambda_1+3\mu_1&\lambda_2+3\mu_2\end{bmatrix}=\begin{bmatrix}1&0\\0&1\end{bmatrix}$$
$$\iff\begin{cases}-2\lambda_1+\mu_1=1\\-2\lambda_2+\mu_2=0\\ \lambda_1+3\mu_1=0\\ \lambda_2+3\mu_2=1\end{cases}\iff\left[\begin{array}{cccc|c}-2&0&1&0&1\\0&-2&0&1&0\\1&0&3&0&0\\0&1&0&3&1\end{array}\right]$$
(incognite nell'ordine $\lambda_1,\lambda_2,\mu_1,\mu_2$). MEG, con scambio delle righe $\mathrm{I}\to\mathrm{III}$, $\mathrm{II}\to\mathrm{IV}$, $\mathrm{III}\to\mathrm{I}$, $\mathrm{IV}\to\mathrm{II}$:
$$\left[\begin{array}{cccc|c}1&0&3&0&0\\0&1&0&3&1\\-2&0&1&0&1\\0&-2&0&1&0\end{array}\right]\xrightarrow[\ \mathrm{IV}+2\mathrm{II}\to\mathrm{IV}\ ]{\ \mathrm{III}+2\mathrm{I}\to\mathrm{III}\ }\left[\begin{array}{cccc|c}1&0&3&0&0\\0&1&0&3&1\\0&0&7&0&1\\0&0&0&7&2\end{array}\right]$$
$$\xrightarrow[\ \frac17\mathrm{IV}\to\mathrm{IV}\ ]{\ \frac17\mathrm{III}\to\mathrm{III}\ }\left[\begin{array}{cccc|c}1&0&3&0&0\\0&1&0&3&1\\0&0&1&0&\frac17\\0&0&0&1&\frac27\end{array}\right]\xrightarrow[\ \mathrm{II}-3\mathrm{IV}\to\mathrm{II}\ ]{\ \mathrm{I}-3\mathrm{III}\to\mathrm{I}\ }\left[\begin{array}{cccc|c}1&0&0&0&-\frac37\\0&1&0&0&\frac17\\0&0&1&0&\frac17\\0&0&0&1&\frac27\end{array}\right]$$
$$\lambda_1=-\tfrac37\qquad\lambda_2=\tfrac17\qquad\mu_1=\tfrac17\qquad\mu_2=\tfrac27$$

$$\underbrace{\left(-\tfrac37\begin{bmatrix}-2&0\\1&0\end{bmatrix}+\tfrac17\begin{bmatrix}0&-2\\0&1\end{bmatrix}\right)}_{A_1}+\underbrace{\left(\tfrac17\begin{bmatrix}1&0\\3&0\end{bmatrix}+\tfrac27\begin{bmatrix}0&1\\0&3\end{bmatrix}\right)}_{A_2}=\begin{bmatrix}1&0\\0&1\end{bmatrix}=\mathrm{Id}_2$$

**Risposta: sì.**

> [!note] Osservazione (non presente negli appunti)
> Calcolando i prodotti: $A_1=\begin{bmatrix}\frac67&-\frac27\\-\frac37&\frac17\end{bmatrix}\in V$ e $A_2=\begin{bmatrix}\frac17&\frac27\\\frac37&\frac67\end{bmatrix}\in W$ (verificato: $BA_1=\underline{0}$ e $A_1+A_2=\mathrm{Id}_2$). Inoltre la matrice dei coefficienti è stata ridotta a quattro pivot: i quattro vettori delle basi di $V$ e $W$ sono indipendenti e generano $M_{\mathbb{R}}(2,2)$ ($\dim=2+2=4$). Quindi **ogni** matrice $2\times2$ si scrive in modo unico come somma di un elemento di $V$ e uno di $W$, non solo $\mathrm{Id}_2$.

## Note collegate
- [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]]
- [[128_Fac_simile_ii_Dimensione_e_Basi_di_V_e_W]]
- [[121_Basi_Canoniche]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/esercizi/fac-simile-28-10
