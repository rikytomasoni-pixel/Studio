---
created: 2026-10-07
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
  - argomento/forme_indeterminate_e_asintotici
aliases: []
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Ordini di Infinito e Infinitesimo

### Ordini di infinito
**Definizione.** Siano $a_n,b_n$ **infinite** ($\lim a_n=\pm\infty$, $\lim b_n=\pm\infty$, non necessariamente con lo stesso segno). Se
$$\lim_{n\to\infty}\frac{a_n}{b_n}=\begin{cases}0&a_n\text{ è infinito di ordine inferiore rispetto a }b_n\\ \ell\in\mathbb{R}\setminus\{0\}&a_n,b_n\text{ sono infiniti dello stesso ordine}\\ \pm\infty&b_n\text{ è infinito di ordine inferiore rispetto a }a_n\\ \nexists&a_n,b_n\text{ non confrontabili}\end{cases}$$

**Esempi.**
- $(\log_an)^\beta$ è infinito di ordine inferiore rispetto a $n^\alpha,a^n,n!,n^n$ ($\forall a>1,\alpha>0,\beta>0$).
- $n!$ è infinito di ordine superiore rispetto a $n^\alpha,a^n,(\log_an)^\beta$.
- $\log n$ e $\log n^2$ sono infiniti dello stesso ordine: $\dfrac{\log n}{\log n^2}=\dfrac{\log n}{2\log n}=\dfrac12\to\dfrac12$.
- $(2+\sin n)\,n$ e $n$ sono **non confrontabili**.

### Ordini di infinitesimo
**Definizione.** Siano $a_n,b_n$ **infinitesime** ($\lim a_n=\lim b_n=0$, con $b_n\neq0$ definitivamente). Se
$$\lim_{n\to\infty}\frac{a_n}{b_n}=\begin{cases}0&a_n\text{ è infinitesimo di ordine superiore rispetto a }b_n\\ \ell\in\mathbb{R}\setminus\{0\}&\text{infinitesimi dello stesso ordine}\\ \pm\infty&b_n\text{ è infinitesimo di ordine superiore rispetto a }a_n\\ \nexists&\text{non confrontabili}\end{cases}$$

**Esempio.** $\dfrac1{n^n}$ è infinitesimo di ordine superiore rispetto a $\dfrac1{n^\alpha},\dfrac1{(\log_an)^\beta},\dfrac1{a^n},\dfrac1{n!}$ ($\forall\alpha>0,\beta>0,a>1$).

### o-piccolo e asintotico
**Definizione.** Date due successioni qualsiasi $a_n,b_n$ (con $b_n\neq0$ definitivamente):
- $a_n$ è **o-piccolo** di $b_n$, in simboli $a_n=o(b_n)$ per $n\to\infty$, se $\displaystyle\lim\frac{a_n}{b_n}=0$;
- $a_n$ è **asintotico** a $b_n$, in simboli $a_n\sim b_n$ per $n\to\infty$, se $\displaystyle\lim\frac{a_n}{b_n}=1$.

**Osservazioni.**
- Se $\lim\frac{a_n}{b_n}=\pm\infty$ allora $\lim\frac{b_n}{a_n}=0$, quindi $b_n=o(a_n)$.
- Se $\lim\frac{a_n}{b_n}=\ell\in\mathbb{R}\setminus\{0\}$ allora $\lim\frac{a_n}{\ell\,b_n}=1$, quindi $a_n\sim\ell\,b_n$.
- Gerarchia degli infiniti con o-piccolo ($\forall\alpha>0,\beta>0,a>1$):
$$(\log_an)^\beta=o(n^\alpha),\quad n^\alpha=o(a^n),\quad a^n=o(n!),\quad n!=o(n^n).$$

**Esempio.**
$$a_n=7n^{47}+\log n+\log\log n+(\log n)^{18}+\sin n+n^{18}-\arctan n^2=7n^{47}+o(n^{47})\ \sim\ 7n^{47}.$$

---
Precedente: [[Criterio del Rapporto]] · Successivo: [[Definizione di o-piccolo e Asintotico]]
