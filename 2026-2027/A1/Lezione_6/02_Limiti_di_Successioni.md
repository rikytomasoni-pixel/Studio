---
tags:
  - AM1
  - successioni
  - limiti
  - convergenza
  - divergenza
  - successioni-regolari
data: 2026-09-30
fonte: Lezione 6
---

# Limiti di successioni: convergenza, divergenza, regolarità

## Convergenza

> [!warning] Definizione — Convergenza
> Diremo che una successione $a_n$ **converge** a $l\in\mathbb{R}$, e scriveremo
> $$\lim_{n\to\infty} a_n = l$$
> se $\forall\, \varepsilon>0\ \exists\, N\in\mathbb{N}$ tale che
> $$\forall\, n\geq N \quad |a_n-l|<\varepsilon \qquad (l-\varepsilon<a_n<l+\varepsilon)$$

![[BandaContenenteLimite.png]]

**Osservazioni.**
$$\lim_{n\to\infty} a_n = l \quad\Longleftrightarrow\quad \lim_{n\to\infty} |a_n-l| = 0 \quad\Longleftrightarrow\quad \lim_{n\to\infty} (a_n-l) = 0$$

**Osservazione.** Non tutte le successioni ammettono limite $l\in\mathbb{R}$.
$$\nexists\, \lim_{n\to\infty} n = l\in\mathbb{R}, \qquad a_n=n$$
$$\nexists\, \lim_{n\to\infty} (-1)^n = l\in\mathbb{R}, \qquad a_n=(-1)^n$$

### Unicità del limite

> [!abstract] Teorema — Unicità del limite
> Data una successione $a_n$, se esiste $\lim_{n\to\infty} a_n = l \in\mathbb{R}$, allora esso è unico.

**Dimostrazione.** Per assurdo supponiamo esistano $l_1, l_2\in\mathbb{R}$, $l_1\neq l_2$, tali che
$$\lim_{n\to\infty} a_n = l_1, \qquad \lim_{n\to\infty} a_n = l_2$$
Per comodità sia $l_1>l_2$.

Nella definizione di limite scegliamo $\varepsilon = \dfrac{1}{3}\,|l_1-l_2| = \dfrac{l_1-l_2}{3}>0$.

![[BandeLimitiDisgiunti.png]]

In questo modo $l_1-\varepsilon>l_2+\varepsilon$. Infatti ciò equivale a
$$l_1-l_2>2\varepsilon = 2\,\dfrac{l_1-l_2}{3} \quad\Longleftrightarrow\quad \dfrac{1}{3}(l_1-l_2)>0$$
che è vero.

Quindi $(l_1-\varepsilon,l_1+\varepsilon)\cap(l_2-\varepsilon,l_2+\varepsilon)=\emptyset$, gli intervalli sono disgiunti.

Per definizione di limite:
$$\exists\, N_1\in\mathbb{N} : \forall\, n\geq N_1 \quad a_n\in(l_1-\varepsilon,l_1+\varepsilon)$$
$$\exists\, N_2\in\mathbb{N} : \forall\, n\geq N_2 \quad a_n\in(l_2-\varepsilon,l_2+\varepsilon)$$

Ma allora $\forall\, n\geq N=\max\{N_1,N_2\}$ deve essere
$$a_n \in (l_1-\varepsilon,l_1+\varepsilon)\cap(l_2-\varepsilon,l_2+\varepsilon) = \emptyset$$
Assurdo. Quindi se $\exists \lim_{n\to\infty} a_n\in\mathbb{R}$, esso è unico. $\blacksquare$

**Esempio.** $\lim_{n\to\infty} \dfrac{1}{n} = 0$.

Fissato $\varepsilon>0$ si risolve
$$|a_n-0|<\varepsilon \quad\Longleftrightarrow\quad 0-\varepsilon<a_n<0+\varepsilon \quad\Longleftrightarrow\quad \begin{cases} a_n<\varepsilon \\ a_n>-\varepsilon\end{cases} \quad\Longleftrightarrow\quad \begin{cases} \dfrac1n<\varepsilon \\[2mm] \dfrac1n>-\varepsilon\end{cases} \quad\Longleftrightarrow\quad \begin{cases} n>\dfrac1\varepsilon \\[2mm] \forall\, n\in\mathbb{N} \quad \left(\dfrac1n>0>-\varepsilon\right)\end{cases}$$
$$\Longrightarrow\quad n>\dfrac1\varepsilon$$
$\lim_{n\to\infty}\dfrac1n=0$ per definizione.

## Divergenza

> [!warning] Definizione — Divergenza a $+\infty$
> Diremo che $a_n$ **diverge a $+\infty$**, e scriveremo $\lim_{n\to\infty} a_n = +\infty$, se
> $$\forall\, M>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad a_n>M$$

![[Divergenza+Infinito.png]]

> [!warning] Definizione — Divergenza a $-\infty$
> Diremo che $a_n$ **diverge a $-\infty$**, e scriveremo $\lim_{n\to\infty} a_n = -\infty$, se
> $$\forall\, M>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad a_n<-M$$

![[Divergenza-Infinito.png]]

**Esempio.** $\lim_{n\to\infty} \log\dfrac1n = -\infty$, con $a_n=\log\dfrac1n$.

$\forall\, M>0$ risolvo $\log\dfrac1n<-M \iff \dfrac1n<e^{-M} \iff n>e^M$ ✓.

$\lim_{n\to\infty}\log\dfrac1n=-\infty$ per definizione.

## Regolarità

> [!warning] Definizione
> Sia $\overline{\mathbb{R}} = \mathbb{R}\cup\{+\infty\}\cup\{-\infty\}$ ($\mathbb{R}$ esteso).
>
> Se $\lim_{n\to\infty} a_n = l\in\mathbb{R}$, diremo che $a_n$ **converge** (a $l$).
> Se $\lim_{n\to\infty} a_n = \pm\infty$, diremo che $a_n$ **diverge** (a $\pm\infty$).
>
> In ciascun caso diremo che $a_n$ è **regolare**.
>
> Se $a_n$ non converge né diverge, diremo che essa è **irregolare** (o oscillante, o indeterminata): $\nexists\,\lim_{n\to\infty}a_n$ in $\overline{\mathbb{R}}$.

**Esempi.**
$$a_n = (-1)^n \quad \text{irregolare, limitata}$$
$$a_n = (-2)^n \quad \text{irregolare, illimitata}$$
$$a_n = \begin{cases} 2^n & \text{se } n \text{ pari} \\ 1 & \text{se } n \text{ dispari}\end{cases} \quad \text{irregolare, illimitata dall'alto}$$

> [!abstract] Teorema — Unicità del limite (in $\overline{\mathbb{R}}$)
> Se esiste $\lim_{n\to\infty} a_n = l \in\overline{\mathbb{R}}$, allora tale limite è unico.
> *(non dim.)*

> [!warning] Definizione — Successione infinitesima/infinita
> Se $\lim_{n\to\infty} a_n = 0$ diremo che $a_n$ è una **successione infinitesima**.
>
> Se $\lim_{n\to\infty} a_n = \pm\infty$ diremo che $a_n$ è una **successione infinita**.

## Convergenza per eccesso e per difetto

> [!warning] Definizione
> Diremo che $a_n$ converge a $l$ **per eccesso** (**per difetto**) se
> $$\lim_{n\to\infty} a_n = l$$
> ed inoltre $a_n\geq l$ ($a_n\leq l$) definitivamente per $n\in\mathbb{N}$.
>
> Scriveremo
> $$\lim_{n\to\infty} a_n = l^+ \qquad (l^-)$$

**Osservazione.**
$$\lim_{n\to\infty} a_n = l^+ \quad\Longleftrightarrow\quad \forall\, \varepsilon>0\ \exists\, N\in\mathbb{N} : \forall\, n\geq N \quad l\leq a_n < l+\varepsilon$$

![[LimiteEccesso.png]]

$$\lim_{n\to\infty} a_n = l^- \quad\Longleftrightarrow\quad \forall\, \varepsilon>0\ \exists\, N\in\mathbb{N} : \forall\, n\geq N \quad l-\varepsilon<a_n\leq l$$

**Esempio.**
$$\lim_{n\to\infty} 2^{1/n} = 1^+$$
$$\lim_{n\to\infty} \dfrac{n}{n+1} = 1^-$$
$$\lim_{n\to\infty} \dfrac{(-1)^n}{n} = 0 \qquad \text{(né per eccesso né per difetto)}$$

### Note collegate
- [[00_MOC_A1]]
- [[01_Successioni_Definizioni_Base]] — definizioni preliminari
- [[03_Successioni_Monotone]] — teorema sul limite di successioni monotone
- [[00_Successione_Convergente_e_Limitata]]
- [[03_Valore_Assoluto]] — disuguaglianza triangolare
- [[02_Estremo_Superiore_Inferiore]] — $\overline{\mathbb{R}}$
- [[03_Dimostrazione_per_Assurdo]] — metodo usato nella dimostrazione dell'unicità del limite