---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - criterio-della-radice
  - leibniz
  - convergenza-assoluta
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 24-27)"
---

# Esempio: la serie $\sum\frac{(\alpha-1)^n}{n\,2^n}$

> [!example] Esempio
> $$\sum_{n=1}^\infty\frac{(\alpha-1)^n}{n\,2^n}\qquad\alpha\in\mathbb{R}$$
> $a_n=\dfrac{(\alpha-1)^n}{n\,2^n}=\dfrac1n\,q^n$ con $q=\dfrac{\alpha-1}{2}$.

## Condizione necessaria: $a_n\to0$?
Per la gerarchia degli infiniti ([[36_Gerarchia_degli_Infiniti]])
$$a_n\longrightarrow\begin{cases}+\infty & q=\frac{\alpha-1}{2}>1\\ 0 & |q|=\left|\frac{\alpha-1}{2}\right|\leq1\\ \nexists & q=\frac{\alpha-1}{2}<-1\end{cases}$$
Condizione $-1\leq\frac{\alpha-1}{2}\leq1$ $\iff$ $-2\leq\alpha-1\leq2$ $\iff$ $-1\leq\alpha\leq3$.

La serie **non converge per $\alpha>3$** (diverge a $+\infty$) **né per $\alpha<-1$** (indeterminata). La serie può convergere solo per $-1\leq\alpha\leq3$.

## Caso $\alpha\in[-1,3]$: convergenza assoluta con il criterio della radice
$$|a_n|=\frac1n\left|\frac{\alpha-1}{2}\right|^n=\frac1n|q|^n$$
$$\sqrt[n]{|a_n|}=\frac{1}{\sqrt[n]{n}}|q|=e^{\log n^{-1/n}}|q|=|q|\,e^{-\frac1n\log n}\longrightarrow|q|\,e^0=|q|$$
per gerarchia infiniti ($\frac{\log n}{n}\to0$). Quindi
$$\lim_{n\to\infty}\sqrt[n]{|a_n|}=|q|=\left|\frac{\alpha-1}{2}\right|$$
Per il criterio della radice ([[65_Criterio_della_Radice_per_Serie]]), $\sum|a_n|$ converge se $\left|\frac{\alpha-1}{2}\right|<1$, cioè $-1<\frac{\alpha-1}{2}<1$, cioè $-1<\alpha<3$.

$\Rightarrow$ per $\alpha\in(-1,3)$, $\sum|a_n|$ converge, cioè $\sum a_n$ **converge assolutamente**.
$\Rightarrow$ per $\alpha\in(-1,3)$, $\sum a_n$ converge anche semplicemente per il criterio di convergenza assoluta ([[74_Criterio_di_Convergenza_Assoluta]]).

## Casi rimasti: $\left|\frac{\alpha-1}{2}\right|=1$, cioè $\alpha=-1$ e $\alpha=3$
- **$\alpha=3$**: la serie diventa $\displaystyle\sum_{n=1}^\infty\frac1n$, che diverge a $+\infty$ (serie armonica, [[55_Serie_Armonica]]).
- **$\alpha=-1$**: la serie diventa $\displaystyle\sum_{n=1}^\infty\frac{(-1)^n}{n}=\sum_{n=1}^\infty(-1)^nb_n$ con $b_n=\dfrac1n$. Non converge assolutamente (la serie dei moduli è la serie armonica) ma **converge semplicemente** per il criterio di Leibniz ([[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]), perché $\frac1n\geq0$, $\lim\frac1n=0$ e $\frac1n$ è decrescente.

## Riassunto
$$\sum_{n=1}^\infty\frac{(\alpha-1)^n}{n\,2^n}$$
- per $\alpha\geq3$ **diverge a $+\infty$**;
- per $-1<\alpha<3$ **converge assolutamente e semplicemente**;
- per $\alpha=-1$ **converge semplicemente ma non assolutamente**;
- per $\alpha<-1$ **non converge** (indeterminata).

## Note collegate
- [[65_Criterio_della_Radice_per_Serie]]
- [[74_Criterio_di_Convergenza_Assoluta]]
- [[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]
- [[73_Convergenza_Assoluta_e_Semplice]]
- [[36_Gerarchia_degli_Infiniti]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-alpha-meno-1-alla-n
