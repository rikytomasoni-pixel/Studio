---
tags:
  - AM1
  - successioni
  - teorema-del-confronto
  - carabinieri
  - limiti
data: 2026-10-02
fonte: Lezione 7
---

# Teoremi del confronto per successioni

## Teorema del confronto per successioni convergenti (dei due carabinieri)

> [!abstract] Teorema
> Date tre successioni $a_n, b_n, c_n$ tali che
> $$a_n \leq c_n \leq b_n \quad \text{definitivamente in } n\in\mathbb{N}$$
> e tali che $\exists\, \lim_{n\to\infty} a_n = \lim_{n\to\infty} b_n = l\in\mathbb{R}$. Allora
> $$\exists\, \lim_{n\to\infty} c_n = l \in\mathbb{R}$$

**Dimostrazione.** Per definizione di limite:
$$\exists\, N_1\in\mathbb{N} \text{ tale che } \forall\, n\geq N_1 \quad |a_n-l|<\varepsilon \quad \text{cioè} \quad l-\varepsilon<a_n<l+\varepsilon \qquad (①)$$
$$\exists\, N_2\in\mathbb{N} \text{ tale che } \forall\, n\geq N_2 \quad |b_n-l|<\varepsilon \quad \text{cioè} \quad l-\varepsilon<b_n<l+\varepsilon \qquad (②)$$
Inoltre $\exists\, N_3\in\mathbb{N}$ tale che $\forall\, n\geq N_3$ $a_n\leq c_n\leq b_n$ $\quad (③)$

Allora $\forall\, n\geq N=\max\{N_1,N_2,N_3\}$ (da ①②③):
$$l-\varepsilon<a_n\leq c_n\leq b_n<l+\varepsilon$$
$$\Rightarrow \quad \forall\, \varepsilon>0\ \exists\, N\in\mathbb{N} : \forall\, n\geq N \quad l-\varepsilon<c_n<l+\varepsilon$$
cioè, per definizione, $\lim_{n\to\infty} c_n = l$. $\blacksquare$

## Teorema del confronto per successioni divergenti

> [!abstract] Teorema
> Date due successioni $a_n, b_n$ tali che $a_n\leq b_n$ definitivamente in $n\in\mathbb{N}$. Allora:
>
> 1. se $\lim_{n\to\infty} a_n = +\infty$, allora $\exists\, \lim_{n\to\infty} b_n = +\infty$
> 2. se $\lim_{n\to\infty} b_n = -\infty$, allora $\exists\, \lim_{n\to\infty} a_n = -\infty$

**Dimostrazione.** Si dimostra solo 1); 2) è analoga.

Per definizione di limite, $\forall\, M>0$:
$$\exists\, N_1\in\mathbb{N} \text{ tale che } \forall\, n\geq N_1 \quad a_n>M \qquad (①)$$
Inoltre $\exists\, N_2\in\mathbb{N}$ tale che $\forall\, n\geq N_2$ vale $a_n\leq b_n$ $\quad (②)$

Quindi $\forall\, M>0\ \exists\, N=\max\{N_1,N_2\}$ tale che $\forall\, n\geq N$ (da ①②):
$$M<a_n\leq b_n$$
$$\Rightarrow \quad \forall\, M>0\ \exists\, N\in\mathbb{N} : \forall\, n\geq N \quad M<b_n$$
cioè, per definizione, $\lim_{n\to\infty} b_n = +\infty$. $\blacksquare$

## Corollari

> [!abstract] Corollario
> **1)** Se $b_n, a_n$ sono successioni tali che $|b_n|\leq a_n$ definitivamente in $n\in\mathbb{N}$ e se $\lim_{n\to\infty} a_n=0$, allora
> $$\exists\, \lim_{n\to\infty} b_n = 0 \qquad \left(\lim_{n\to\infty}|b_n|=0\right)$$
>
> **2)** Se $b_n, a_n$ sono successioni tali che $a_n$ è limitata e $\lim_{n\to\infty} b_n=0$, allora
> $$\lim_{n\to\infty} a_n\cdot b_n = 0$$
> anche se $a_n$ non converge.

**Esempio.** Siano $a_n=\dfrac{1}{n}$, $b_n=\sin n$.

$\lim_{n\to\infty} a_n=0$ e $|b_n|=|\sin n|\leq 1\ \ \forall\, n\in\mathbb{N}$ ($b_n$ limitata, anche se non converge).

Dal corollario precedente segue
$$\lim_{n\to\infty} a_n\cdot b_n = \lim_{n\to\infty} \dfrac{\sin n}{n} = 0$$

### Note collegate
- [[00_MOC_A1]]
- [[30_Limiti_di_Successioni]]
- [[33_Teorema_Permanenza_del_Segno]]
- [[34_Algebra_dei_Limiti]]
- [[36_Gerarchia_degli_Infiniti]]