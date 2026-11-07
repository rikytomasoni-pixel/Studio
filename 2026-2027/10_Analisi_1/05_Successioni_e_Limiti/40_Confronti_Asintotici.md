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

> [!warning] Definizione — Ordine di infinito
> Siano $a_n, b_n$ successioni infinite, cioè
> $$\lim_{n\to\infty} a_n = \pm\infty, \qquad \lim_{n\to\infty} b_n = \pm\infty$$
> (non necessariamente dello stesso segno). Se
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = \begin{cases}
> 0 & a_n \text{ è infinito di ordine inferiore rispetto a } b_n\\
> l\in\mathbb{R}\setminus\{0\} & a_n, b_n \text{ sono infiniti dello stesso ordine}\\
> \pm\infty & b_n \text{ è infinito di ordine inferiore rispetto a } a_n\\
> \nexists & a_n, b_n \text{ non confrontabili}
> \end{cases}$$

**Esempio.** $(\log_a n)^\beta$ è infinito di ordine inferiore rispetto a $n^\alpha, a^n, n!, n^n$, $\forall\, a>1$, $\forall\, \alpha>0$, $\forall\, \beta>0$.

**Esempio.** $n!$ è infinito di ordine superiore rispetto a $n^\alpha, a^n, (\log_a n)^\beta$, $\forall\, a>1$, $\forall\, \alpha>0$, $\forall\, \beta>0$.

**Esempio.** $\log n$, $\log n^2$ sono infiniti dello stesso ordine.

Infatti
$$\dfrac{\log n}{\log n^2} = \dfrac{\log n}{2\log n} = \dfrac{1}{2} \ \longrightarrow\ \dfrac{1}{2}$$

**Esempio.** $(2+\sin n)\,n$ e $n$ non sono confrontabili.

### Note collegate
- [[00_MOC_Analisi_1]]
- [[36_Gerarchia_degli_Infiniti]] — esempi di confronto tra infiniti
- [[41_o_piccolo_e_Asintotico]] — ordine di infinitesimo, notazioni $o(\cdot)$ e $\sim$
- [[30_Limiti_di_Successioni]]

#AM1/successioni-e-limiti/confronti-asintotici
