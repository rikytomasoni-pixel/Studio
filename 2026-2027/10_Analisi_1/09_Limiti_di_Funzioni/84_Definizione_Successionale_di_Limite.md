---
tags:
  - AM1
  - limiti-di-funzioni
  - limite-successionale
  - definizione
data: 2026-10-23
fonte: "AM1 L13 26-27.pdf (pag. 4-6)"
---

# Definizione successionale di limite

> [!abstract] Definizione (definizione successionale di limite)
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$ ($I$ insieme) e sia $x_0\in\overline{\mathbb{R}}$ punto di accumulazione per $I$ ([[83_Punti_di_Accumulazione]]). Sia $\ell\in\overline{\mathbb{R}}$.
>
> Se per ogni successione $\{x_n\}$ tale che
> 1. $\{x_n\}\subset I$
> 2. $x_n\neq x_0$ $\ \forall n\geq1$
> 3. $\displaystyle\lim_{n\to\infty}x_n=x_0$
>
> vale $\displaystyle\lim_{n\to\infty}f(x_n)=\ell$, allora diremo che
> $$\lim_{x\to x_0}f(x)=\ell$$

## Non esistenza del limite

> [!note] Osservazione
> Se esistono due successioni $\{x_n\}$, $\{z_n\}$ tali che
> 1. $\{x_n\}\subset I$, $\{z_n\}\subset I$
> 2. $x_n\neq x_0$, $z_n\neq x_0$ $\ \forall n\geq1$
> 3. $\displaystyle\lim_{n\to\infty}z_n=\lim_{n\to\infty}x_n=x_0$
>
> e
> $$\lim_{n\to\infty}f(x_n)=\ell_1,\qquad\lim_{n\to\infty}f(z_n)=\ell_2$$
> con $\ell_1,\ell_2\in\overline{\mathbb{R}}$, $\ell_1\neq\ell_2$, allora
> $$\nexists\lim_{x\to x_0}f(x)$$

> [!example] Esempio: $\nexists\displaystyle\lim_{x\to+\infty}\sin x$
> Qui $x_0=+\infty$. Infatti, siano
> $$x_n=\frac\pi2+2n\pi\quad(n\geq1),\qquad z_n=\frac{3}{2}\pi+2n\pi\quad(n\geq1)$$
> Allora $\displaystyle\lim_{n\to\infty}z_n=+\infty=\lim_{n\to\infty}x_n$ ($=x_0$). Tuttavia
> $$\lim_{n\to\infty}\sin z_n=-1\neq1=\lim_{n\to\infty}\sin x_n\ \Rightarrow\ \nexists\lim_{x\to+\infty}\sin x$$

## Note collegate
- [[83_Punti_di_Accumulazione]]
- [[85_Teorema_di_Unicita_del_Limite]]
- [[86_Definizione_Topologica_di_Limite]]
- [[30_Limiti_di_Successioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/definizione-successionale
