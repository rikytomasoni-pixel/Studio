---
tags:
  - AM1
  - successioni
  - confronti-asintotici
  - ordine-di-infinito
  - ordine-di-infinitesimo
data: 2026-10-07
fonte: Lezione 8
---

# Confronti e stime asintotiche: ordine di infinito

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

### Note collegate
- [[00_MOC_Analisi_1]]
- [[36_Gerarchia_degli_Infiniti]] — esempi di confronto tra infiniti
- [[41_o_piccolo_e_Asintotico]] — notazioni $o(\cdot)$ e $\sim$
- [[30_Limiti_di_Successioni]]

#AM1/successioni-e-limiti/confronti-asintotici
