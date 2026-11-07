---
tags:
  - AM1
  - continuita
  - esempio
  - dirichlet
  - discontinuita
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 11-12)"
---

# Funzione di Dirichlet

$$f(x)=\begin{cases}0&x\in\mathbb{R}\setminus\mathbb{Q}\\ 1&x\in\mathbb{Q}\end{cases}$$

**Affermazione.** $\forall x_0\in\overline{\mathbb{R}}$ **non esiste** $\displaystyle\lim_{x\to x_0}f(x)$. In particolare $f$ è discontinua in $x_0$, $\forall x_0\in\mathbb{R}$.

**Dimostrazione** (con la [[84_Definizione_Successionale_di_Limite|definizione successionale]]). Se $x_0\in\overline{\mathbb{R}}$ possiamo trovare due successioni $x_n,z_n$ tali che

1. $z_n\neq x_0,\ x_n\neq x_0\quad\forall n\ge1$
2. $z_n\in\mathbb{R}\setminus\mathbb{Q},\ x_n\in\mathbb{Q}\quad\forall n\ge1$
3. $\displaystyle\lim_{n\to\infty}z_n=\lim_{n\to\infty}x_n=x_0$

(questo è possibile perché $\mathbb{Q}$ e $\mathbb{R}\setminus\mathbb{Q}$ sono **densi** in $\mathbb{R}$).

Allora $f(x_n)=1$ e $f(z_n)=0$ $\ \forall n\ge1$, quindi
$$\lim_{n\to\infty}f(x_n)=1\ \neq\ 0=\lim_{n\to\infty}f(z_n)\ \Rightarrow\ \nexists\lim_{x\to x_0}f(x)\quad\forall x_0\in\overline{\mathbb{R}}$$

## Note collegate
- [[93_Continuita_in_un_Punto]]
- [[84_Definizione_Successionale_di_Limite]]
- [[85_Teorema_di_Unicita_del_Limite]]
- [[98_Discontinuita_di_Seconda_Specie]]
- [[00_MOC_Analisi_1]]

#AM1/continuita/dirichlet
