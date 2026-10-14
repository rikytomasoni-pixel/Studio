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

# Numero di Nepero

> **Teorema.** La successione $a_n=\left(1+\dfrac1n\right)^n$, $n\ge1$, è **monotona crescente e limitata**. In particolare ammette limite in $\mathbb{R}$. *(Senza dimostrazione completa.)*

**Definizione.**
$$e=\lim_{n\to\infty}\left(1+\frac1n\right)^n=2{,}71828\dots$$

**Osservazioni.**
- $e=\sup_{n\ge1}\left(1+\frac1n\right)^n$ e $e>\left(1+\frac1n\right)^n\ \forall n\ge1$.
- *Idea della dimostrazione:* sfrutta la **disuguaglianza di Bernoulli** (cfr. [[2026-09-14 A1 Lezione 1|Bernoulli]]): si mostra $\dfrac{a_n}{a_{n-1}}\ge1$ $\forall n\ge2$, quindi $a_n\ge a_{n-1}$ e $a_n$ è crescente. Un'altra applicazione della disuguaglianza di Bernoulli mostra che $a_n$ è limitata.
- Vedremo che $e=\displaystyle\sum_{n=0}^\infty\frac1{n!}$.

> **Teorema.** Sia $c_n$ una successione con $\lim c_n=\pm\infty$. Allora
> $$\lim_{n\to\infty}\left(1+\frac1{c_n}\right)^{c_n}=e.$$

> **Corollario.** $\forall a\in\mathbb{R}$: $\displaystyle\lim_{n\to\infty}\left(1+\frac an\right)^n=e^a$.

**Dimostrazione.** Se $a\neq0$, per $n$ grande $1+\frac an>0$ e
$$\left(1+\frac an\right)^n=\left[\left(1+\frac an\right)^{n/a}\right]^a=\left[\left(1+\frac1{c_n}\right)^{c_n}\right]^a,\qquad c_n=\frac na\to\pm\infty,$$
che tende a $e^a$. Se $a=0$: $\left(1+\frac0n\right)^n=1\to1=e^0$. $\square$

---
Precedente: [[Potenze con Base ed Esponente Variabili]] · Successivo: [[Criterio del Rapporto]]
