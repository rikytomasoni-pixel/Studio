---
tags:
  - AM1
  - limiti-di-funzioni
  - unicita-del-limite
  - teorema
  - dimostrazione
data: 2026-10-23
fonte: "AM1 L13 26-27.pdf (pag. 6-7)"
---

# Teorema di unicità del limite

> [!abstract] Teorema (di unicità del limite)
> Data $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in\overline{\mathbb{R}}$ punto di accumulazione per $I$. Se esiste
> $$\lim_{x\to x_0}f(x)=\ell\in\overline{\mathbb{R}}$$
> allora tale limite è **unico**.

## Dimostrazione
Per assurdo, esistono $\ell_1,\ell_2\in\overline{\mathbb{R}}$ con $\ell_1\neq\ell_2$ e
$$\lim_{x\to x_0}f(x)=\ell_1,\qquad\lim_{x\to x_0}f(x)=\ell_2$$
Allora, per ogni successione $\{x_n\}\subset I$ tale che $x_n\neq x_0$ $\forall n\geq1$ e con $\displaystyle\lim_{n\to\infty}x_n=x_0$, deve essere contemporaneamente
$$\lim_{n\to\infty}f(x_n)=\ell_1\qquad\text{e}\qquad\lim_{n\to\infty}f(x_n)=\ell_2\qquad\text{con }\ell_1\neq\ell_2$$
Assurdo per l'unicità del limite per successioni ([[30_Limiti_di_Successioni]]). $\square$

## Note collegate
- [[84_Definizione_Successionale_di_Limite]]
- [[86_Definizione_Topologica_di_Limite]]
- [[30_Limiti_di_Successioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/unicita-del-limite
