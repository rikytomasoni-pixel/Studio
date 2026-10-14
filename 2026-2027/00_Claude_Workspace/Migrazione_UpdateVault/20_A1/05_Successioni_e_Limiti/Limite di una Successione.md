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

# Limite di una Successione

## Convergenza

> [!warning] Definizione — Convergenza
> Diremo che una successione $a_n$ **converge** a $l\in\mathbb{R}$, e scriveremo
> $$\lim_{n\to\infty} a_n = l$$
> se $\forall\, \varepsilon>0\ \exists\, N\in\mathbb{N}$ tale che
> $$\forall\, n\geq N \quad |a_n-l|<\varepsilon \qquad (l-\varepsilon<a_n<l+\varepsilon)$$

![[definizione-limite-successione-striscia-epsilon.png]]

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

![[unicita-limite-intorni-disgiunti.png]]

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

---
Precedente: [[Successioni Limitate e Definitivamente]] · Successivo: [[Limiti Infiniti e Regolarità]]
