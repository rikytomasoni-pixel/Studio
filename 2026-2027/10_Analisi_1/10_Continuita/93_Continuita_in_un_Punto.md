---
tags:
  - AM1
  - continuita
  - definizione
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 8-9, 13)"
---

# Continuità in un punto e in un insieme

> [!abstract] Definizione — funzione continua
> Data $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in I$ punto di accumulazione di $I$. Se
> $$\lim_{x\to x_0}f(x)=f(x_0)$$
> diremo che $f$ è **continua in $x_0$**.
>
> Diremo che $f$ è **continua in $I$** se essa è continua in $x_0$, $\forall x_0\in I$. Scriveremo in tal caso $f\in C^0(I)$.

> [!note] Osservazione — definizione metrica
> Secondo la definizione metrica, $f$ continua in $x_0$ se e solo se $\forall\varepsilon>0\ \exists\delta>0$ tale che
> $$x_0-\delta<x<x_0+\delta\ \Rightarrow\ f(x_0)-\varepsilon<f(x)<f(x_0)+\varepsilon\qquad\text{cioè}\qquad|x-x_0|<\delta\ \Rightarrow\ |f(x)-f(x_0)|<\varepsilon$$
> (vedi [[92_Limite_Finito_in_un_Punto_Finito]]; qui $x=x_0$ è ammesso perché $f(x_0)$ è definito).

> [!note] Osservazione — definizione successionale
> Secondo la definizione successionale ([[84_Definizione_Successionale_di_Limite]]): per ogni successione $\{x_n\}\subset I$ tale che $\displaystyle\lim_{n\to\infty}x_n=x_0$ vale
> $$\lim_{n\to\infty}f(x_n)=f(x_0)=f\Big(\lim_{n\to\infty}x_n\Big)$$

> [!note] Osservazione — dominio
> Domandarsi se $f:(-\infty,0)\cup(0,\infty)\to\mathbb{R}$, $f(x)=\dfrac1x$ $\ \forall x\neq0$, sia continua o no in $x_0=0$ **non ha senso**, secondo la definizione di continuità appena vista, perché $f$ non è definita in $x_0=0$.

## Esempi e classificazione
- [[94_Esempio_Continuita_di_e_alla_x]]
- [[95_Funzione_di_Dirichlet]]
- Punti di discontinuità: [[96_Discontinuita_Eliminabile_e_Prolungamento_per_Continuita]], [[97_Discontinuita_di_Prima_Specie_a_Salto]], [[98_Discontinuita_di_Seconda_Specie]]

## Note collegate
- [[92_Limite_Finito_in_un_Punto_Finito]]
- [[84_Definizione_Successionale_di_Limite]]
- [[103_Algebra_delle_Funzioni_Continue]]
- [[117_Continuita_delle_Funzioni_Elementari]]
- [[00_MOC_Analisi_1]]

#AM1/continuita/definizione
