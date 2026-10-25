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

> [!abstract] $\displaystyle\lim_{x\to-\infty}f(x)=\ell$
> $\forall\varepsilon>0\ \exists M>0$ tale che
> $$x<-M\ \Rightarrow\ f(x)\in(\ell-\varepsilon,\ell+\varepsilon)\quad\text{cioè}\quad|f(x)-\ell|<\varepsilon$$

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** pag. 10 (per $+\infty$) e pag. 11 (per $-\infty$). **Cosa cercare:** grafico di una funzione che oscilla e si avvicina alla retta orizzontale $y=\ell$ (in rosso) restando, da un certo punto in poi, nella fascia tra $y=\ell-\varepsilon$ e $y=\ell+\varepsilon$ (linee azzurre tratteggiate). Per $+\infty$ la soglia $M$ è segnata a destra sull'asse $x$ (in verde); per $-\infty$ la soglia $-M$ è a sinistra.

> [!example] Esempi
> $$\lim_{x\to+\infty}e^{-x}=0\qquad\qquad\lim_{x\to-\infty}\frac1x=0$$

## 2) Limite infinito all'infinito ($x_0=\pm\infty$, $\ell=\pm\infty$)

> [!abstract] $\displaystyle\lim_{x\to+\infty}f(x)=+\infty$
> $\forall M>0\ \exists K>0$ tale che $\quad x>K\ \Rightarrow\ f(x)>M$

> [!abstract] $\displaystyle\lim_{x\to+\infty}f(x)=-\infty$
> $\forall M>0\ \exists K>0$ tale che $\quad x>K\ \Rightarrow\ f(x)<-M$

Similmente per $\displaystyle\lim_{x\to-\infty}f(x)=+\infty$ e $\displaystyle\lim_{x\to-\infty}f(x)=-\infty$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** pag. 14 (caso $+\infty$) e pag. 15 (caso $-\infty$, entrambi per $x\to+\infty$), nel corpo della pagina. **Cosa cercare:** grafico di una funzione crescente (decrescente nel caso $-\infty$) con la soglia $M$ (o $-M$) segnata in blu sull'asse $y$ e la soglia $K$ in verde sull'asse $x$: oltre $K$ il grafico supera $M$ (o scende sotto $-M$).

> [!example] Esempi
> $$\lim_{x\to-\infty}e^{-x}=+\infty\qquad\qquad\lim_{x\to+\infty}\log x=+\infty$$

## Note collegate
- [[86_Definizione_Topologica_di_Limite]]
- [[88_Asintoto_Orizzontale_e_Limiti_per_Eccesso_e_per_Difetto]]
- [[89_Asintoto_Obliquo]]
- [[30_Limiti_di_Successioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/definizioni-metriche
