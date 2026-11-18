---
tags:
  - AM1
  - limiti-di-funzioni
  - teorema-del-confronto
  - carabinieri
  - teorema
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 19-21)"
---

# Teoremi del confronto per limiti di funzioni

> [!abstract] Teorema del confronto (due carabinieri)
> Se $x_0\in\overline{\mathbb{R}}$, $f,g,h:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0$ punto di accumulazione per $I$, $\ell\in\mathbb{R}$.
> Se $\exists\displaystyle\lim_{x\to x_0}f(x)=\lim_{x\to x_0}h(x)=\ell$ ed inoltre definitivamente per $x\to x_0$ vale
> $$f(x)\le g(x)\le h(x)$$
> allora $\exists\displaystyle\lim_{x\to x_0}g(x)=\ell$.

> [!abstract] Teorema del confronto (per limiti infiniti)
> Se $x_0\in\overline{\mathbb{R}}$, $f,g:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0$ punto di accumulazione per $I$ e definitivamente per $x\to x_0$ vale $f(x)\le g(x)$, allora
> 1. se $\displaystyle\lim_{x\to x_0}f(x)=+\infty$, anche $\displaystyle\lim_{x\to x_0}g(x)=+\infty$
> 2. se $\displaystyle\lim_{x\to x_0}g(x)=-\infty$, anche $\displaystyle\lim_{x\to x_0}f(x)=-\infty$
>
> *(senza dimostrazione: si può dimostrare come i corrispondenti teoremi per le successioni)*

> [!note] Osservazione
> I teoremi di confronto valgono anche per $\displaystyle\lim_{x\to x_0^+}f(x)$ e per $\displaystyle\lim_{x\to x_0^-}f(x)$, limiti da destra e da sinistra rispettivamente.

> [!abstract] Corollario
> Se $\displaystyle\lim_{x\to x_0}g(x)=0$, con $x_0\in\overline{\mathbb{R}}$, e se $|f(x)|\le g(x)$ definitivamente per $x\to x_0$, allora $\exists\displaystyle\lim_{x\to x_0}f(x)=0$.
>
> *(segue dal teorema dei due carabinieri come per le successioni)*

> [!abstract] Corollario
> Se $\exists\displaystyle\lim_{x\to x_0}g(x)=0$, $x_0\in\overline{\mathbb{R}}$, e se $h(x)$ è limitata definitivamente per $x\to x_0$, allora
> $$\exists\lim_{x\to x_0}g(x)\cdot h(x)=0$$
> *(come per le successioni)*

> [!example] Esempi
> $$\lim_{x\to\infty}\frac{\sin x}{x}=0\qquad\qquad\lim_{x\to0}x^7\sin\frac1x=0$$

## Note collegate
- [[35_Teoremi_del_Confronto]] (versione per successioni)
- [[99_Proprieta_Valida_Definitivamente]]
- [[101_Teorema_di_Permanenza_del_Segno_per_Funzioni]]
- [[102_Algebra_dei_Limiti_di_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/teorema-del-confronto
