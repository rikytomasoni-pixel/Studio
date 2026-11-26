---
tags:
  - AM1
  - taylor
  - serie-di-taylor
  - serie
  - definizione
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 16-19)"
---

# Serie di Taylor

Se $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo, è derivabile infinite volte in $I$ e $x,x_0\in I$, per ogni $n\in\mathbb{N}$ si può scrivere il [[167_Polinomio_di_Taylor|polinomio di Taylor]]
$$P_n(x)=\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$$
Passando (**formalmente**) al limite per $n\to\infty$ si trova la serie
$$\sum_{k=0}^{\infty}\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$$

> [!abstract] Definizione (serie di Taylor)
> Se $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo, $x_0\in I$, $f$ derivabile infinite volte in $x_0$, la serie $\displaystyle\sum_{k=0}^{\infty}\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$ si dice **serie di Taylor di $f$ centrata in $x_0$** (di **Mac Laurin** se $x_0=0$).

## Osservazioni

- La somma parziale $N$-esima della serie di Taylor di $f$ è il polinomio di Taylor di $f$ di ordine $N$, $\forall N\in\mathbb{N}$ ([[47_Serie_Introduzione_e_Somme_Parziali]]).
- **Non è detto** che la serie di Taylor di $f$ centrata in $x_0$ converga per $x\ne x_0$ (in $x=x_0$ converge a $f(x_0)$).
- **Se** la serie di Taylor di $f$ converge in $x$, **non è detto** che converga a $f(x)$.

## Esempi (dimostrabili, non dimostrati a lezione)

Si dimostra tuttavia che
$$e^x=\sum_{k=0}^\infty\frac{x^k}{k!}\ \ \forall x\in\mathbb{R}\qquad\sin x=\sum_{k=0}^\infty(-1)^k\frac{x^{2k+1}}{(2k+1)!}\ \ \forall x\in\mathbb{R}$$
$$\cos x=\sum_{k=0}^\infty(-1)^k\frac{x^{2k}}{(2k)!}\ \ \forall x\in\mathbb{R}\qquad\frac1{1-x}=\sum_{k=0}^\infty x^k\ \ \forall x\in(-1,1)$$
(l'ultima è la [[50_Serie_Geometrica|serie geometrica]]). In particolare, per $x=1$:
$$e=\lim_{n\to\infty}\Big(1+\frac1n\Big)^n=\sum_{k=0}^\infty\frac1{k!}$$
(numero di Nepero, [[38_Numero_di_Nepero]]).

## Note collegate
- [[167_Polinomio_di_Taylor]]
- [[172_Sviluppi_di_Maclaurin_di_e_alla_x_sin_cos]]
- [[180_Esponenziale_Complesso_e_Formula_di_Eulero]]
- [[50_Serie_Geometrica]]
- [[38_Numero_di_Nepero]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/serie-di-taylor
