---
tags:
  - AM1
  - successioni
  - criterio-del-rapporto
  - teorema
data: 2026-10-07
fonte: Lezione 8
---

# Criterio del rapporto (per successioni)

> [!abstract] Teorema — Criterio del rapporto per successioni
> Sia $a_n$ successione tale che $a_n>0$ definitivamente in $n\in\mathbb{N}$. Supponiamo esista
> $$l = \lim_{n\to\infty} \dfrac{a_{n+1}}{a_n} \in\overline{\mathbb{R}}$$
>
> Allora:
> - se $l>1$, allora $\displaystyle\lim_{n\to\infty} a_n = +\infty$
> - se $0\leq l<1$, allora $\displaystyle\lim_{n\to\infty} a_n = 0$

**Osservazione.** Se $l=1$ non si può concludere nulla sul $\displaystyle\lim_{n\to\infty} a_n$.

*(Senza dimostrazione: è contenuta nella dimostrazione del criterio del rapporto per serie, che vedremo.)*

## Esempi

**Esempio.** $\displaystyle\lim_{n\to\infty} \dfrac{a^n}{n!} = 0 \qquad a>0$

Ovvio se $a\in[0,1]$. In generale, sia $a_n=\dfrac{a^n}{n!}$:
$$\dfrac{a_{n+1}}{a_n} = \dfrac{a^{n+1}}{(n+1)!}\cdot\dfrac{n!}{a^n} = \dfrac{a\cdot n!}{(n+1)\cdot n!} = \dfrac{a}{n+1}$$
$$\Rightarrow\quad l = \lim_{n\to\infty} \dfrac{a_{n+1}}{a_n} = \lim_{n\to\infty} \dfrac{a}{n+1} = 0 \quad \forall\, a>0$$
$$\Rightarrow\quad l\in[0,1) \quad\Rightarrow\quad \lim_{n\to\infty} a_n = \lim_{n\to\infty} \dfrac{a^n}{n!} = 0$$
per criterio del rapporto.

**Esempio.** $\displaystyle\lim_{n\to\infty} \dfrac{n^n}{n!} = +\infty$

Sia $a_n=\dfrac{n^n}{n!}$,
$$\dfrac{a_{n+1}}{a_n} = \dfrac{(n+1)^{n+1}}{(n+1)!}\cdot\dfrac{n!}{n^n} = \dfrac{(n+1)(n+1)^n\, n!}{(n+1)\, n!\; n^n} = \left(\dfrac{n+1}{n}\right)^n = \left(1+\dfrac{1}{n}\right)^n$$
$$\Rightarrow\quad l = \lim_{n\to\infty} \dfrac{a_{n+1}}{a_n} = \lim_{n\to\infty} \left(1+\dfrac{1}{n}\right)^n = e\in(1,\infty]$$
$$\Rightarrow\quad \lim_{n\to\infty} a_n = \lim_{n\to\infty} \dfrac{n^n}{n!} = +\infty$$
per criterio del rapporto.

**Osservazione.**
$$\lim_{n\to\infty} \dfrac{n!}{n^n} = \lim_{n\to\infty} \left(\dfrac{n^n}{n!}\right)^{-1} = 0$$

## Gerarchia degli infiniti

> [!abstract] Gerarchia degli infiniti
> $$(\log_a n)^\beta \ll n^\alpha \ll a^n \ll n! \ll n^n \qquad \forall\, \beta>0,\ \forall\, \alpha>0,\ \forall\, a>1$$

Vedi [[36_Gerarchia_degli_Infiniti]].

**Esempio.** $\displaystyle\lim_{n\to\infty} n^{1/n} = 1 \qquad [\infty^0]$

$$n^{\frac{1}{n}} = e^{\log n^{\frac{1}{n}}} = e^{\frac{1}{n}\log n}$$
$$\lim_{n\to\infty} \dfrac{1}{n}\log n = 0 \quad \text{per gerarchia degli infiniti}$$
$$\Rightarrow\quad \lim_{n\to\infty} n^{\frac{1}{n}} = \lim_{n\to\infty} e^{\frac{1}{n}\log n} = e^0 = 1$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[36_Gerarchia_degli_Infiniti]] — usato negli esempi
- [[38_Numero_di_Nepero]] — limite notevole $e$ usato nell'esempio $n^n/n!$
- [[37_Algebra_Limiti_Infiniti]]
- [[64_Criterio_del_Rapporto_per_Serie]] — versione per serie (con le conseguenze sul limite)

#AM1/successioni-e-limiti/criterio-del-rapporto
