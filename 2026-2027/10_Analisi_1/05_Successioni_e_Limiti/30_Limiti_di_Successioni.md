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

**Dimostrazione.** Per assurdo supponiamo esistano $l, l'\in\mathbb{R}$, $l\neq l'$, tali che
$$\lim_{n\to\infty} a_n = l, \qquad \lim_{n\to\infty} a_n = l'$$
Per comodità sia $l<l'$.

Nella definizione di limite scegliamo $\varepsilon = \dfrac{l'-l}{2}$.

![[BandeLimitiDisgiunti.png]]

In questo modo gli intervalli sono disgiunti. Infatti ciò equivale a
$$l+\varepsilon \leq l'-\varepsilon \quad\Longleftrightarrow\quad l'-l-2\varepsilon\geq 0 \quad\Longleftrightarrow\quad l'-l-(l'-l) = 0 \geq 0$$
che è vero.

Quindi $(l-\varepsilon,l+\varepsilon)\cap(l'-\varepsilon,l'+\varepsilon)=\emptyset$, gli intervalli sono disgiunti.

Per definizione di limite:
$$\exists\, N_1\in\mathbb{N} : \forall\, n\geq N_1 \quad a_n\in(l-\varepsilon,l+\varepsilon)$$
$$\exists\, N_2\in\mathbb{N} : \forall\, n\geq N_2 \quad a_n\in(l'-\varepsilon,l'+\varepsilon)$$

Ma allora $\forall\, n\geq N=\max\{N_1,N_2\}$ deve essere
$$a_n \in (l-\varepsilon,l+\varepsilon)\cap(l'-\varepsilon,l'+\varepsilon) = \emptyset$$
Assurdo. Quindi se $\exists \lim_{n\to\infty} a_n\in\mathbb{R}$, esso è unico. $\blacksquare$

**Esempio.** $\lim_{n\to\infty} \dfrac{1}{n} = 0$.

Fissato $\varepsilon>0$ vogliamo risolvere
$$\left|\dfrac{1}{n}-0\right|<\varepsilon \quad\Longleftrightarrow\quad \dfrac{1}{n}<\varepsilon \quad\Longleftrightarrow\quad n>\dfrac{1}{\varepsilon}$$
quindi $\forall\, n\geq N$ con $N>\dfrac{1}{\varepsilon}$, per definizione $\lim_{n\to\infty} \dfrac{1}{n}=0$.

## Divergenza

> [!warning] Definizione — Divergenza a $+\infty$
> Diremo che $a_n$ **diverge a $+\infty$**, e scriveremo $\lim_{n\to\infty} a_n = +\infty$, se
> $$\forall\, M>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad a_n>M$$

![[Divergenza+Infinito.png]]

> [!warning] Definizione — Divergenza a $-\infty$
> Diremo che $a_n$ **diverge a $-\infty$**, e scriveremo $\lim_{n\to\infty} a_n = -\infty$, se
> $$\forall\, M>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad a_n<-M$$

![[Divergenza-Infinito.png]]

**Esempio.** $\lim_{n\to\infty} \log n = +\infty$.

$\forall\, M>0$ cerchiamo $n$ tale che $\log n>M$, cioè $n>e^M$; per definizione $\lim_{n\to\infty}\log n = +\infty$.

## Regolarità

> [!warning] Definizione
> Sia $\overline{\mathbb{R}} = \mathbb{R}\cup\{+\infty\}\cup\{-\infty\}$.
>
> Se $\lim_{n\to\infty} a_n = l\in\mathbb{R}$, diremo che $a_n$ **converge** (a $l$).
> Se $\lim_{n\to\infty} a_n = \pm\infty$, diremo che $a_n$ **diverge** (a $\pm\infty$).
>
> In ciascun caso diremo che $a_n$ è **regolare**.
>
> Se $a_n$ non converge né diverge, diremo che essa è **irregolare** (o oscillante, o indeterminata).

**Esempi.**
$$a_n = (-1)^n \quad \text{irregolare, limitata}$$
$$a_n = (-2)^n \quad \text{irregolare, illimitata}$$
$$a_n = 2^n \quad \text{regolare, non limitata (illimitata dall'alto)}$$

> [!abstract] Teorema — Unicità del limite (in $\overline{\mathbb{R}}$)
> Se esiste $\lim_{n\to\infty} a_n = l \in\overline{\mathbb{R}}$, allora tale limite è unico.
> *(non dim., segue dallo stesso argomento usato per $l\in\mathbb{R}$)*

> [!warning] Definizione — Successione infinitesima/infinita
> Se $\lim_{n\to\infty} a_n = 0$ diremo che $a_n$ è una **successione infinitesima**.
>
> Se $\lim_{n\to\infty} |a_n| = +\infty$ diremo che $a_n$ è una **successione infinita**.

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
$$\lim_{n\to\infty}\left(1+\dfrac{1}{n}\right) = 1^+ \qquad \text{(per eccesso)}$$
$$\lim_{n\to\infty}\left(1-\dfrac{1}{n}\right) = 1^- \qquad \text{(per difetto)}$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[29_Successioni_Definizioni_Base]] — definizioni preliminari
- [[31_Successioni_Monotone]] — teorema sul limite di successioni monotone
- [[32_Successione_Convergente_e_Limitata]]
- [[09_Valore_Assoluto]] — disuguaglianza triangolare
- [[08_Estremo_Superiore_Inferiore]] — $\overline{\mathbb{R}}$
- [[04_Dimostrazione_per_Assurdo]] — metodo usato nella dimostrazione dell'unicità del limite

#AM1/successioni-e-limiti/limiti-di-successioni
