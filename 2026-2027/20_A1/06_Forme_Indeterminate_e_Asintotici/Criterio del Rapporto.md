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

# Criterio del Rapporto

> **Teorema (criterio del rapporto).** Sia $a_n>0$ definitivamente e supponiamo esista $\ell=\displaystyle\lim_{n\to\infty}\frac{a_{n+1}}{a_n}\in\overline{\mathbb{R}}$. Allora:
> - se $\ell>1$: $\lim a_n=+\infty$;
> - se $0\le\ell<1$: $\lim a_n=0$.

**Osservazione.** Se $\ell=1$ non si può concludere nulla su $\lim a_n$. *(Senza dimostrazione: è contenuta nella dimostrazione del criterio del rapporto per serie, che vedremo.)*

**Esempio 1.** $\lim\dfrac{a^n}{n!}=0$ per $a\ge0$ (ovvio se $a\in[0,1]$). Qui $a_n=\frac{a^n}{n!}$ e
$$\frac{a_{n+1}}{a_n}=\frac{a^{n+1}}{(n+1)!}\cdot\frac{n!}{a^n}=\frac a{n+1}\to0\in[0,1)\ \Rightarrow\ \lim\frac{a^n}{n!}=0.$$

**Esempio 2.** $\lim\dfrac{n^n}{n!}=+\infty$. Con $a_n=\frac{n^n}{n!}$:
$$\frac{a_{n+1}}{a_n}=\frac{(n+1)^{n+1}}{(n+1)!}\cdot\frac{n!}{n^n}=\left(\frac{n+1}n\right)^n=\left(1+\frac1n\right)^n\to e\in(1,\infty],$$
quindi $\lim\dfrac{n^n}{n!}=+\infty$, e di conseguenza $\lim\dfrac{n!}{n^n}=\lim\left(\dfrac{n^n}{n!}\right)^{-1}=0$.

### Gerarchia degli infiniti (riquadro riassuntivo)
$$(\log_an)^\beta\ \ll\ n^\alpha\ \ll\ a^n\ \ll\ n!\ \ll\ n^n\qquad\forall\beta>0,\ \forall\alpha>0,\ \forall a>1.$$

---
Precedente: [[Numero di Nepero]] · Successivo: [[Ordini di Infinito e Infinitesimo]]
