---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - confronto-asintotico
  - bertrand
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 28-30)"
---

# Esempio: confronto asintotico con la serie di Bertrand

> [!example] Esempio
> $$\sum_{n=2}^\infty\frac{\left[\left(1+\sin\frac1n\right)^{\log n}-1\right]^\alpha}{\left(1+\log\log n+\log n\right)\log\!\left((2n+1)^2\right)}\qquad\alpha\in\mathbb{R}$$
> Usiamo il criterio del confronto asintotico ([[62_Criterio_del_Confronto_Asintotico_per_Serie]]). Sia $a_n=\dfrac{b_n^{\,\alpha}}{c_n}$ con $b_n$ e $c_n$ come sotto.

## Numeratore
Sia
$$b_n=\left(1+\sin\frac1n\right)^{\log n}-1=(1+\varepsilon_n)^{\alpha_n}-1,\qquad\varepsilon_n=\sin\frac1n,\quad\alpha_n=\log n$$

> [!tip] Asintotico notevole
> $(1+\varepsilon_n)^{\alpha_n}-1\sim\varepsilon_n\alpha_n$ se $\varepsilon_n\to0$ e $\alpha_n\varepsilon_n\to0$ (vedi [[42_Confronti_Asintotici_Proprieta_e_Notevoli]], [[43_Asintotici_con_Funzioni_Composte]]).

Nel nostro caso $\varepsilon_n=\sin\frac1n\sim\frac1n\to0$ e
$$\alpha_n\varepsilon_n=\sin\frac1n\log n\sim\frac{\log n}{n}\to0\quad\text{per gerarchia infiniti}$$
$$\Rightarrow\ b_n\sim\sin\frac1n\,\log n\sim\frac{\log n}{n}$$

## Denominatore
Sia $c_n=\left(1+\log\log n+\log n\right)\log\!\left((2n+1)^2\right)$. Allora
$$c_n=\log n\left(\frac{1}{\log n}+\frac{\log\log n}{\log n}+1\right)\cdot2\log(2n+1)=\log n\,\big(1+o(1)\big)\cdot2\log(2n+1)$$
perché $\dfrac{\log\log n}{\log n}\to0$ per gerarchia infiniti. Quindi
$$c_n\sim2\log n\cdot\log(2n)=2\log n\,(\log n+\log2)\sim2(\log n)^2$$

## Conclusione
$$a_n=\frac{b_n^{\,\alpha}}{c_n}\sim\left(\frac{\log n}{n}\right)^{\alpha}\cdot\frac{1}{2(\log n)^2}=\frac{1}{2\,n^\alpha(\log n)^{2-\alpha}}>0$$

Poiché la serie di Bertrand ([[61_Serie_di_Bertrand_Generalizzata]])
$$\sum_{n=2}^\infty\frac{1}{n^\alpha(\log n)^\beta}$$
**converge** se $\alpha>1$, $\forall\beta\in\mathbb{R}$, oppure se $\alpha=1$, $\beta>1$, mentre **diverge** se $\alpha<1$, $\forall\beta\in\mathbb{R}$, oppure se $\alpha=1$, $\beta\leq1$, per il criterio del confronto asintotico (con $\beta=2-\alpha$) $\displaystyle\sum_{n=2}^\infty a_n$

- **converge** se $\alpha>1$;
- **diverge** se $\alpha\leq1$.

> [!note] Fine degli argomenti della I prova in itinere
> Con questo esempio terminano gli argomenti della prima prova in itinere.

## Note collegate
- [[62_Criterio_del_Confronto_Asintotico_per_Serie]]
- [[63_Esempio_Confronto_Asintotico_con_Parametro]]
- [[61_Serie_di_Bertrand_Generalizzata]]
- [[42_Confronti_Asintotici_Proprieta_e_Notevoli]]
- [[43_Asintotici_con_Funzioni_Composte]]
- [[36_Gerarchia_degli_Infiniti]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-confronto-asintotico-bertrand
