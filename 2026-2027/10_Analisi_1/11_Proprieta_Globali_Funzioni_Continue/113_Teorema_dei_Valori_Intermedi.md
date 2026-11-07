---
tags:
  - AM1
  - continuita
  - valori-intermedi
  - teorema
data: 2026-11-06
lezione: 16
fonte: "AM1 L16 26-27.pdf (pag. 7-9)"
---

# Teorema dei valori intermedi

> [!abstract] Teorema (dei valori intermedi)
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$ con $I\subseteq\mathbb{R}$ intervallo, sia $f$ continua in $I$. Allora se $y_1,y_2\in\operatorname{Im}f$, per ogni $\lambda$ compreso tra $y_1$ e $y_2$ $\exists x_0\in I$ tale che
> $$f(x_0)=\lambda$$
> In particolare $\operatorname{Im}f$ è un **intervallo**.

## Dimostrazione
Siano $y_1,y_2\in\operatorname{Im}f\subseteq\mathbb{R}$. Supponiamo $y_1\le y_2$. Dunque $\exists x_1,x_2\in I$ tali che $f(x_1)=y_1$, $f(x_2)=y_2$.

Se $\lambda=y_1$ o $\lambda=y_2$ allora $x_0=x_1$ o $x_0=x_2$ e la dimostrazione è conclusa.

Se $\lambda\in(y_1,y_2)$, per comodità supponiamo $x_1<x_2$ (il caso $x_2<x_1$ è simile). Poiché $x_1,x_2\in I$, $[x_1,x_2]\subseteq I$ e $f$ ristretta a $[x_1,x_2]$ è continua. Consideriamo la funzione ausiliaria
$$g:[x_1,x_2]\to\mathbb{R},\qquad g(x)=f(x)-\lambda\quad\forall x\in[x_1,x_2]$$
Allora $g$ è continua in $[x_1,x_2]$. Inoltre
$$g(x_1)=f(x_1)-\lambda=y_1-\lambda<0\qquad g(x_2)=f(x_2)-\lambda=y_2-\lambda>0$$
Per il [[111_Teorema_degli_Zeri|teorema degli zeri]] applicato alla funzione continua $g$, $\exists x_0\in[x_1,x_2]\subseteq I$ tale che
$$0=g(x_0)=f(x_0)-\lambda\ \Rightarrow\ f(x_0)=\lambda,\quad x_0\in I$$
In particolare abbiamo quindi $[y_1,y_2]\subseteq\operatorname{Im}f$ $\forall y_1,y_2\in\operatorname{Im}f$, cioè $\operatorname{Im}f\subseteq\mathbb{R}$ è un intervallo. $\square$

> [!note] Osservazione
> Se $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo e $f$ continua, allora
> $$\operatorname{Im}f\supseteq\Big(\inf_If,\ \sup_If\Big)$$
> $\inf_If$ può appartenere a $\operatorname{Im}f$ oppure no; $\sup_If$ può appartenere a $\operatorname{Im}f$ oppure no. Dipende dalla funzione $f$ considerata.

## Note collegate
- [[111_Teorema_degli_Zeri]]
- [[114_Immagine_di_una_Funzione_Continua_su_un_Intervallo_Chiuso]]
- [[116_Continuita_e_Invertibilita]]
- [[10_Retta_Reale_Intervalli]]
- [[00_MOC_Analisi_1]]

#AM1/proprieta-globali/valori-intermedi
