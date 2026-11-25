---
tags:
  - AM1
  - derivate-successive
  - convessita
  - interpretazione-geometrica
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 5-7)"
---

# Interpretazione geometrica della convessità: le corde

> [!abstract] Riformulazione della definizione
> Se $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo, $f$ è convessa in $I$ se e solo se $\forall x_0,x_1\in I$, $\forall t\in[0,1]$ vale
> $$(*)\qquad f\big((1-t)x_0+tx_1\big)\le(1-t)f(x_0)+t f(x_1)$$
> (è la definizione di [[156_Funzioni_Convesse_e_Concave]] con $t$ e $1-t$ scambiati).

## La corda sul grafico

Siano $P_0=(x_0,f(x_0))$, $P_1=(x_1,f(x_1))$ con $x_0\ne x_1$. Il segmento di estremi $P_0,P_1$ (**corda** sul grafico) è, per [[158_Segmento_e_Retta_per_due_Punti]],
$$P_t=(1-t)P_0+tP_1=\big(\underbrace{(1-t)x_0+tx_1}_{x_t},\ \underbrace{(1-t)f(x_0)+tf(x_1)}_{y_t}\big),\qquad t\in[0,1]$$
Con queste relazioni $(*)$ diventa
$$f(x_t)\le y_t\qquad\forall t\in[0,1]$$

In altri termini: all'ascissa $x_t$ il valore $f(x_t)$ è minore o uguale a $y_t$, cioè il punto $(x_t,f(x_t))$ sul grafico di $f$ giace **sotto** il punto $(x_t,y_t)$ sulla corda di estremi $P_0,P_1$.

> [!important] Significato geometrico
> La disuguaglianza $(*)$ dice che, comunque si scelgano due punti $P_0,P_1$ sul grafico di $f$, la corda di estremi $P_0,P_1$ giace **sopra** il grafico di $f$ (tra $x_0$ e $x_1$).

![[cordaSuGrafico.png]]

## Forma equivalente

Equivalentemente (usando l'equazione della retta per $P_0,P_1$)
$$f(x)\le\frac{f(x_1)-f(x_0)}{x_1-x_0}(x-x_0)+f(x_0)\qquad\forall x_0,x_1\in I,\ \forall x\in[x_0,x_1]\ \ (\text{con }x_0<x_1)$$

## Note collegate
- [[156_Funzioni_Convesse_e_Concave]]
- [[158_Segmento_e_Retta_per_due_Punti]]
- [[160_Teorema_di_Regolarita_delle_Funzioni_Convesse]]
- [[161_Convessita_e_Rette_Tangenti]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/convessita
