---
tags:
  - AM1
  - successioni
  - numero-di-nepero
  - teorema
data: 2026-10-07
fonte: Lezione 8
---

# Numero di Nepero

> [!abstract] Teorema
> La successione
> $$a_n = \left(1+\dfrac{1}{n}\right)^n, \qquad n\geq 1$$
> è monotona crescente e limitata.
>
> In particolare essa ammette limite $l\in\mathbb{R}$.
>
> (senza dimostrazione)

> [!note] Definizione — Numero di Nepero
> $$e = \lim_{n\to\infty} \left(1+\dfrac{1}{n}\right)^n = 2{,}71828\ldots$$

**Osservazione.**
$$e = \sup_{n\geq 1} \left(1+\dfrac{1}{n}\right)^n$$
$$e > \left(1+\dfrac{1}{n}\right)^n \qquad \forall\, n\geq 1$$

**Idea della dimostrazione.** Si sfrutta la disuguaglianza di Bernoulli (vedi [[04_Dimostrazione_per_Induzione]]): si dimostra che
$$\dfrac{a_n}{a_{n-1}} \geq 1 \qquad \forall\, n\geq 2$$
$$\Rightarrow \quad a_n \geq a_{n-1} \quad\Rightarrow\quad a_n \text{ crescente}$$

Un'altra applicazione della disuguaglianza di Bernoulli dimostra che $a_n$ è limitata.

**Osservazione.** $e = \displaystyle\sum_{n=0}^{\infty} \dfrac{1}{n!}$ (vedremo in seguito).

## Teorema — limite notevole generalizzato

> [!abstract] Teorema
> Se $c_n$ è una successione tale che
> $$\lim_{n\to\infty} c_n = \pm\infty$$
> allora
> $$\lim_{n\to\infty} \left(1+\dfrac{1}{c_n}\right)^{c_n} = e$$

**Corollario.** $\forall\, a\in\mathbb{R}$:
$$\lim_{n\to\infty} \left(1+\dfrac{a}{n}\right)^n = e^a$$

**Dimostrazione.** Per $n$ grande $\left(1+\dfrac{a}{n}\right)>0$ e, se $a\neq0$, vale
$$\left(1+\dfrac{a}{n}\right)^n = \left[\left(1+\dfrac{a}{n}\right)^{n/a}\right]^a = \left[\left(1+\dfrac{1}{n/a}\right)^{n/a}\right]^a = \left[\left(1+\dfrac{1}{c_n}\right)^{c_n}\right]^a \to e^a \qquad c_n=\dfrac{n}{a}$$

Se $a=0$: $\left(1+\dfrac{0}{n}\right)^n = 1 = e^0$. $\blacksquare$

### Note collegate
- [[00_MOC_A1]]
- [[03_Successioni_Monotone]] — teorema sul limite di successioni monotone e limitate (usato qui)
- [[00_Algebra_Limiti_Infiniti]] — forma indeterminata $1^\infty$
- [[04_Dimostrazione_per_Induzione]] — disuguaglianza di Bernoulli
- [[02_Criterio_del_Rapporto]]