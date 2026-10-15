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

## $o$-piccolo

> [!warning] Definizione — $o$-piccolo
> Date due successioni $a_n, b_n$ qualsiasi (con $b_n\neq 0$ definitivamente in $n\in\mathbb{N}$), diremo che:
> - $a_n$ è **$o$-piccolo** di $b_n$, e scriveremo $a_n=o(b_n)$ per $n\to\infty$, se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 0$$

## Asintotico

> [!warning] Definizione — Asintotico
> $a_n$ è **asintotico** a $b_n$, e scriveremo $a_n\sim b_n$ per $n\to\infty$, se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 1$$

**Osservazioni.**
- Se $a_n = o(b_n)$, allora $\lim_{n\to\infty} \dfrac{a_n}{b_n}=0 \ \Rightarrow\ b_n \not\sim a_n$ in generale (da non confondere le due nozioni).
- Se $\lim_{n\to\infty} \dfrac{a_n}{b_n}=l\in\mathbb{R}\setminus\{0\}$, allora $a_n\sim l\,b_n$.

## Gerarchia degli infiniti in termini di $o$-piccolo

**Osservazione.**
$$(\log n)^\alpha = o(n^\beta) \qquad \forall\, \alpha,\beta>0$$
$$n^\alpha = o(q^n) \qquad \forall\, \alpha>0,\ q>1$$
$$q^n = o(n!) \qquad \forall\, q>0$$
$$n! = o(n^n)$$

## Esempio applicativo

**Esempio.** $a_n = 7n^4+\log n + \log\log n + (\log n)^{100} + n^{18} + n-1$

Il termine dominante è $7n^4$: tutti gli altri addendi sono $o(n^4)$ per $n\to\infty$. Quindi
$$a_n = 7n^4 + o(n^4)$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[40_Confronti_Asintotici]] — ordine di infinito (nozione duale per successioni che divergono)
- [[36_Gerarchia_degli_Infiniti]]
- [[30_Limiti_di_Successioni]]

#AM1/successioni-e-limiti/o-piccolo-e-asintotico
