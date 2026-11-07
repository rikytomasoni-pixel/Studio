---
tags:
  - AM1
  - successioni
  - o-piccolo
  - asintotico
  - infinitesimi
data: 2026-10-07
fonte: Lezione 8
---

# Ordine di infinitesimo, o-piccolo, successioni asintotiche

## Ordine di infinitesimo

> [!warning] Definizione — Ordine di infinitesimo
> Date due successioni infinitesime $a_n, b_n$, cioè
> $$\lim_{n\to\infty} a_n = \lim_{n\to\infty} b_n = 0$$
> (con $b_n\neq 0$ definitivamente in $n\in\mathbb{N}$), se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = \begin{cases}
> 0 & a_n \text{ infinitesimo di ordine superiore rispetto a } b_n\\
> l\in\mathbb{R}\setminus\{0\} & a_n, b_n \text{ infinitesimi dello stesso ordine}\\
> \pm\infty & b_n \text{ infinitesimo di ordine superiore rispetto a } a_n\\
> \nexists & a_n, b_n \text{ non confrontabili}
> \end{cases}$$

**Esempio.** $\dfrac{1}{n^n}$ è infinitesimo di ordine superiore rispetto a $\dfrac{1}{n^\alpha}$, $\dfrac{1}{(\log_a n)^\beta}$, $\dfrac{1}{a^n}$, $\dfrac{1}{n!}$, $\forall\, \alpha>0$, $\forall\, \beta>0$, $\forall\, a>1$.

## $o$-piccolo e asintotico

> [!warning] Definizione
> Date due successioni $a_n, b_n$ qualsiasi (con $b_n\neq 0$ definitivamente in $n\in\mathbb{N}$), diremo che:
> - $a_n$ è **$o$-piccolo** di $b_n$, e scriveremo $a_n=o(b_n)$ per $n\to\infty$, se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 0$$
> - $a_n$ è **asintotico** a $b_n$, e scriveremo $a_n\sim b_n$ per $n\to\infty$, se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 1$$

**Osservazioni.**
- Se $\displaystyle\lim_{n\to\infty} \dfrac{a_n}{b_n}=\pm\infty$, allora $\displaystyle\lim_{n\to\infty} \dfrac{b_n}{a_n}=0$, cioè $b_n=o(a_n)$.
- Se $\displaystyle\lim_{n\to\infty} \dfrac{a_n}{b_n}=l\in\mathbb{R}\setminus\{0\}$, allora $\displaystyle\lim_{n\to\infty} \dfrac{a_n}{l\,b_n}=1$, cioè $a_n\sim l\,b_n$.

## Gerarchia degli infiniti in termini di $o$-piccolo

**Osservazione.**
$$(\log_a n)^\beta = o(n^\alpha) \qquad \forall\, \alpha>0,\ \forall\, \beta>0,\ \forall\, a>1$$
$$n^\alpha = o(a^n) \qquad \forall\, \alpha>0,\ \forall\, a>1$$
$$a^n = o(n!) \qquad \forall\, a>1$$
$$n! = o(n^n)$$

## Esempio applicativo

**Esempio.** $a_n = 7n^{47} + \log n + \log\log n + (\log n)^{18} + \sin n + n^{18} - 1 + \arctan n^2$

Il termine dominante è $7n^{47}$: tutti gli altri addendi sono $o(n^{47})$ per $n\to\infty$. Quindi
$$a_n = 7n^{47} + o(n^{47}) \ \sim\ 7n^{47}$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[40_Confronti_Asintotici]] — ordine di infinito (nozione duale per successioni che divergono)
- [[36_Gerarchia_degli_Infiniti]]
- [[30_Limiti_di_Successioni]]

#AM1/successioni-e-limiti/o-piccolo-e-asintotico
