---
tags:
  - AM1
  - taylor
  - approssimazione-polinomiale
  - o-piccolo
  - de-l-hopital
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 16-18)"
---

# Approssimazioni polinomiali e sviluppo del seno

## Motivazione

Abbiamo visto che (ad esempio)
$$\sin x=x+o(x)\qquad\text{per }x\to0$$
Questo non è sempre sufficiente. Ad esempio
$$\lim_{x\to0}\frac{\sin x-x}{x^3}=\lim_{x\to0}\frac{o(x)}{x^3}=\left[\tfrac00\right]$$
e da $o(x)$ non si ricava il limite (è una forma di indecisione: $\frac{o(x)}{x^3}=o\!\left(\frac1{x^2}\right)$).

## Calcolo con de l'Hôpital

Tuttavia per [[152_Teorema_di_de_l_Hopital|de l'Hôpital]] (applicato tre volte)
$$\lim_{x\to0}\frac{\sin x-x}{x^3}\overset{H}{=}\lim_{x\to0}\frac{\cos x-1}{3x^2}\overset{H}{=}\lim_{x\to0}\frac{-\sin x}{6x}\overset{H}{=}\lim_{x\to0}-\frac16\cos x=-\frac16$$

$$\Rightarrow\ \lim_{x\to0}\frac{\sin x-x}{x^3}+\frac16=0\ \Rightarrow\ \lim_{x\to0}\frac{\sin x-x+\frac16x^3}{x^3}=0$$
$$\Rightarrow\ \sin x-x+\frac16x^3=o(x^3)\ \Rightarrow\ \boxed{\sin x=x-\frac16x^3+o(x^3)}\qquad x\to0$$

> [!important] Raffinamento
> Questo è un **raffinamento** di $\sin x=x+o(x)$ per $x\to0$: il termine $-\frac16x^3+o(x^3)$ sostituisce il resto $o(x)$.

## Altri esempi (stessa idea)

$$e^x=1+x+o(x)\qquad x\to0$$
$$e^x=1+x+\frac{x^2}{2}+o(x^2)\qquad x\to0$$
$$e^x=1+x+\frac{x^2}{2}+\frac{x^3}{6}+o(x^3)\qquad x\to0$$
e così via.

## Idea generale: polinomi di grado più alto

L'approssimazione di una funzione $f$ tramite un polinomio di grado al più 1
$$f(x)=f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)\qquad x\to x_0$$
realizzata tramite la derivata prima e la nozione di [[127_Differenziabilita_e_Approssimazione_Lineare|differenziabilità]], non è sempre sufficiente nelle applicazioni.

L'idea è di ricavare **approssimazioni migliori** di $f$ per $x\to x_0$ con polinomi di grado anche più elevato. A tale scopo, se $f$ è derivabile in $x_0\in(a,b)$ almeno $n$ volte con $n\ge1$, il candidato più ragionevole è il polinomio di grado (al più) $n$ che abbia in $x_0$ lo stesso valore di $f$, insieme a tutte le sue derivate fino all'ordine $n$ incluso. Se indichiamo con $P_n(x)$ tale polinomio, vogliamo quindi che
$$P_n^{(k)}(x_0)=f^{(k)}(x_0)\qquad\forall k=0,1,\dots,n$$
(per convenzione $f^{(0)}(x)=f(x)$ per ogni $x$). Il polinomio che soddisfa questa richiesta è il [[167_Polinomio_di_Taylor|polinomio di Taylor]].

## Note collegate
- [[167_Polinomio_di_Taylor]]
- [[168_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[152_Teorema_di_de_l_Hopital]]
- [[154_Esempi_di_Applicazione_de_l_Hopital]]
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[127_Differenziabilita_e_Approssimazione_Lineare]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/approssimazioni
