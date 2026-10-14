---
created: 2026-09-30
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/successioni_e_limiti
aliases: []
origine: UpdateVault
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Limiti Infiniti e Regolarità

## Divergenza

> [!warning] Definizione — Divergenza a $+\infty$
> Diremo che $a_n$ **diverge a $+\infty$**, e scriveremo $\lim_{n\to\infty} a_n = +\infty$, se
> $$\forall\, M>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad a_n>M$$

![[divergenza-a-piu-infinito.png]]

> [!warning] Definizione — Divergenza a $-\infty$
> Diremo che $a_n$ **diverge a $-\infty$**, e scriveremo $\lim_{n\to\infty} a_n = -\infty$, se
> $$\forall\, M>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad a_n<-M$$

![[divergenza-a-meno-infinito.png]]

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

![[convergenza-per-eccesso.png]]

$$\lim_{n\to\infty} a_n = l^- \quad\Longleftrightarrow\quad \forall\, \varepsilon>0\ \exists\, N\in\mathbb{N} : \forall\, n\geq N \quad l-\varepsilon<a_n\leq l$$

**Esempio.**
$$\lim_{n\to\infty}\left(1+\dfrac{1}{n}\right) = 1^+ \qquad \text{(per eccesso)}$$
$$\lim_{n\to\infty}\left(1-\dfrac{1}{n}\right) = 1^- \qquad \text{(per difetto)}$$

---
Precedente: [[Limite di una Successione]] · Successivo: [[Successioni Monotone]]
