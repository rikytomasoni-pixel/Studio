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

# Assioma di Completezza

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

---
Precedente: [[Maggioranti, Minoranti ed Estremi]] · Successivo: [[Valore Assoluto]]
