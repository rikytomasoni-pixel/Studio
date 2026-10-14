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

# Aritmetizzazione dell'Infinito e Forme di Indeterminazione

> **Teorema.** Siano $a_n,b_n$ successioni.
> 1. Se $\lim a_n=a\in\mathbb{R}$ e $\lim b_n=\pm\infty$ $\Rightarrow$ $\lim(a_n+b_n)=\pm\infty$ (ovvero $a\pm\infty=\pm\infty$, $\forall a\in\mathbb{R}$).
> 2. Se $\lim a_n=\pm\infty$ e $\lim b_n=\pm\infty$ **concordi in segno** $\Rightarrow$ $\lim(a_n+b_n)=\pm\infty$ (stesso segno): $+\infty+\infty=+\infty$, $-\infty-\infty=-\infty$.
> 3. Se $\lim a_n=a\in\overline{\mathbb{R}}\setminus\{0\}$ e $\lim b_n=\pm\infty$ $\Rightarrow$ $\lim a_nb_n=\pm\infty$ con la **regola dei segni**: $+$ se $a>0$ e $\lim b_n=+\infty$, o $a<0$ e $\lim b_n=-\infty$; $-$ altrimenti. Cioè $\pm\infty\cdot a=\pm\infty$ con regola dei segni $\forall a\in\overline{\mathbb{R}}\setminus\{0\}$.
> 4. Se $\lim a_n=a\in\overline{\mathbb{R}}\setminus\{0\}$ e $\lim b_n=0^\pm$ ($b_n\neq0$ definitivamente) $\Rightarrow$ $\lim\dfrac{a_n}{b_n}=\pm\infty$ con la regola dei segni: $\dfrac a{0^\pm}=\pm\infty$.
> 5. Se $\lim a_n=a\in\mathbb{R}$ e $\lim b_n=\pm\infty$ $\Rightarrow$ $\lim\dfrac{a_n}{b_n}=0$ (ovvero $\dfrac a{\pm\infty}=0$ $\forall a\in\mathbb{R}$).

### Forme di indeterminazione
$$\infty-\infty,\qquad\infty\cdot0,\qquad\frac\infty\infty,\qquad\frac00$$
sono **forme di indeterminazione**: nulla si può dire in generale.

**Esempi per $[0\cdot\infty]$** (tutti con $b_n=\sqrt7\,n\to\infty$):

| $a_n$ | $a_nb_n$ | Limite |
|---|---|---|
| $\dfrac1n$ | $\sqrt7$ | $\sqrt7$ |
| $\dfrac1{n^2}$ | $\dfrac{\sqrt7}n$ | $0$ |
| $\dfrac1{\sqrt n}$ | $\sqrt7\sqrt n$ | $+\infty$ |
| $\dfrac{(-1)^n}n$ | $(-1)^n\sqrt7$ | non esiste |

---
Precedente: [[Rapporti di Somme di Potenze]] · Successivo: [[Tecniche per le Forme Infinito meno Infinito]]
