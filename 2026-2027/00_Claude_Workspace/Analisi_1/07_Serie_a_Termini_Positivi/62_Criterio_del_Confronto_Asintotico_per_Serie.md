---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - confronto-asintotico
  - teorema
  - dimostrazione
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 9-11, 14)"
stato: da_verificare
destinazione: 10_Analisi_1/07_Serie_a_Termini_Positivi (cartella nuova)
---

# Criterio del confronto asintotico per serie a termini positivi

> [!abstract] Teorema — Criterio del confronto asintotico
> Siano $a_n,b_n$ due successioni a termini (definitivamente) positivi. Supponiamo che
> $$a_n\sim b_n\qquad\left(\lim_{n\to\infty}\frac{a_n}{b_n}=1\right)$$
> Allora $\displaystyle\sum_{n=1}^\infty a_n$ e $\displaystyle\sum_{n=1}^\infty b_n$ hanno lo **stesso carattere**, cioè o convergono entrambe o divergono (a $+\infty$) entrambe.

> [!note] Osservazione
> Se le due serie convergono, il risultato della somma sarà in generale **diverso**.

## Dimostrazione
Poiché $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=1$, per ogni $\varepsilon>0$ esiste $N_1\in\mathbb{N}$ tale che per ogni $n\geq N_1$
$$1-\varepsilon<\frac{a_n}{b_n}<1+\varepsilon$$
Per $\varepsilon=\frac12$ esiste $N_1\in\mathbb{N}$ tale che per ogni $n\geq N_1$
$$\underbrace{\frac12<\frac{a_n}{b_n}}_{\textcircled{1}}\ ,\qquad\underbrace{\frac{a_n}{b_n}<\frac32}_{\textcircled{2}}$$
Poiché $a_n,b_n$ sono definitivamente positive, esiste $N_2\in\mathbb{N}$ tale che per ogni $n\geq N_2$ $a_n>0$, $b_n>0$. Allora per ogni $n\geq N=\max\{N_1,N_2\}$:
$$\textcircled{2}\Rightarrow0<a_n<\frac32b_n\qquad(**)$$
$$\textcircled{1}\Rightarrow0<b_n<2a_n\qquad(***)$$
- Per il [[58_Criterio_del_Confronto_per_Serie]], da $(**)$: se $\sum a_n$ diverge allora diverge anche $\sum b_n$; inoltre se $\sum b_n$ converge allora converge anche $\sum a_n$.
- Da $(***)$: se $\sum b_n$ diverge allora diverge anche $\sum a_n$; inoltre se $\sum a_n$ converge allora converge anche $\sum b_n$ (sempre per il criterio del confronto).

$\Rightarrow\sum a_n,\ \sum b_n$ convergono entrambe oppure divergono entrambe a $+\infty$. $\square$

## Osservazione: segno concordante
Se $a_n\sim b_n$ allora, definitivamente in $n\in\mathbb{N}$, $a_n,b_n$ sono **concordi in segno**:
$$a_n=\frac{a_n}{b_n}\cdot b_n$$
Poiché $\frac{a_n}{b_n}\to1>0$, per la permanenza del segno ([[33_Teorema_Permanenza_del_Segno]]) $\frac{a_n}{b_n}$ è definitivamente positivo. Quindi $a_n$ e $b_n$ devono essere definitivamente concordi in segno.

## Esempi
- [[63_Esempio_Confronto_Asintotico_con_Parametro]]
- [[67_Esempio_Serie_n_Fattoriale_su_n_alla_n]] (con Stirling)

## Note collegate
- [[40_Confronti_Asintotici]]
- [[42_Confronti_Asintotici_Proprieta_e_Notevoli]]
- [[60_Serie_Armonica_Generalizzata]]
- [[61_Serie_di_Bertrand_Generalizzata]]
- [[00_MOC_Analisi_1]]

#AM1/serie/confronto-asintotico
