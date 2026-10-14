---
created: 2026-10-07
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
  - argomento/forme_indeterminate_e_asintotici
aliases: []
origine: UpdateVault
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Ordini di Infinito e Infinitesimo

## Confronti e stime asintotiche: ordine di infinito

> [!warning] Definizione
> Siano $a_n, b_n$ successioni infinite, cioè
> $$\lim_{n\to\infty} |a_n| = +\infty, \qquad \lim_{n\to\infty} |b_n| = +\infty$$
> (non necessariamente dello stesso segno). Se esiste
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = l \in\mathbb{R}\setminus\{0\}$$
> allora $a_n$ e $b_n$ si dicono **infiniti dello stesso ordine**.
>
> - Se $l=0$: $a_n$ è **infinito di ordine inferiore** rispetto a $b_n$.
> - Se $l=\pm\infty$: $b_n$ è **infinito di ordine inferiore** rispetto a $a_n$.
> - Se $\nexists\, \lim \dfrac{a_n}{b_n}$: $a_n, b_n$ **non sono confrontabili**.

**Esempio.** $(\log n)^\beta$ è infinito di ordine inferiore rispetto a $n^\alpha, q^n, n!$, $\forall\, \alpha,\beta>0$, $\forall\, q>1$.

**Esempio.** $n!$ è infinito di ordine superiore rispetto a $n^\alpha, q^n, (\log n)^\beta$, $\forall\, \alpha,\beta>0$, $\forall\, q>0$.

**Esempio.** $\log n$, $\log(n^2)$ sono infiniti dello stesso ordine.

Infatti $\dfrac{\log(n^2)}{\log n} = \dfrac{2\log n}{\log n} = 2 \ \to\ 2 \neq 0,\pm\infty$.

**Esempio.** $n+\sin n$, $n$ non sono confrontabili? In realtà:
$$\lim_{n\to\infty} \dfrac{n+\sin n}{n} = 1 \quad \text{(stesso ordine)}$$

## Ordine di infinitesimo, o-piccolo, successioni asintotiche

### Ordine di infinitesimo

> [!warning] Definizione
> Date due successioni infinitesime $a_n, b_n$, cioè
> $$\lim_{n\to\infty} a_n = \lim_{n\to\infty} b_n = 0$$
> (con $b_n\neq 0$ definitivamente in $n\in\mathbb{N}$), se esiste
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = l$$
> allora:
> - se $l\in\mathbb{R}\setminus\{0\}$: $a_n, b_n$ sono **infinitesimi dello stesso ordine**
> - se $l=0$: $a_n$ è infinitesimo di **ordine inferiore** rispetto a $b_n$
> - se $l=\pm\infty$: $b_n$ è infinitesimo di **ordine inferiore** rispetto a $a_n$
> - se $\nexists\, l$: $a_n, b_n$ **non sono confrontabili**

**Esempio.** $\dfrac{1}{n^\alpha}$ è infinitesimo di ordine superiore rispetto a $\dfrac{1}{\log n}$, $\forall\, \alpha>0$.

### $o$-piccolo

> [!warning] Definizione — $o$-piccolo
> Date due successioni $a_n, b_n$ qualsiasi (con $b_n\neq 0$ definitivamente in $n\in\mathbb{N}$), diremo che:
> - $a_n$ è **$o$-piccolo** di $b_n$, e scriveremo $a_n=o(b_n)$ per $n\to\infty$, se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 0$$

### Asintotico

> [!warning] Definizione — Asintotico
> $a_n$ è **asintotico** a $b_n$, e scriveremo $a_n\sim b_n$ per $n\to\infty$, se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 1$$

**Osservazioni.**
- Se $a_n = o(b_n)$, allora $\lim_{n\to\infty} \dfrac{a_n}{b_n}=0 \ \Rightarrow\ b_n \not\sim a_n$ in generale (da non confondere le due nozioni).
- Se $\lim_{n\to\infty} \dfrac{a_n}{b_n}=l\in\mathbb{R}\setminus\{0\}$, allora $a_n\sim l\,b_n$.

### Gerarchia degli infiniti in termini di $o$-piccolo

**Osservazione.**
$$(\log n)^\alpha = o(n^\beta) \qquad \forall\, \alpha,\beta>0$$
$$n^\alpha = o(q^n) \qquad \forall\, \alpha>0,\ q>1$$
$$q^n = o(n!) \qquad \forall\, q>0$$
$$n! = o(n^n)$$

### Esempio applicativo

**Esempio.** $a_n = 7n^4+\log n + \log\log n + (\log n)^{100} + n^{18} + n-1$

Il termine dominante è $7n^4$: tutti gli altri addendi sono $o(n^4)$ per $n\to\infty$. Quindi
$$a_n = 7n^4 + o(n^4)$$

---
Precedente: [[Criterio del Rapporto]] · Successivo: [[Definizione di o-piccolo e Asintotico]]
