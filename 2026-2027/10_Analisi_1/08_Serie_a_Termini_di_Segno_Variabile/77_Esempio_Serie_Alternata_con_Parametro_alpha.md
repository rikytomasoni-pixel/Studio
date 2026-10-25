---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - leibniz
  - convergenza-assoluta
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 17-19)"
---

# Esempio: la serie $\sum\frac{(-1)^n}{n^\alpha}$

> [!example] Esempio
> $$\sum_{n=1}^\infty\frac{(-1)^n}{n^\alpha}\qquad\alpha\in\mathbb{R},\qquad a_n=\frac{1}{n^\alpha}$$

## Convergenza semplice
- $a_n\geq0$ (serie a termini di segno alterno);
- $$\lim_{n\to\infty}a_n=\begin{cases}0 & \forall\alpha>0\\ 1 & \text{se }\alpha=0\\ +\infty & \text{se }\alpha<0\end{cases}$$
  la serie **non converge** se $\alpha\leq0$ (non è verificata la condizione necessaria $\lim a_n=0$, [[54_Condizione_Necessaria_di_Convergenza]]: la serie è **indeterminata**);
- se $\alpha>0$: $a_{n+1}=\dfrac{1}{(n+1)^\alpha}<\dfrac{1}{n^\alpha}=a_n$ $\ \forall n\geq1$, quindi $a_n$ è decrescente.

Per il criterio di Leibniz ([[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]), $\displaystyle\sum_{n=1}^\infty\frac{(-1)^n}{n^\alpha}$ **converge semplicemente** $\forall\alpha>0$.

## Convergenza assoluta
$$\sum_{n=1}^\infty\left|\frac{(-1)^n}{n^\alpha}\right|=\sum_{n=1}^\infty\frac{1}{n^\alpha}$$
è la serie armonica generalizzata ([[60_Serie_Armonica_Generalizzata]]): converge se $\alpha>1$, diverge se $\alpha\leq1$. Quindi $\sum\frac{(-1)^n}{n^\alpha}$ converge assolutamente se e solo se $\alpha>1$.

## Riassunto
$$\sum_{n=1}^\infty\frac{(-1)^n}{n^\alpha}$$
- è **indeterminata** per $\alpha\leq0$;
- converge **semplicemente ma non assolutamente** per $0<\alpha\leq1$;
- converge **assolutamente**, e quindi semplicemente, per $\alpha>1$.

## Note collegate
- [[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]
- [[73_Convergenza_Assoluta_e_Semplice]]
- [[60_Serie_Armonica_Generalizzata]]
- [[78_Osservazioni_sul_Criterio_di_Leibniz]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-serie-alternata-alpha
