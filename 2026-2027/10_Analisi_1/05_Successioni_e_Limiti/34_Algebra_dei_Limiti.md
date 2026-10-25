---
tags:
  - AM1
  - successioni
  - algebra-dei-limiti
  - teorema
data: 2026-10-02
fonte: Lezione 7
---

# Algebra dei limiti

> [!abstract] Teorema — Algebra dei limiti
> Siano $a_n, b_n$ due successioni ed esistano $a=\lim_{n\to\infty} a_n$, $b=\lim_{n\to\infty} b_n \in\mathbb{R}$. Allora:
>
> 1. $\displaystyle\lim_{n\to\infty} (a_n\pm b_n) = a\pm b$
> 2. $\displaystyle\lim_{n\to\infty} (a_n\cdot b_n) = a\cdot b$
> 3. $\displaystyle\lim_{n\to\infty} \dfrac{a_n}{b_n} = \dfrac{a}{b}$ $\quad(b\neq 0)$
> 4. $\displaystyle\lim_{n\to\infty} a_n^{\,b_n} = a^b$ $\quad(a>0)$

**Dimostrazione.**

**1)** Osserviamo che
$$|(a_n+b_n)-(a+b)| = |(a_n-a)+(b_n-b)| \leq |a_n-a|+|b_n-b|$$
per la disuguaglianza triangolare ($\forall\, x,y\in\mathbb{R}$, $|x+y|\leq|x|+|y|$).

Per definizione di limite, $\forall\, \varepsilon>0$:
$$\exists\, N_1\in\mathbb{N} : \forall\, n\geq N_1 \quad |a_n-a|<\dfrac{\varepsilon}{2}$$
$$\exists\, N_2\in\mathbb{N} : \forall\, n\geq N_2 \quad |b_n-b|<\dfrac{\varepsilon}{2}$$

Allora se $n\geq\max\{N_1,N_2\}$:
$$|(a_n+b_n)-(a+b)| \leq |a_n-a|+|b_n-b| < \dfrac{\varepsilon}{2}+\dfrac{\varepsilon}{2} = \varepsilon$$
$$\Rightarrow \quad \lim_{n\to\infty}(a_n+b_n) = a+b$$

Similmente per "$-$".

**2)** Osserviamo che
$$|a_nb_n-ab| = |a_nb_n-a_nb+a_nb-ab| = |a_n(b_n-b)+b(a_n-a)|$$
$$\leq |a_n(b_n-b)|+|b(a_n-a)| = |a_n||b_n-b|+|b||a_n-a|$$
per la disuguaglianza triangolare.

Poiché $a_n$ converge, $a_n$ è limitata (vedi [[32_Successione_Convergente_e_Limitata]]), cioè $\exists\, M>0$ tale che $|a_n|<M\ \ \forall\, n\in\mathbb{N}$.

Quindi
$$|a_nb_n-ab| \leq |a_n||b_n-b| + |b||a_n-a| \leq M|b_n-b| + |b||a_n-a|$$

Per definizione di limite, $\forall\, \varepsilon>0$:
$$\exists\, N_1\in\mathbb{N} : \forall\, n\geq N_1 \quad |a_n-a|<\varepsilon$$
$$\exists\, N_2\in\mathbb{N} : \forall\, n\geq N_2 \quad |b_n-b|<\varepsilon$$

$\Rightarrow$ $\forall\, n\geq\max\{N_1,N_2\}$ vale
$$|a_nb_n-ab| < M|b_n-b| + |b||a_n-a| < (M+|b|)\,\varepsilon$$

Per definizione di limite,
$$\lim_{n\to\infty} a_nb_n = a\cdot b \qquad \blacksquare$$

**3), 4)** Non dimostrati.

## Corollario (permanenza del segno e algebra dei limiti)

> [!abstract] Corollario
> Date due successioni $a_n, b_n$ tali che $\exists\, \lim_{n\to\infty} a_n=a$, $\lim_{n\to\infty} b_n=b\in\mathbb{R}$. Allora:
>
> 1. se $a>b$ ($a<b$ risp.), allora definitivamente $a_n>b_n$ ($a_n<b_n$ risp.)
> 2. se $a_n\geq b_n$ ($a_n\leq b_n$ risp.) definitivamente in $n\in\mathbb{N}$, allora $a\geq b$ ($a\leq b$ risp.)

**Dimostrazione.** Sia $c_n=a_n-b_n$; allora, per l'algebra dei limiti, $\exists\, c=\lim_{n\to\infty} c_n = a-b\in\mathbb{R}$.

**1)** Se $a>b$ allora $c>0$ e, per permanenza del segno, $c_n>0$ definitivamente in $n\in\mathbb{N}$, che equivale a $a_n>b_n$ definitivamente in $n\in\mathbb{N}$.

**2)** Se $a_n\geq b_n$ definitivamente, allora $c_n=a_n-b_n\geq 0$ definitivamente. Perché $\exists\, c=\lim_{n\to\infty} c_n$, deve essere $c\geq 0$ per permanenza del segno. Ciò equivale a $a\geq b$. $\blacksquare$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[33_Teorema_Permanenza_del_Segno]]
- [[30_Limiti_di_Successioni]]
- [[32_Successione_Convergente_e_Limitata]] — successione convergente è limitata (usato nella dimostrazione)
- [[09_Valore_Assoluto]] — disuguaglianza triangolare
- [[35_Teoremi_del_Confronto]]

#AM1/successioni-e-limiti/algebra-dei-limiti
