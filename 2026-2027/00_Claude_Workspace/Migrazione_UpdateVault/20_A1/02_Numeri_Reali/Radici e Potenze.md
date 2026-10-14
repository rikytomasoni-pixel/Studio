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

# Radici e Potenze

## Radice n-esima

> [!abstract] Teorema — Esistenza e unicità della radice n-esima
> Sia $y\in\mathbb{R}$, $y\geq 0$, $n\geq 1$. Allora $\exists!\, x\in\mathbb{R}$ tale che
> $$x\geq 0 \quad \text{e} \quad x^n = y$$
> *(segue dal fatto che la funzione $f:[0,\infty)\to[0,\infty)$, $f(t)=t^n\ \forall\, t\geq 0$, è monotona strettamente crescente, continua, con $f(0)=0$ e $\displaystyle\lim_{t\to\infty} f(t) = +\infty$)*

> [!warning] Definizione — Radice n-esima
> Il numero reale $x$ di cui sopra si chiama **radice $n$-esima** di $y$:
> $$x = \sqrt[n]{y} = y^{1/n}$$

**Osservazione.**
$$\sqrt[2]{4} = 2 \qquad \left(\text{NON } \sqrt[2]{4}=\pm 2,\ \text{sbagliato in } \mathbb{R}\right)$$

**Osservazioni.**
$$\sqrt[2]{a^2} = |a| \qquad \forall\, a\in\mathbb{R}$$
$$\sqrt[n]{y} \geq 0 \qquad \forall\, y\in\mathbb{R},\ y\geq 0,\ \forall\, n\in\mathbb{N},\ n\geq 1$$
$$\sqrt[n]{a^n} = a \qquad \forall\, a\geq 0,\ a\in\mathbb{R}$$

## Potenze con esponente razionale

> [!warning] Definizione — Potenze con esponente $\geq 0$
> $\forall\, a>0$, $\forall\, m,n\in\mathbb{N}$, $n\neq 0$, definiamo:
> $$a^0 = 1$$
> $$a^m = \underbrace{a\cdot a \cdots a}_{m \text{ volte}}$$
> $$a^{1/n} = \sqrt[n]{a}$$
> $$a^{m/n} = \left(a^m\right)^{1/n}$$

**Osservazione.** $a^r\in\mathbb{R}$ è ben definita $\forall\, a\in\mathbb{R}, a>0$ e $\forall\, r\in\mathbb{Q}, r\geq 0$.

> [!warning] Definizione — Potenze con esponente negativo
> $\forall\, a\in\mathbb{R}, a>0$, definiamo $a^{-1} = \dfrac{1}{a}$, e $\forall\, m,n\in\mathbb{N}$, $n\neq 0$:
> $$a^{-m} = \underbrace{a^{-1}\cdots a^{-1}}_{m \text{ volte}} = \left(a^{-1}\right)^m$$
> $$a^{-1/n} = \left(a^{1/n}\right)^{-1} = \dfrac{1}{a^{1/n}}$$
> $$a^{-m/n} = \left(a^{m/n}\right)^{-1} = \dfrac{1}{a^{m/n}}$$

**Osservazione.** Con quanto visto, $a^r\in\mathbb{R}$ è ben definita $\forall\, a\in\mathbb{R}, a>0$, $\forall\, r\in\mathbb{Q}$.

## Potenze con esponente reale qualsiasi

**Domanda:** come definire $a^b$, $\forall\, a\in\mathbb{R}, a>0$ e $\forall\, b\in\mathbb{R}$ (esponente reale, non necessariamente razionale)?

Cominciamo osservando che se $b\in\mathbb{R}$ allora
$$b = \pm\, b_0,b_1b_2b_3\ldots b_k \ldots$$
con $b_0\in\mathbb{N}$, $b_k\in\{0,1,\ldots,9\}\ \ \forall\, k\in\mathbb{N}, k\geq 1$ — l'**espansione decimale** di $b$.

Consideriamo i numeri razionali ottenuti troncando l'espansione decimale:
$$\pm b_0 \in \mathbb{Q}, \quad \pm b_0,b_1 \in \mathbb{Q}, \quad \pm b_0,b_1b_2 \in \mathbb{Q}, \quad \ldots, \quad \pm b_0,b_1b_2b_3\ldots b_k \in \mathbb{Q}, \quad \ldots$$

e corrispondentemente calcoliamo
$$a^{\pm b_0},\quad a^{\pm b_0,b_1},\quad a^{\pm b_0,b_1b_2},\quad \ldots,\quad a^{\pm b_0,b_1b_2b_3\ldots b_k},\quad \ldots$$

che sono ben definiti dalle definizioni viste sopra, poiché $\pm b_0,b_1b_2b_3\ldots b_k \in \mathbb{Q}\ \ \forall\, k\in\mathbb{N}$.

**Idea:** si definisce
$$a^b = \lim_{k\to\infty} a^{\pm b_0,b_1b_2b_3\ldots b_k} \ \in \mathbb{R}$$

Si dimostra che $a^b$ può essere caratterizzato come
$$a^b = \sup\left\{ a^{\pm b_0,b_1b_2b_3\ldots b_k} : k\in\mathbb{N}\right\} \in \mathbb{R}$$
oppure come
$$a^b = \inf\left\{ a^{\pm b_0,b_1b_2b_3\ldots b_k} : k\in\mathbb{N}\right\} \in \mathbb{R}$$
a seconda che i valori della successione $a^{\pm b_0,b_1b_2b_3\ldots b_k}$ siano crescenti o decrescenti.

Si dimostra che questa procedura produce un numero reale ben definito, che si denota con $a^b$.

**Osservazioni.**
- $a^b$ è definito $\forall\, a\in\mathbb{R}, a>0$, $\forall\, b\in\mathbb{R}$, e vale $a^b>0$.
- $a^b$ può essere definito anche per valori $a\leq 0$ se $b\in\mathbb{R}$ è particolare (ad esempio se $b\in\mathbb{N}$), ma ciò **non è possibile per tutti** i $b\in\mathbb{R}$.

> [!warning] Da fare
> Proprietà delle potenze: vedere sul libro di testo — **da sapere**.

---
Precedente: [[Densità di Q in R]] · Successivo: [[Logaritmi]]
