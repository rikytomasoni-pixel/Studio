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

> [!warning] Definizione
> Date due successioni infinitesime $a_n,b_n$, cioè
> $$\lim_{n\to\infty}a_n=\lim_{n\to\infty}b_n=0$$
> (con $b_n\neq0$ definitivamente in $n\in\mathbb{N}$), se
> $$\lim_{n\to\infty}\dfrac{a_n}{b_n}=\begin{cases}0 & a_n \text{ infinitesimo di ordine superiore rispetto a } b_n\\[2pt] l\in\mathbb{R}\setminus\{0\} & a_n,b_n \text{ infinitesimi dello stesso ordine}\\[2pt] \pm\infty & b_n \text{ infinitesimo di ordine superiore rispetto a } a_n\\[2pt] \nexists & a_n,b_n \text{ non confrontabili}\end{cases}$$

**Esempio.** $\dfrac{1}{n^n}$ è infinitesimo di ordine superiore rispetto a $\dfrac{1}{n^\alpha},\ \dfrac{1}{(\log_a n)^\beta},\ \dfrac{1}{a^n},\ \dfrac{1}{n!}$, $\quad\forall\,\alpha>0,\ \forall\,\beta>0,\ \forall\,a>1$.

## $o$-piccolo e asintotico

> [!warning] Definizione
> Date due successioni $a_n,b_n$ qualsiasi (con $b_n\neq0$ definitivamente in $n\in\mathbb{N}$), diremo che:
> - $a_n$ è **$o$-piccolo** di $b_n$, e scriveremo $a_n=o(b_n)$ per $n\to\infty$, se
> $$\lim_{n\to\infty}\dfrac{a_n}{b_n}=0$$
> - $a_n$ è **asintotico** a $b_n$, e scriveremo $a_n\sim b_n$ per $n\to\infty$, se
> $$\lim_{n\to\infty}\dfrac{a_n}{b_n}=1$$

**Osservazioni.**
- Se $\displaystyle\lim_{n\to\infty}\dfrac{a_n}{b_n}=\pm\infty$ allora $\displaystyle\lim_{n\to\infty}\dfrac{b_n}{a_n}=0\ \Rightarrow\ b_n=o(a_n)$.
- Se $\displaystyle\lim_{n\to\infty}\dfrac{a_n}{b_n}=l\in\mathbb{R}\setminus\{0\}$ allora $\displaystyle\lim_{n\to\infty}\dfrac{a_n}{l\cdot b_n}=1\ \Rightarrow\ a_n\sim l\,b_n$.

## Gerarchia degli infiniti in termini di $o$-piccolo

$$(\log_a n)^\beta=o(n^\alpha)\qquad\forall\,\alpha>0,\ \forall\,\beta>0,\ \forall\,a>1$$
$$n^\alpha=o(a^n)\qquad\forall\,\alpha>0,\ \forall\,a>1$$
$$a^n=o(n!)\qquad\forall\,a>1$$
$$n!=o(n^n)$$

## Esempio applicativo

**Esempio.** $a_n=7n^{47}+\log n+\log\log n+(\log n)^{18}+\sin n+n^{18}-1+\arctan n^2$

Il termine dominante è $7n^{47}$: tutti gli altri addendi sono $o(n^{47})$ per $n\to\infty$. Quindi
$$a_n=7n^{47}+o(n^{47})\ \sim\ 7n^{47}$$

> [!warning] Differenze rispetto alla trascrizione precedente
> - Nella definizione di ordine di infinitesimo la versione precedente aveva i casi $l=0$ e $l=\pm\infty$ con "ordine inferiore" **invertito**: nel PDF, se $\lim a_n/b_n=0$ allora $a_n$ è infinitesimo di ordine **superiore**; se $\pm\infty$, è $b_n$ ad essere di ordine superiore.
> - L'esempio "$\frac1{n^\alpha}$ di ordine superiore rispetto a $\frac1{\log n}$" non è nel PDF (è vero); nel PDF l'esempio è con $\frac1{n^n}$.
> - L'osservazione "$a_n=o(b_n)\Rightarrow b_n\not\sim a_n$" non è nel PDF (vera in generale); sostituita con le due osservazioni del PDF.
> - L'esempio finale era scritto con $7n^4$, $(\log n)^{100}$, $n-1$: nel PDF è $7n^{47}$, $(\log n)^{18}$, $n^{18}-1$, con in più $\sin n$ e $\arctan n^2$.

### Note collegate
- [[00_MOC_A1]]
- [[03_Confronti_Asintotici]] — ordine di infinito (nozione duale per successioni che divergono)
- [[04_Gerarchia_degli_Infiniti]]
- [[02_Limiti_di_Successioni]]
