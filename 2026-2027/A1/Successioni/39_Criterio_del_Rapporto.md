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

## Applicazione alla gerarchia degli infiniti

**Osservazione.** $\displaystyle\lim_{n\to\infty} n^{1/n} = 1$ $\quad [\infty^0]$

$$n^{1/n} = e^{\frac{1}{n}\log n}, \qquad \dfrac{\log n}{n} \to 0 \quad \text{per gerarchia degli infiniti}$$
$$\Rightarrow \quad \lim_{n\to\infty} n^{1/n} = \lim_{n\to\infty} e^{\frac{\log n}{n}} = e^0 = 1$$

### Note collegate
- [[00_MOC_A1]]
- [[36_Gerarchia_degli_Infiniti]] — usato negli esempi
- [[38_Numero_di_Nepero]] — limite notevole $e$ usato nell'esempio $n^n/n!$
- [[37_Algebra_Limiti_Infiniti]]