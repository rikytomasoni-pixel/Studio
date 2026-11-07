---
tags:
  - AM1
  - limiti-di-funzioni
  - limite-metrico
  - limite-infinito
  - definizione
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 2-4)"
---

# Limite infinito in un punto finito

Terzo caso delle [[87_Definizioni_Metriche_di_Limite_all_Infinito|definizioni metriche]] (dopo il limite finito e infinito all'infinito): $\ell=\pm\infty$, $x_0\in\mathbb{R}$.

> [!abstract] Definizione — $\displaystyle\lim_{x\to x_0}f(x)=+\infty$
> $\forall M>0\ \exists\delta>0$ tale che
> $$\begin{cases}x\in(x_0-\delta,x_0+\delta)\\ x\neq x_0\end{cases}\ \Rightarrow\ f(x)\in(M,+\infty)$$
> cioè
> $$x_0-\delta<x<x_0+\delta,\ x\neq x_0\ \Rightarrow\ f(x)>M\qquad\text{ovvero}\qquad 0<|x-x_0|<\delta\ \Rightarrow\ f(x)>M$$

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L14 pag. 2: grafico con una curva che "esplode" verso l'alto attorno a $x_0$; retta orizzontale blu all'altezza $M$ sull'asse $y$, intervallo $(x_0-\delta,x_0+\delta)$ evidenziato in verde sull'asse $x$ (con $x_0$ al centro).

> [!abstract] Definizione — $\displaystyle\lim_{x\to x_0}f(x)=-\infty$
> $\forall M>0\ \exists\delta>0$ tale che
> $$\begin{cases}x\in(x_0-\delta,x_0+\delta)\\ x\neq x_0\end{cases}\ \Rightarrow\ f(x)\in(-\infty,-M)$$
> cioè
> $$x_0-\delta<x<x_0+\delta,\ x\neq x_0\ \Rightarrow\ f(x)<-M\qquad\text{ovvero}\qquad 0<|x-x_0|<\delta\ \Rightarrow\ f(x)<-M$$

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L14 pag. 3: grafico speculare (curva che scende verso $-\infty$ attorno a $x_0$, sopra la retta orizzontale $-M$), con intorno $(x_0-\delta,x_0+\delta)$ in verde.

> [!example] Esempio
> $$\lim_{x\to0}\frac{1}{x^2}=+\infty$$

## Note collegate
- [[87_Definizioni_Metriche_di_Limite_all_Infinito]]
- [[86_Definizione_Topologica_di_Limite]]
- [[91_Limiti_Destro_e_Sinistro_e_Asintoto_Verticale]]
- [[92_Limite_Finito_in_un_Punto_Finito]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/limite-infinito-al-punto
