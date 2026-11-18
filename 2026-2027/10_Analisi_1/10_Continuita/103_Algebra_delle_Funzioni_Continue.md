---
tags:
  - AM1
  - continuita
  - algebra-delle-funzioni-continue
  - teorema
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 2-3)"
---

# Algebra delle funzioni continue

> [!abstract] Teorema
> Se $f,g$ sono continue in $x_0\in\mathbb{R}$, cioè
> $$\lim_{x\to x_0}f(x)=f(x_0),\qquad\lim_{x\to x_0}g(x)=g(x_0)$$
> allora
> 1. $\displaystyle\lim_{x\to x_0}\big(f(x)\pm g(x)\big)=f(x_0)\pm g(x_0)$, cioè $f\pm g$ è continua in $x_0$
> 2. $\displaystyle\lim_{x\to x_0}\big(f(x)\cdot g(x)\big)=f(x_0)\cdot g(x_0)$, cioè $f\cdot g$ è continua in $x_0$
> 3. $\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=\frac{f(x_0)}{g(x_0)}$ se $g(x_0)\neq0$, cioè $f/g$ è continua in $x_0$
> 4. $\displaystyle\lim_{x\to x_0}\big(f(x)\big)^\alpha=\big(f(x_0)\big)^\alpha$, $\alpha\in\mathbb{R}$ (se $(f(x))^\alpha$ è ben definita in un intorno $\mathcal{U}(x_0)$ di $x_0$), cioè $f^\alpha$ è continua in $x_0$

**Dimostrazione.** Segue immediatamente dal teorema sull'algebra dei limiti ([[102_Algebra_dei_Limiti_di_Funzioni]]) perché esistono i limiti
$$\ell_1=\lim_{x\to x_0}f(x)=f(x_0)\in\mathbb{R},\qquad\ell_2=\lim_{x\to x_0}g(x)=g(x_0)\in\mathbb{R}\qquad\square$$

## Note collegate
- [[93_Continuita_in_un_Punto]]
- [[105_Continuita_della_Funzione_Composta]]
- [[117_Continuita_delle_Funzioni_Elementari]]
- [[00_MOC_Analisi_1]]
- [[131_Algebra_delle_Derivate]] (versione per le derivate)

#AM1/continuita/algebra-funzioni-continue
