---
tags:
  - AM1
  - limiti-di-funzioni
  - limite-metrico
  - limiti-all-infinito
  - definizione
data: 2026-10-23
fonte: "AM1 L13 26-27.pdf (pag. 10-15)"
---

# Definizioni metriche di limite all'infinito

Specificando la forma esplicita degli intorni $\mathcal{U}(\ell)$, $\mathcal{U}(x_0)$ ([[82_Intorni_di_un_Punto_e_di_Infinito]]), nei casi $x_0,\ell\in\mathbb{R}\cup\{+\infty\}\cup\{-\infty\}$, si trovano le **definizioni metriche** di limite (a partire dalla [[86_Definizione_Topologica_di_Limite]]).

## 1) Limite finito all'infinito ($x_0=\pm\infty$, $\ell\in\mathbb{R}$)

> [!abstract] $\displaystyle\lim_{x\to+\infty}f(x)=\ell$
> $\forall\varepsilon>0\ \exists M>0$ tale che
> $$x>M\ \Rightarrow\ f(x)\in(\ell-\varepsilon,\ell+\varepsilon)\quad\text{cioè}\quad\ell-\varepsilon<f(x)<\ell+\varepsilon\quad\text{cioè}\quad|f(x)-\ell|<\varepsilon$$
![[LimiteFinitoInfinito.png]]

> [!abstract] $\displaystyle\lim_{x\to-\infty}f(x)=\ell$
> $\forall\varepsilon>0\ \exists M>0$ tale che
> $$x<-M\ \Rightarrow\ f(x)\in(\ell-\varepsilon,\ell+\varepsilon)\quad\text{cioè}\quad|f(x)-\ell|<\varepsilon$$
> ![[LimiteFinito-Inf.png]]


> [!example] Esempi
> $$\lim_{x\to+\infty}e^{-x}=0\qquad\qquad\lim_{x\to-\infty}\frac1x=0$$

## 2) Limite infinito all'infinito ($x_0=\pm\infty$, $\ell=\pm\infty$)

> [!abstract] $\displaystyle\lim_{x\to+\infty}f(x)=+\infty$
> $\forall M>0\ \exists K>0$ tale che $\quad x>K\ \Rightarrow\ f(x)>M$
> ![[LimiteInfInf.png]]

> [!abstract] $\displaystyle\lim_{x\to+\infty}f(x)=-\infty$
> $\forall M>0\ \exists K>0$ tale che $\quad x>K\ \Rightarrow\ f(x)<-M$
> ![[LimInf-Inf.png]]

Similmente per $\displaystyle\lim_{x\to-\infty}f(x)=+\infty$ e $\displaystyle\lim_{x\to-\infty}f(x)=-\infty$.



> [!example] Esempi
> $$\lim_{x\to-\infty}e^{-x}=+\infty\qquad\qquad\lim_{x\to+\infty}\log x=+\infty$$

## Note collegate
- Prosegue con [[90_Limite_Infinito_in_un_Punto_Finito]] e [[92_Limite_Finito_in_un_Punto_Finito]] (L14)
- [[86_Definizione_Topologica_di_Limite]]
- [[88_Asintoto_Orizzontale_e_Limiti_per_Eccesso_e_per_Difetto]]
- [[89_Asintoto_Obliquo]]
- [[30_Limiti_di_Successioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/definizioni-metriche
