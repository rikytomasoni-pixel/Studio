---
tags:
  - AM1
  - derivate
  - teorema
  - dimostrazione
  - funzioni-costanti
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 16, 20-22)"
---

# Caratterizzazione delle funzioni costanti su un intervallo

> [!abstract] Teorema (caratterizzazione delle funzioni costanti su un intervallo)
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo. Allora $f$ è costante in $I$ se e solo se $f$ è derivabile in $I$ con $f'(x)=0$ per ogni $x\in I$.

**Dimostrazione.**

($\Rightarrow$) Se $f$ è costante in $I$, $f(x)=\lambda$ per ogni $x\in I$, con $\lambda\in\mathbb{R}$ fissato. Segue che
$$f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}h=\lim_{h\to0}\frac{\lambda-\lambda}h=\lim_{h\to0}\frac0h=0$$
cioè $f$ è derivabile in $I$ e $f'(x)=0$ per ogni $x\in I$.

($\Leftarrow$) Vogliamo mostrare che $f$ è costante in $I$, cioè che per ogni $x_1,x_2\in I$ vale $f(x_1)=f(x_2)$. Siano $x_1,x_2\in I$ con $x_1<x_2$. Allora $f:[x_1,x_2]\to\mathbb{R}$ è derivabile e quindi anche continua in $[x_1,x_2]\subseteq I$. Per il [[142_Teorema_di_Lagrange|teorema di Lagrange]] esiste $c\in(x_1,x_2)\subseteq I$ tale che
$$f(x_2)-f(x_1)=f'(c)(x_2-x_1)$$
Poiché $f'(x)=0$ per ogni $x\in I$, avremo $f'(c)=0$ e
$$f(x_2)-f(x_1)=f'(c)(x_2-x_1)=0\ \Rightarrow\ f(x_2)=f(x_1)\ \Rightarrow\ f\text{ è costante}\qquad\square$$

## Osservazione: l'ipotesi "intervallo" è necessaria
Se $f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$ e $\mathcal{D}(f)$ **non** è un intervallo, può accadere che $f'(x)=0$ per ogni $x\in\mathcal{D}(f)$ ma che $f$ non sia costante in $\mathcal{D}(f)$.

**Esempio.**
$$f(x)=\begin{cases}1&\text{se }x>0\\-1&\text{se }x<0\end{cases}\qquad f:\underbrace{(-\infty,0)\cup(0,\infty)}_{\mathcal{D}(f)}\to\mathbb{R}$$
$f'(x)=0$ per ogni $x\in\mathcal{D}(f)$, $\mathcal{D}(f)$ non è un intervallo e $f$ non è costante.

## Note collegate
- [[142_Teorema_di_Lagrange]]
- [[141_Teorema_di_Rolle]]
- [[140_Test_di_Monotonia]]
- [[129_Derivabilita_e_Continuita]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/funzioni-costanti
