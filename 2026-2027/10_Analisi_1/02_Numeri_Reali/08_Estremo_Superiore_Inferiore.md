---
tags:
  - AM1
  - estremo-superiore
  - estremo-inferiore
  - maggioranti
  - minoranti
  - assioma-di-continuita
data: 2026-09-16
fonte: Lezione 2
---

# Maggioranti, minoranti, estremo superiore e inferiore

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

## Proprietà dell'estremo superiore (assioma di continuità)

> [!warning] Definizione — Proprietà dell'estremo superiore/inferiore
> $X$ soddisfa la **proprietà dell'estremo superiore** (inferiore) se ogni sottoinsieme $E\subseteq X$ non vuoto e limitato dall'alto (dal basso) possiede estremo superiore $\sup E\in X$ (estremo inferiore $\inf E \in X$).

> [!abstract] Teorema — Assiomatica di $\mathbb{R}$
> $\mathbb{R}$ è l'**unico** campo ordinato che soddisfa la proprietà dell'estremo superiore (equivalentemente, dell'estremo inferiore).

**Osservazione.** La proprietà dell'estremo superiore (inferiore), nella definizione assiomatica di $\mathbb{R}$, prende il nome di **assioma di continuità**.

## $\mathbb{Q}$ non soddisfa la proprietà dell'estremo superiore

$$E = \{r\in\mathbb{Q} : r\geq 0,\ r^2\leq 2\} \subset \mathbb{Q}, \qquad \nexists\, \sup E \text{ in } \mathbb{Q}$$

**Osservazioni.**
- Dato $E\subseteq \mathbb{R}$, se esiste $\max E$ / $\min E$ allora $\max E = \sup E$ / $\min E = \inf E$.
- Dato $E\subseteq \mathbb{R}$ non vuoto e limitato dall'alto/dal basso, sicuramente esiste in $\mathbb{R}$ $\sup E$ / $\inf E$. Se inoltre $\sup E \in E$ / $\inf E \in E$, allora $\sup E = \max E$ / $\inf E = \min E$.

## $\mathbb{R}$ esteso: $\sup E = +\infty$, $\inf E = -\infty$

> [!warning] Definizione
> Se $E\subseteq \mathbb{R}$ è un insieme:
> - **illimitato dall'alto**, scriveremo $\sup E = +\infty$;
> - **illimitato dal basso**, scriveremo $\inf E = -\infty$.

**Osservazione.** Dato $E\subseteq \mathbb{R}$ non vuoto, esistono sempre $\sup E, \inf E$ in
$$\overline{\mathbb{R}} = \mathbb{R}\cup\{+\infty\}\cup\{-\infty\}$$
e $\sup E / \inf E \in \mathbb{R}$ se e solo se $E$ è limitato dall'alto/dal basso.

## Caratterizzazione di $\sup$ e $\inf$

**Osservazione.** Sia $E\subseteq \mathbb{R}$ non vuoto e limitato dall'alto. $x_0\in\mathbb{R}$ è $\sup E$ se:

1. $x\leq x_0\ \ \forall\, x\in E$  ($x_0$ è maggiorante di $E$)
2. $\forall\, k<x_0\ \ \exists\, x\in E: \ k<x\leq x_0$
   *(ogni $k<x_0$ non è maggiorante di $E$, cioè $x_0$ è il più piccolo maggiorante)*

Sia $E\subseteq \mathbb{R}$ non vuoto e limitato dal basso. $x_1\in\mathbb{R}$ è $\inf E$ se:

1. $x_1\leq x\ \ \forall\, x\in E$  ($x_1$ è minorante di $E$)
2. $\forall\, h>x_1\ \ \exists\, x\in E: \ x_1\leq x<h$
   *(ogni $h>x_1$ non è minorante di $E$, cioè $x_1$ è il più grande minorante)*

### Note collegate
- [[00_MOC_Analisi_1]]
- [[07_Insiemi_Limitati_Max_Min]] — insiemi limitati, massimo e minimo
- [[06_Campi_Ordinati]] — campo ordinato
- [[04_Dimostrazione_per_Assurdo]] — $\nexists\, x\in\mathbb{Q}: x^2=2$
- [[10_Retta_Reale_Intervalli]] — $\sup$ e $\inf$ degli intervalli
- [[20_Funzioni_Limitate_Estremi]] — $\sup$ e $\inf$ di una funzione

#AM1/numeri-reali/estremo-superiore-inferiore
