---
tags:
  - AM1
  - derivate
  - motivazione
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 4-6)"
---

# Problemi che motivano la derivata

Introduzione al calcolo differenziale: tre problemi la cui risposta porta alla definizione di [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto|derivata]].

## Problema 1 — retta tangente al grafico
Data $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, come **definire** la retta tangente al grafico di $f$ nel punto $(x_0,f(x_0))$?

**Esempio.** Se $f(x)=\alpha x^2+\beta x+\gamma$ con $\alpha\neq0$, il grafico è una parabola in $\mathbb{R}^2$. Sia $x_0\in\mathbb{R}$ e $P_0=(x_0,f(x_0))$. Allora tutte le rette (non verticali) per $P_0$ hanno $2$ intersezioni distinte con il grafico di $f$ (una delle quali è $P_0$), tranne un'unica retta $r$. Quell'unica retta $r$ è la retta tangente al grafico di $f$ in $P_0$.

![[rettaTangente.png]]

**Esempio.** $f(x)=|x|$, $x_0=0$, $P_0=(0,0)$. Esiste retta tangente in $P_0$?

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 5**: grafico di $|x|$ con alcune rette per l'origine (verdi, blu e una rossa quasi orizzontale) che intersecano il grafico in modi diversi.

**Esempio.**
$$f(x)=\begin{cases}x^2\sin\frac1x&x\neq0\\0&x=0\end{cases}\qquad P_0=(0,0)$$
Esiste retta tangente in $P_0$?

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 5**: grafico di $f$ che oscilla tra le parabole $x^2$ e $-x^2$ (in blu) con oscillazioni sempre più fitte vicino all'origine.

(Le risposte arrivano in [[123_Esempi_di_Derivata_e_Retta_Tangente]].)

## Problema 2 — tasso di variazione istantaneo
Data $y=f(t)$ con $f:(a,b)\to\mathbb{R}$ e $t_0\in(a,b)$, la **variazione media** di $f$ nell'intervallo $[t_0,t_0+T]$ (per $T>0$, $t_0+T<b$) è
$$\frac{\Delta f}{\Delta t}=\frac{f(t_0+T)-f(t_0)}{T}$$
Come trovare/definire il **tasso di variazione istantaneo** di $f$ rispetto a $t$ per $t=t_0$?

## Problema 3 — approssimazione lineare
Data $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$. È possibile (in qualche senso da precisare) approssimare $f$ con un polinomio di grado al più $1$ in $x$, vicino a $x_0$? (Risposta: [[127_Differenziabilita_e_Approssimazione_Lineare]].)

## Note collegate
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[123_Esempi_di_Derivata_e_Retta_Tangente]]
- [[126_Interpretazione_della_Derivata_nelle_Applicazioni]]
- [[127_Differenziabilita_e_Approssimazione_Lineare]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/motivazione
