---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - criterio-del-confronto
  - teorema
  - dimostrazione
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 5-8)"
---

# Criterio del confronto per serie a termini positivi

> [!abstract] Teorema — Criterio del confronto
> Date due successioni $a_n,b_n$ tali che (definitivamente in $n\in\mathbb{N}$)
> $$0\leq a_n\leq b_n\qquad\forall n\in\mathbb{N}$$
> Allora:
> 1. se $\displaystyle\sum_{n=1}^\infty a_n$ diverge a $+\infty$, allora anche $\displaystyle\sum_{n=1}^\infty b_n$ diverge a $+\infty$;
> 2. se $\displaystyle\sum_{n=1}^\infty b_n$ converge, allora anche $\displaystyle\sum_{n=1}^\infty a_n$ converge.
>
> Inoltre, se $a_n\leq b_n$ per ogni $n\in\mathbb{N}$, allora
> $$\sum_{n=1}^\infty a_n\leq\sum_{n=1}^\infty b_n$$

## Dimostrazione
Per semplicità supponiamo che
$$(*)\qquad 0\leq a_n\leq b_n\qquad\forall n\in\mathbb{N},\ n\geq1$$
Consideriamo le somme parziali
$$S_N=\sum_{n=1}^N a_n\qquad\qquad\sigma_N=\sum_{n=1}^N b_n$$
Da $(*)$ segue che per ogni $N\in\mathbb{N}$, $N\geq1$,
$$0\leq S_N\leq\sigma_N$$
Poiché $S_N,\sigma_N$ sono crescenti, esistono (vedi [[57_Serie_a_Termini_Positivi]])
$$S=\lim_{N\to\infty}S_N,\qquad\sigma=\lim_{N\to\infty}\sigma_N\qquad\text{con }S,\sigma\in\mathbb{R}\cup\{+\infty\}$$

**1)** Se $\sum a_n$ diverge, allora $S=\sum_{n=1}^\infty a_n=\lim_{N\to\infty}S_N=+\infty$. Poiché $\sigma_N\geq S_N$ per ogni $N\geq1$, per il teorema del confronto per successioni divergenti ([[35_Teoremi_del_Confronto]]) deve essere
$$\sum_{n=1}^\infty b_n=\lim_{N\to\infty}\sigma_N=+\infty$$
cioè $\sum b_n$ diverge.

**2)** Se $\sum b_n$ converge, $\displaystyle\sum_{n=1}^\infty b_n=\lim_{N\to\infty}\sigma_N=\sigma\in\mathbb{R}$. Essendo $\sigma_N$ crescente,
$$\sigma=\sup_{N\in\mathbb{N}}\sigma_N\geq\sigma_N$$
Allora per ogni $N\geq1$
$$S_N\leq\sigma_N\leq\sigma\in\mathbb{R}$$
$\Rightarrow S_N$, che è crescente, è **limitata** $\Rightarrow\exists\lim_{N\to\infty}S_N=S\in\mathbb{R}$, cioè $\sum a_n=\lim S_N=S\in\mathbb{R}$ converge.

**3)** Essendo $\sigma_N\geq S_N$ per ogni $N\geq1$ e poiché esistono $\lim\sigma_N=\sigma$, $\lim S_N=S$ in $\mathbb{R}\cup\{+\infty\}$, per la permanenza del segno ([[33_Teorema_Permanenza_del_Segno]])
$$S=\lim_{N\to\infty}S_N\leq\lim_{N\to\infty}\sigma_N=\sigma\ \Rightarrow\ \sum_{n=1}^\infty a_n=S\leq\sigma=\sum_{n=1}^\infty b_n\qquad\square$$

## Esempi
- [[59_Esempio_Confronto_Serie_18_cos_n]]
- Serie di riferimento da usare come $b_n$: [[50_Serie_Geometrica]], [[60_Serie_Armonica_Generalizzata]], [[61_Serie_di_Bertrand_Generalizzata]]

## Note collegate
- [[57_Serie_a_Termini_Positivi]]
- [[62_Criterio_del_Confronto_Asintotico_per_Serie]]
- [[35_Teoremi_del_Confronto]]
- [[00_MOC_Analisi_1]]

#AM1/serie/criterio-del-confronto
