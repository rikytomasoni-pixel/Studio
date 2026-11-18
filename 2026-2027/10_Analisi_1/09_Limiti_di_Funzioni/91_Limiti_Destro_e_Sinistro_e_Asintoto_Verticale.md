---
tags:
  - AM1
  - limiti-di-funzioni
  - limite-destro-sinistro
  - asintoto-verticale
  - definizione
  - proposizione
  - li
data: 2026-10-28
lezione: 14
fonte: AM1 L14 26-27.pdf (pag. 3-6)
---

# Limiti da destra e da sinistra e asintoto verticale

Talvolta è necessario distinguere il comportamento al limite di $f$ a seconda che $x$ si avvicini a $x_0$ da destra o da sinistra.

> [!note] Osservazione (non presente negli appunti)
> Nel quaderno, accanto a "da destra" e "da sinistra", compaiono tra parentesi "per eccesso" e "per difetto". Più avanti nella stessa lezione ([[92_Limite_Finito_in_un_Punto_Finito]]) le due coppie di nozioni vengono tenute distinte: **da destra/da sinistra** riguarda il modo in cui $x\to x_0^{\pm}$, **per eccesso/per difetto** ([[88_Asintoto_Orizzontale_e_Limiti_per_Eccesso_e_per_Difetto]]) riguarda il lato da cui $f(x)$ si avvicina a $\ell$.

> [!abstract] Definizione — limite $+\infty$ ($-\infty$) da destra e da sinistra
> Data $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in\mathbb{R}$ di accumulazione per $I\cap(x_0,+\infty)$ (rispettivamente per $I\cap(-\infty,x_0)$):
>
> $\displaystyle\lim_{x\to x_0^+}f(x)=+\infty\ (-\infty)$ se $\forall M>0\ \exists\delta>0$ tale che
> $$x_0<x<x_0+\delta\ \Rightarrow\ f(x)>M\quad(f(x)<-M)$$
>
> $\displaystyle\lim_{x\to x_0^-}f(x)=+\infty\ (-\infty)$ se $\forall M>0\ \exists\delta>0$ tale che
> $$x_0-\delta<x<x_0\ \Rightarrow\ f(x)>M\quad(f(x)<-M)$$

> [!note] Osservazione
> Definizione simile per $\displaystyle\lim_{x\to x_0^{\pm}}f(x)=\ell\in\mathbb{R}$ (vedi [[92_Limite_Finito_in_un_Punto_Finito]]).

> [!example] Esempio
> $\displaystyle\lim_{x\to0}\frac1x$ **non esiste**, mentre
> $$\lim_{x\to0^+}\frac1x=+\infty\qquad\lim_{x\to0^-}\frac1x=-\infty$$

> [!abstract] Proposizione
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in\mathbb{R}$ punto di accumulazione per $I\cap(x_0,+\infty)$ e per $I\cap(-\infty,x_0)$, $\ell\in\overline{\mathbb{R}}$. Allora
> $$\lim_{x\to x_0}f(x)=\ell\iff\lim_{x\to x_0^+}f(x)=\lim_{x\to x_0^-}f(x)=\ell$$

> [!note] Osservazione
> Se almeno uno tra $\displaystyle\lim_{x\to x_0^+}f(x)$ e $\displaystyle\lim_{x\to x_0^-}f(x)$ non esiste, oppure se esistono entrambi ma sono diversi, allora $\nexists\displaystyle\lim_{x\to x_0}f(x)$.

> [!abstract] Definizione — asintoto verticale
> Se $x_0\in\mathbb{R}$ e
> $$\lim_{x\to x_0^+}f(x)=\pm\infty\quad\text{oppure}\quad\lim_{x\to x_0^-}f(x)=\pm\infty$$
> (include i casi in cui $\displaystyle\lim_{x\to x_0}f(x)=\pm\infty$), allora diremo che $x=x_0$ è un **asintoto verticale** per $f$.

> [!example] Esempi
> $f(x)=\dfrac1{x^2}$, $\ f(x)=\log x$, $\ f(x)=\dfrac1x$ (tutte con asintoto verticale $x=0$).

![[TrisDiFunzioni.png]]

## Note collegate
- [[90_Limite_Infinito_in_un_Punto_Finito]]
- [[92_Limite_Finito_in_un_Punto_Finito]]
- [[88_Asintoto_Orizzontale_e_Limiti_per_Eccesso_e_per_Difetto]]
- [[89_Asintoto_Obliquo]]
- [[97_Discontinuita_di_Prima_Specie_a_Salto]]
- [[00_MOC_Analisi_1]]
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]] (derivata destra e sinistra)
- [[125_Derivata_Infinita_e_Tangente_Verticale]]

#AM1/limiti-di-funzioni/limiti-destro-sinistro
