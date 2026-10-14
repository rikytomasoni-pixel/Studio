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

# Criterio del Rapporto

> [!abstract] Teorema — Criterio del rapporto
> Sia $a_n$ successione tale che $a_n\neq 0$ definitivamente in $n\in\mathbb{N}$. Supponiamo esista
> $$l = \lim_{n\to\infty} \left|\dfrac{a_{n+1}}{a_n}\right| \in\overline{\mathbb{R}}$$
>
> Allora:
> - se $l>1$, allora $\lim_{n\to\infty} |a_n| = +\infty$
> - se $l<1$, allora $\lim_{n\to\infty} a_n = 0$
> - se $l=1$, non si può concludere nulla sul limite di $a_n$

**Nota.** La dimostrazione è contenuta nella dimostrazione del criterio del rapporto per serie, che vedremo in seguito.

## Esempi

**Esempio.** $\displaystyle\lim_{n\to\infty} \dfrac{2^n}{n!} = 0$

Verifica con il criterio del rapporto: sia $a_n=\dfrac{2^n}{n!}$,
$$\left|\dfrac{a_{n+1}}{a_n}\right| = \dfrac{2^{n+1}}{(n+1)!}\cdot\dfrac{n!}{2^n} = \dfrac{2}{n+1} \to 0$$
$$\Rightarrow \quad l=0\in[0,1) \quad\Rightarrow\quad \lim_{n\to\infty} a_n = \lim_{n\to\infty} \dfrac{2^n}{n!} = 0$$
per criterio del rapporto.

**Esempio.** $\displaystyle\lim_{n\to\infty} \dfrac{n^n}{n!} = +\infty$

Sia $a_n=\dfrac{n^n}{n!}$,
$$\left|\dfrac{a_{n+1}}{a_n}\right| = \dfrac{(n+1)^{n+1}}{(n+1)!}\cdot\dfrac{n!}{n^n} = \left(\dfrac{n+1}{n}\right)^n = \left(1+\dfrac{1}{n}\right)^n \to e$$
$$\Rightarrow \quad l=e\in(1,\infty] \quad\Rightarrow\quad \lim_{n\to\infty} |a_n| = \lim_{n\to\infty} \dfrac{n^n}{n!} = +\infty$$
per criterio del rapporto.

---
Precedente: [[Numero di Nepero]] · Successivo: [[Ordini di Infinito e Infinitesimo]]
