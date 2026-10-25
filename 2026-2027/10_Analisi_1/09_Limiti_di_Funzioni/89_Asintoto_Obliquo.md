---
tags:
  - AM1
  - limiti-di-funzioni
  - asintoto-obliquo
  - definizione
  - proposizione
data: 2026-10-23
fonte: "AM1 L13 26-27.pdf (pag. 15-16)"
---

# Asintoto obliquo

> [!abstract] Definizione — asintoto obliquo
> $f$ ha **asintoto obliquo** $y=mx+q$, con $m\in\mathbb{R}\setminus\{0\}$ e $q\in\mathbb{R}$, per $x\to+\infty$ (rispettivamente $x\to-\infty$) se
> $$\lim_{x\to+\infty}\big(f(x)-(mx+q)\big)=0\qquad\left(\text{rispettivamente }\lim_{x\to-\infty}\big(f(x)-(mx+q)\big)=0\right)$$

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** pag. 16, in alto. **Cosa cercare:** grafico di $f(x)$ (nero) che si avvicina alla retta $y=mx+q$ (blu) al crescere di $x$; in un punto $x$ è tracciato un segmento verticale tratteggiato rosso tra $f(x)$ e $mx+q$.

$|f(x)-(mx+q)|$ è la lunghezza del segmento verticale di estremi $(x,f(x))$ e $(x,mx+q)$, rispettivamente sul grafico di $f$ e sull'asintoto.

> [!note] Osservazione
> $\displaystyle\lim_{x\to\pm\infty}\big(f(x)-(mx+q)\big)=0$ equivale a
> $$f(x)-(mx+q)=o(1)\quad x\to\pm\infty,\qquad f(x)=mx+q+o(1)\quad x\to\pm\infty$$
> (vedi [[41_o_piccolo_e_Asintotico]]).

> [!abstract] Proposizione
> $f$ ha asintoto obliquo a $\pm\infty$ se e solo se
> 1. $\displaystyle\lim_{x\to\pm\infty}\frac{f(x)}{x}=m\in\mathbb{R}\setminus\{0\}$
> 2. $\displaystyle\lim_{x\to\pm\infty}\big(f(x)-mx\big)=q\in\mathbb{R}$
>
> In tal caso l'asintoto è $y=mx+q$.

## Esempi
> [!example] $f(x)=2x+3+e^{-x}$
> Ha asintoto obliquo $y=2x+3$ a $+\infty$ ($f(x)=2x+3+o(1)$ a $+\infty$).
> Non ha asintoto obliquo a $-\infty$ ($\displaystyle\lim_{x\to-\infty}\frac{f(x)}{x}=-\infty$).

> [!example] $f(x)=2x+3+\log x$
> **Non** ha asintoto obliquo a $+\infty$:
> $$\lim_{x\to+\infty}\frac{f(x)}{x}=2\qquad\qquad\lim_{x\to+\infty}\big(f(x)-2x\big)=+\infty$$

## Note collegate
- [[88_Asintoto_Orizzontale_e_Limiti_per_Eccesso_e_per_Difetto]]
- [[87_Definizioni_Metriche_di_Limite_all_Infinito]]
- [[41_o_piccolo_e_Asintotico]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/asintoto-obliquo
