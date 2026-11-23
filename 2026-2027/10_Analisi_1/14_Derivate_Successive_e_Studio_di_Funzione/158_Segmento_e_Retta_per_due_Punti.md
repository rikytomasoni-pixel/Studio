---
tags:
  - AM1
  - derivate-successive
  - convessita
  - geometria-analitica
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 2-5)"
---

# Segmento e retta per due punti

Preliminare geometrico alla [[159_Interpretazione_Geometrica_della_Convessita|interpretazione geometrica della convessità]]: i punti $tx_1+(1-t)x_0$ che compaiono nella definizione di [[156_Funzioni_Convesse_e_Concave|funzione convessa]] descrivono un segmento.

## Retta per due punti di $\mathbb{R}^2$

Dati due punti distinti $P_0=(x_0,y_0)$ e $P_1=(x_1,y_1)$ di $\mathbb{R}^2$, l'insieme dei punti
$$P_t=(1-t)P_0+tP_1=P_0+t(P_1-P_0)=\big((1-t)x_0+tx_1,\ (1-t)y_0+ty_1\big),\qquad t\in\mathbb{R}$$
è la **retta** per $P_0$ e $P_1$. Infatti, se $P_t=(x,y)$,
$$\begin{cases}x=(1-t)x_0+tx_1\\ y=(1-t)y_0+ty_1\end{cases}\qquad\forall t\in\mathbb{R}$$
e risolvendo in $t$ (se $x_0\ne x_1$, $y_0\ne y_1$)
$$\frac{x-x_0}{x_1-x_0}=t=\frac{y-y_0}{y_1-y_0}\quad\text{cioè}\quad y=\underbrace{\frac{y_1-y_0}{x_1-x_0}}_{m}(x-x_0)+y_0$$
che è l'equazione della retta per $P_0,P_1$.

> [!note] Casi particolari
> Se $x_1=x_0$ allora $x=x_0$ (retta verticale); se $y_1=y_0$ allora $y=y_0$ (retta orizzontale).

## Segmento

Per $t\in[0,1]$
$$P_t=(1-t)P_0+tP_1$$
descrive il **segmento** di estremi $P_0$ e $P_1$ in $\mathbb{R}^2$, orientato da $P_0$ a $P_1$. Per $t<0$ e $t>1$ si ottengono i punti della retta fuori dal segmento (dalla parte di $P_0$ e di $P_1$ rispettivamente).

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Pag. 4:** retta per $P_0$ e $P_1$ (in blu), con il segmento $t\in[0,1]$ evidenziato in rosso, un punto $P_t$ (in verde) sul segmento e due punti $P_t$ sulla retta fuori dal segmento, uno con $t>1$ (oltre $P_1$) e uno con $t<0$ (prima di $P_0$). Da cercare: retta con due punti marcati e segmento rosso tra loro.

## Generalizzazione

In $\mathbb{R}^3$, con $P_0=(x_0,y_0,z_0)\ne P_1=(x_1,y_1,z_1)$, la formula $P_t=(1-t)P_0+tP_1$, $t\in\mathbb{R}$, è la retta per i due punti. Più in generale ciò è vero in $\mathbb{R}^n$ per ogni $n\ge2$: per $P_0\ne P_1$ in $\mathbb{R}^n$
$$P_t=(1-t)P_0+tP_1,\qquad t\in\mathbb{R}$$
è la retta in $\mathbb{R}^n$ per $P_0,P_1$.

## Note collegate
- [[159_Interpretazione_Geometrica_della_Convessita]]
- [[156_Funzioni_Convesse_e_Concave]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/convessita
