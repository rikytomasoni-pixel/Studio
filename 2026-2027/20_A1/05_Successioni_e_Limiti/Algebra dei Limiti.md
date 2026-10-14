---
created: 2026-10-02
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/successioni_e_limiti
aliases: []
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Algebra dei Limiti

> **Teorema (algebra dei limiti).** Siano $a_n,b_n$ due successioni con $a=\lim a_n$, $b=\lim b_n\in\mathbb{R}$. Allora:
> 1. $\lim(a_n\pm b_n)=a\pm b$;
> 2. $\lim a_n\cdot b_n=a\cdot b$;
> 3. $\lim\dfrac{a_n}{b_n}=\dfrac ab$ (se $b\neq0$);
> 4. $\lim a_n^{\,b_n}=a^b$ (se $a>0$).

**Dimostrazione.**

*1) Somma.* Per la [[2026-09-16 A1 Lezione 2|disuguaglianza triangolare]] ($|x+y|\le|x|+|y|$):
$$|(a_n+b_n)-(a+b)|=|(a_n-a)+(b_n-b)|\le|a_n-a|+|b_n-b|.$$
Per definizione di limite $\forall\varepsilon>0$ esistono $N_1,N_2$ tali che $|a_n-a|<\frac\varepsilon2$ per $n\ge N_1$ e $|b_n-b|<\frac\varepsilon2$ per $n\ge N_2$. Per $n\ge\max\{N_1,N_2\}$:
$$|(a_n+b_n)-(a+b)|<\frac\varepsilon2+\frac\varepsilon2=\varepsilon\ \Rightarrow\ \lim(a_n+b_n)=a+b.$$
Similmente per «$-$».

*2) Prodotto.* Si osserva che
$$|a_nb_n-ab|=|a_nb_n-a_nb+a_nb-ab|=|a_n(b_n-b)+b(a_n-a)|\le|a_n||b_n-b|+|b||a_n-a|.$$
Poiché $a_n$ converge, è limitata ([[Convergente implica Limitata|teorema sopra]]): $\exists M>0$ tale che $|a_n|<M\ \forall n$. Quindi
$$|a_nb_n-ab|\le M|b_n-b|+|b||a_n-a|.$$
Per definizione di limite $\forall\varepsilon>0\ \exists N_1,N_2$: $|a_n-a|<\varepsilon$ per $n\ge N_1$, $|b_n-b|<\varepsilon$ per $n\ge N_2$. Allora per $n\ge\max\{N_1,N_2\}$:
$$|a_nb_n-ab|<M\varepsilon+|b|\varepsilon=(M+|b|)\varepsilon,$$
e quindi $\lim a_nb_n=ab$.

*3), 4)* senza dimostrazione. $\square$

### Corollari (permanenza del segno + algebra)
Date $a_n,b_n$ con $\exists a=\lim a_n$, $b=\lim b_n\in\mathbb{R}$:

1. se $a>b$ ($a<b$) allora definitivamente $a_n>b_n$ ($a_n<b_n$);
2. se $a_n\ge b_n$ ($a_n\le b_n$) definitivamente in $n\in\mathbb{N}$, allora $a\ge b$ ($a\le b$).

**Dimostrazione.** Posto $c_n=a_n-b_n$, per l'algebra dei limiti $\exists c=\lim c_n=a-b\in\mathbb{R}$.
1. Se $a>b$ allora $c>0$ e per permanenza del segno $c_n>0$ definitivamente, cioè $a_n>b_n$ definitivamente.
2. Se $a_n\ge b_n$ definitivamente, $c_n\ge0$ definitivamente; poiché $\exists c=\lim c_n$, per permanenza del segno $c\ge0$, cioè $a\ge b$. $\square$

---
Precedente: [[Permanenza del Segno]] · Successivo: [[Teoremi del Confronto]]
