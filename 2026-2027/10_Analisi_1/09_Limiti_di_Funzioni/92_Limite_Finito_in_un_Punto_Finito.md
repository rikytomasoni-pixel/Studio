---
tags:
  - AM1
  - limiti-di-funzioni
  - limite-metrico
  - limite-finito
  - definizione
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 6-8)"
---

# Limite finito in un punto finito

Quarto caso delle [[87_Definizioni_Metriche_di_Limite_all_Infinito|definizioni metriche]]: $\ell,x_0\in\mathbb{R}$.

> [!abstract] Definizione — $\displaystyle\lim_{x\to x_0}f(x)=\ell$
> $\forall\varepsilon>0\ \exists\delta>0$ tale che
> $$\begin{cases}x\in(x_0-\delta,x_0+\delta)\\ x\neq x_0\end{cases}\ \Rightarrow\ f(x)\in(\ell-\varepsilon,\ell+\varepsilon)$$
> cioè
> $$x_0-\delta<x<x_0+\delta,\ x\neq x_0\ \Rightarrow\ \ell-\varepsilon<f(x)<\ell+\varepsilon\qquad\text{ovvero}\qquad 0<|x-x_0|<\delta\ \Rightarrow\ |f(x)-\ell|<\varepsilon$$

![[LimiteFinitoFinito.png]]

> [!note] Osservazione
> Nella definizione di $\displaystyle\lim_{x\to x_0}f(x)=\ell$ con $x_0\in\mathbb{R}$ **non importa** se $f$ sia definita o meno in $x_0$, e se lo è non importa quale sia il valore $f(x_0)\in\mathbb{R}$.

> [!note] Osservazione — limiti per eccesso/difetto e da destra/sinistra
> Possiamo parlare di limiti per eccesso/difetto ($\ell^{\pm}$) e di limiti da destra/da sinistra ($x_0^{\pm}$) come nei casi precedenti:
> $$\lim_{x\to x_0^{\pm}}f(x)=\ell^{\pm}\qquad x_0,\ell\in\mathbb{R}$$
> Ad esempio $\displaystyle\lim_{x\to x_0^-}f(x)=\ell^+$ significa: $\forall\varepsilon>0\ \exists\delta>0$ tale che
> $$x_0-\delta<x<x_0\ \Rightarrow\ \ell\le f(x)<\ell+\varepsilon$$
> eccetera.

## Note collegate
- [[90_Limite_Infinito_in_un_Punto_Finito]]
- [[91_Limiti_Destro_e_Sinistro_e_Asintoto_Verticale]]
- [[93_Continuita_in_un_Punto]]
- [[88_Asintoto_Orizzontale_e_Limiti_per_Eccesso_e_per_Difetto]]
- [[86_Definizione_Topologica_di_Limite]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/limite-finito-al-punto
