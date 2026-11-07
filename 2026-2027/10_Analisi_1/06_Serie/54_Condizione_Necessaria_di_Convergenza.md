---
tags:
  - AM1
  - serie
  - teorema
  - condizione-necessaria
  - dimostrazione
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 18-19)"
---

# Condizione necessaria affinché una serie converga

> [!abstract] Teorema (condizione necessaria affinché una serie converga)
> Se $\displaystyle\sum_{n=0}^\infty a_n$ converge, allora $\displaystyle\lim_{n\to\infty}a_n=0$.

> [!abstract] Corollario
> Se $\lim_{n\to\infty}a_n$ non esiste, o se $\exists\lim_{n\to\infty}a_n=\ell\in\overline{\mathbb{R}}$ ma $\ell\neq0$, allora la serie $\sum_{n=0}^\infty a_n$ **non converge**.

## Dimostrazione (del teorema)
Sia $S_N=\sum_{n=0}^Na_n$ la successione delle somme parziali di $a_n$. Per ipotesi
$$\exists\,S=\lim_{N\to\infty}S_N\in\mathbb{R}$$
Osserviamo che
$$S_N=\sum_{n=0}^Na_n=\sum_{n=0}^{N-1}a_n+a_N=S_{N-1}+a_N\ \Rightarrow\ a_N=S_N-S_{N-1}\qquad\forall N\geq1$$
Poiché $\lim_{N\to\infty}S_N=\lim_{N\to\infty}S_{N-1}=S\in\mathbb{R}$, per l'algebra dei limiti ([[34_Algebra_dei_Limiti]])
$$\lim_{N\to\infty}a_N=\lim_{N\to\infty}(S_N-S_{N-1})=\lim_{N\to\infty}S_N-\lim_{N\to\infty}S_{N-1}=S-S=0$$
$$\Rightarrow\lim_{N\to\infty}a_N=0\qquad\square$$

> [!danger] Attenzione
> Se $\lim_{n\to\infty}a_n=0$, **non necessariamente** $\sum_{n=0}^\infty a_n$ converge.
> Esempio: la **serie armonica** $\sum_{n=1}^\infty\frac1n$ ha $\lim_{n\to\infty}\frac1n=0$ ma $\sum_{n=1}^\infty\frac1n=+\infty$ (controesempio, vedi [[55_Serie_Armonica]]).

Applicazione al corollario: la serie $\sum(-1)^n$ ([[49_Esempi_Elementari_di_Serie]]) non converge perché $(-1)^n$ non ha limite.

## Note collegate
- [[55_Serie_Armonica]]
- [[48_Studio_del_Carattere_di_una_Serie]]
- [[49_Esempi_Elementari_di_Serie]]
- [[34_Algebra_dei_Limiti]]
- [[00_MOC_Analisi_1]]

#AM1/serie/condizione-necessaria-di-convergenza
