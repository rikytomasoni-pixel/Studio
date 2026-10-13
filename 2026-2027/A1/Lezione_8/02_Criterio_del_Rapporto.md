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
> Sia $a_n$ una successione tale che $a_n>0$ definitivamente in $n\in\mathbb{N}$. Supponiamo che esista
> $$l=\lim_{n\to\infty}\dfrac{a_{n+1}}{a_n}\in\overline{\mathbb{R}}$$
> Allora:
> - se $l>1$, allora $\lim_{n\to\infty}a_n=+\infty$
> - se $0\leq l<1$, allora $\lim_{n\to\infty}a_n=0$

**Osservazione.** Se $l=1$ non si può concludere nulla sul $\lim a_n$.

(Senza dimostrazione: è contenuta nella dimostrazione del criterio del rapporto per serie, che vedremo.)

## Esempi

**Esempio.** $\displaystyle\lim_{n\to\infty}\dfrac{a^n}{n!}=0 \qquad a\geq0$

Ovvio se $a\in[0,1]$. In generale, sia $a_n=\dfrac{a^n}{n!}$:
$$\dfrac{a_{n+1}}{a_n}=\dfrac{a^{n+1}}{(n+1)!}\cdot\dfrac{n!}{a^n}=\dfrac{a\cdot n!}{(n+1)\cdot n!}=\dfrac{a}{n+1}$$
$$\Rightarrow\ l=\lim_{n\to\infty}\dfrac{a_{n+1}}{a_n}=\lim_{n\to\infty}\dfrac{a}{n+1}=0\quad\forall\,a>0\ \Rightarrow\ l\in[0,1)\ \Rightarrow\ \lim_{n\to\infty}a_n=\lim_{n\to\infty}\dfrac{a^n}{n!}=0$$
per criterio del rapporto.

**Esempio.** $\displaystyle\lim_{n\to\infty}\dfrac{n^n}{n!}=+\infty$

Sia $a_n=\dfrac{n^n}{n!}$:
$$\dfrac{a_{n+1}}{a_n}=\dfrac{(n+1)^{n+1}}{(n+1)!}\cdot\dfrac{n!}{n^n}=\dfrac{(n+1)(n+1)^n\,n!}{(n+1)\,n!\,n^n}=\left(\dfrac{n+1}{n}\right)^n=\left(1+\dfrac1n\right)^n$$
$$\Rightarrow\ l=\lim_{n\to\infty}\dfrac{a_{n+1}}{a_n}=\lim_{n\to\infty}\left(1+\dfrac1n\right)^n=e\in(1,\infty]\ \Rightarrow\ \lim_{n\to\infty}a_n=\lim_{n\to\infty}\dfrac{n^n}{n!}=\infty$$
per criterio del rapporto.

**Osservazione.**
$$\lim_{n\to\infty}\dfrac{n!}{n^n}=\lim_{n\to\infty}\left(\dfrac{n^n}{n!}\right)^{-1}=0$$

## Gerarchia degli infiniti

> [!abstract] Gerarchia degli infiniti
> $$(\log_a n)^\beta\ \ll\ n^\alpha\ \ll\ a^n\ \ll\ n!\ \ll\ n^n \qquad \forall\,\beta>0,\ \forall\,\alpha>0,\ \forall\,a>1$$

**Esempio.** $\displaystyle\lim_{n\to\infty}n^{1/n}=1 \quad [\infty^0]$

$$n^{\frac1n}=e^{\log n^{\frac1n}}=e^{\frac1n\log n}$$
$$\lim_{n\to\infty}\dfrac1n\log n=0\quad\text{per gerarchia degli infiniti}\ \Rightarrow\ \lim_{n\to\infty}n^{\frac1n}=\lim_{n\to\infty}e^{\frac1n\log n}=e^0=1$$

> [!warning] Differenze rispetto alla trascrizione precedente
> La versione precedente scriveva il criterio con $\left|\frac{a_{n+1}}{a_n}\right|$, $a_n\neq0$ e $\lim|a_n|=+\infty$ (generalizzazione corretta ma **non** presente nel PDF, che ha $a_n>0$ definitivamente) e usava l'esempio $\frac{2^n}{n!}$, che è il caso $a=2$ dell'esempio generale $\frac{a^n}{n!}$ del PDF.

### Note collegate
- [[00_MOC_A1]]
- [[04_Gerarchia_degli_Infiniti]] — usato negli esempi
- [[01_Numero_di_Nepero]] — limite notevole $e$ usato nell'esempio $n^n/n!$
- [[00_Algebra_Limiti_Infiniti]]
