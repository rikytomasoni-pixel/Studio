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

# Potenze con Base ed Esponente Variabili

Per $a_n>0$: $a_n^{b_n}=e^{\log a_n^{b_n}}=e^{b_n\log a_n}$. Se $\lim a_n=a>0$ e $\lim b_n=b\in\mathbb{R}$ allora $\lim b_n\log a_n=b\log a\in\mathbb{R}$, quindi
$$\lim a_n^{b_n}=e^{b\log a}=e^{\log a^b}=a^b.$$

> **Teorema.** Siano $a_n,b_n$ con $\lim a_n=a\in\overline{\mathbb{R}}$, $a\ge0$ (con $a_n>0$ definitivamente), e $\lim b_n=b\in\overline{\mathbb{R}}$. Allora $\lim a_n^{b_n}=a^b$ (salvo forme indeterminate), dove:
> - $a^{+\infty}=+\infty$ e $a^{-\infty}=0$ $\forall a>1$ (anche $a=+\infty$);
> - $a^{+\infty}=0$ e $a^{-\infty}=+\infty$ $\forall a\in[0,1)$;
> - $(+\infty)^b=+\infty$ $\forall b>0$ (anche $b=+\infty$) e $(+\infty)^b=0$ $\forall b<0$ (anche $b=-\infty$).

**Osservazione.** $\infty^0$, $0^0$, $1^{\pm\infty}$ sono **esclusi**: sono forme di indeterminazione. Invece $a_n\equiv1$, $b_n=n$ dà $1^n\to1$ e $a_n\equiv0$, $b_n=n$ dà $0^n\to0$: questi **non** sono forme di indeterminazione.

**Esempio.** $\displaystyle\lim n^{1/n}=1$ (forma $\infty^0$). Si scrive $n^{1/n}=e^{\frac1n\log n}$ e $\frac1n\log n\to0$ per la gerarchia degli infiniti, quindi $n^{1/n}\to e^0=1$.

---
Precedente: [[Tecniche per le Forme Infinito meno Infinito]] · Successivo: [[Numero di Nepero]]
