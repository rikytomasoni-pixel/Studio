---
created: 2026-09-16
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/2
  - argomento/numeri_reali
aliases: []
origine: UpdateVault
---
[[00_A1_Numeri_Reali|⬅️ Torna a Numeri Reali]]

# Maggioranti, Minoranti ed Estremi

## Insiemi limitati, massimo e minimo

> [!note] Convenzione
> D'ora in poi $X = \mathbb{R}$ oppure $\mathbb{Q}$. Consideriamo sempre $E\subseteq X$ non vuoto.

### Insiemi limitati

> [!warning] Definizione — Limitatezza
> Dato $E\subseteq X$ non vuoto, $E$ si dice:
> - **limitato dall'alto** (o superiormente) se $\exists\, k\in X$ tale che
> $$x\leq k \qquad \forall\, x\in E$$
> - **limitato dal basso** (o inferiormente) se $\exists\, h\in X$ tale che
> $$h\leq x \qquad \forall\, x\in E$$
> - **limitato** se è limitato sia dall'alto che dal basso, cioè se $\exists\, h,k\in X$ tali che
> $$h\leq x\leq k \qquad \forall\, x\in E$$

### Massimo e minimo

> [!warning] Definizione — Massimo e minimo
> Dato $E\subseteq X$ non vuoto, $x_0\in X$ si dice **massimo** di $E$, e scriviamo $x_0=\max E$, se:
> - $x_0\in E$
> - $x\leq x_0\ \ \forall\, x\in E$
>
> Dato $E\subseteq X$ non vuoto, $x_1\in X$ si dice **minimo** di $E$, e scriviamo $x_1=\min E$, se:
> - $x_1\in E$
> - $x_1\leq x\ \ \forall\, x\in E$

**Osservazione.** Condizione *necessaria* affinché esistano $\max E$ / $\min E$ è che $E$ sia limitato dall'alto/dal basso rispettivamente — ma **non è sufficiente**.

### Esempi

**Esempio.** $E=\mathbb{N}$: limitato dal basso, non limitato dall'alto.
$$\min \mathbb{N} = 0, \qquad \nexists\, \max \mathbb{N}$$

**Esempio.** $E=\left\{\dfrac{1}{n} : n\in\mathbb{N},\ n\neq 0\right\} = \left\{1,\ \dfrac{1}{2},\ \dfrac{1}{3},\ \dfrac{1}{4},\ \dots\right\}$

$E$ è limitato, $\max E = 1$, $\nexists\, \min E$.

**Osservazione.** $\max E$ / $\min E$ non sempre esistono, anche quando $E$ è limitato.

## Maggioranti e minoranti

> [!warning] Definizione — Maggiorante e minorante
> Dato $E\subseteq X$ non vuoto e $k\in X$ (non necessariamente $k\in E$), $k$ si dice **maggiorante** di $E$ se
> $$x\leq k \qquad \forall\, x\in E$$
> Dato $E\subseteq X$ non vuoto e $h\in X$ (non necessariamente $h\in E$), $h$ si dice **minorante** di $E$ se
> $$h\leq x \qquad \forall\, x\in E$$

**Osservazioni.**
- Esistono maggioranti/minoranti se e solo se l'insieme è limitato dall'alto/dal basso.
- Se $h$ è minorante di $E$, anche ogni $b\leq h$ è minorante di $E$.
- Se $k$ è maggiorante di $E$, anche ogni $a\geq k$ è maggiorante di $E$.
- Se $k$ è maggiorante di $E$ e $k\in E$, allora $k=\max E$.
- Se $h$ è minorante di $E$ e $h\in E$, allora $h=\min E$.

### Esempi

**Esempio.** $E=\mathbb{N}$: $0=\min E$; ogni $h\leq 0$ è minorante; $\nexists$ maggioranti.

**Esempio.** $E=\left\{\dfrac{1}{n}:n\in\mathbb{N},\ n\neq 0\right\}$: ogni $h\leq 0$ è minorante, $\nexists\, \min E$; ogni $k\geq 1$ è maggiorante, $\max E = 1$.

**Esempio.** $E=\{r\in\mathbb{Q} : r\geq 0,\ r^2\leq 2\}\subset \mathbb{R}$: ogni $h\leq 0$ è minorante, $\min E = 0$; ogni $k\geq \sqrt{2}$ è maggiorante, $\nexists\, \max E$ (infatti $\sqrt 2 \notin E$).

## Estremo superiore e inferiore

> [!warning] Definizione — Estremo superiore e inferiore
> Sia $E\subseteq X$ non vuoto.
> - Se esistono maggioranti di $E$ (cioè $E$ è limitato dall'alto), chiamiamo **estremo superiore** di $E$, $\sup E$, il *minimo tra i maggioranti* di $E$ (se esiste).
> - Se esistono minoranti di $E$ (cioè $E$ è limitato dal basso), chiamiamo **estremo inferiore** di $E$, $\inf E$, il *massimo tra i minoranti* di $E$ (se esiste).

**Osservazione.** $\sup E$ è il migliore dei maggioranti (il più piccolo); $\inf E$ è il migliore dei minoranti (il più grande).

### Esempi

**Esempio.** $E=\mathbb{N}$: $\nexists\, \sup \mathbb{N}$ in $X$; $\inf E = 0 = \min E$.
> *(vedremo più avanti che $\sup \mathbb{N} = +\infty$)*

**Esempio.** $E=\left\{\dfrac{1}{n}:n\in\mathbb{N},\ n\neq 0\right\}$: $\max E = 1 = \sup E$; $\nexists\, \min E$, $\inf E = 0$.

**Esempio.** $E=\{r\in\mathbb{Q}: r^2\leq 2,\ r\geq 0\}$:
- come sottoinsieme di $\mathbb{R}$: $\min E = \inf E = 0$, $\nexists\, \max E$, $\sup E = \sqrt{2}$;
- come sottoinsieme di $\mathbb{Q}$: $\min E = \inf E = 0$, $\nexists\, \max E$, $\nexists\, \sup E$ **(in $\mathbb{Q}$!)**.

---
Precedente: [[Campi Ordinati]] · Successivo: [[Assioma di Completezza]]
