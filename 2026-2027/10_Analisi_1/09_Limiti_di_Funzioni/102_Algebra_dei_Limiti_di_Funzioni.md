---
tags:
  - AM1
  - limiti-di-funzioni
  - algebra-dei-limiti
  - forme-indeterminate
  - teorema
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 22-23)"
---

# Algebra dei limiti e aritmetizzazione parziale di infinito (per funzioni)

> [!abstract] Teorema
> Se esistono $\displaystyle\lim_{x\to x_0}f(x)=\ell_1$, $\displaystyle\lim_{x\to x_0}g(x)=\ell_2$ con $x_0,\ell_1,\ell_2\in\overline{\mathbb{R}}$, allora
> 1. $\displaystyle\lim_{x\to x_0}\big(f(x)\pm g(x)\big)=\ell_1\pm\ell_2$
> 2. $\displaystyle\lim_{x\to x_0}\big(f(x)\cdot g(x)\big)=\ell_1\cdot\ell_2$
> 3. $\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=\frac{\ell_1}{\ell_2}$ *(serve $g(x)\neq0$ definitivamente per $x\to x_0$)*
> 4. $\displaystyle\lim_{x\to x_0}\big(f(x)\big)^{g(x)}=\ell_1^{\ell_2}$ *(serve $f(x)>0$ in un intorno $\mathcal{U}(x_0)$ di $x_0$, salvo al più in $x_0$)*
> 5. $\displaystyle\lim_{x\to x_0}\big(f(x)\big)^{\alpha}=\ell_1^{\alpha}$, $\alpha\in\mathbb{R}$ *(serve che $(f(x))^\alpha$ sia definita in un intorno $\mathcal{U}(x_0)$ di $x_0$, salvo al più in $x_0$)*
>
> con la stessa aritmetizzazione di $\infty$ vista per le successioni, a meno delle **forme di indeterminazione**
> $$[\infty-\infty],\ [0\cdot\infty],\ \Big[\tfrac00\Big],\ \Big[\tfrac\infty\infty\Big],\ [1^{\pm\infty}],\ [\infty^0],\ [0^0]$$
> o del caso $\Big[\dfrac{\ell_1}{0}\Big]$ con $\ell_1\in\overline{\mathbb{R}}\setminus\{0\}$ e $\ell_2=0$ (senza segno).

## Note collegate
- [[34_Algebra_dei_Limiti]] e [[37_Algebra_Limiti_Infiniti]] (successioni)
- [[103_Algebra_delle_Funzioni_Continue]] (caso di funzioni continue)
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/algebra-dei-limiti
