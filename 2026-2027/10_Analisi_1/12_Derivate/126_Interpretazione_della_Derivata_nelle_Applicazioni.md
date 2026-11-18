---
tags:
  - AM1
  - derivate
  - applicazioni
  - interpretazione
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 16-17)"
---

# Interpretazione della derivata nelle applicazioni

Se $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$, $h\in\mathbb{R}$ tale che $x_0+h\in(a,b)$, $h\neq0$, allora
$$\frac{\Delta f}{\Delta x}=\frac{f(x_0+h)-f(x_0)}{h}$$
esprime la **variazione media** di $y=f(x)$ nell'intervallo di estremi $x_0,x_0+h$.

Se $f$ è derivabile in $x_0$,
$$f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}\in\mathbb{R}$$
esprime il **tasso di variazione istantaneo** di $y=f(x)$ al variare della variabile indipendente $x$, in $x=x_0$ (risposta al Problema 2 di [[121_Problemi_Motivanti_delle_Derivate]]).

In particolare:
- se $y=s(t)$ è la legge oraria, $s'(t)$ è la **velocità istantanea**;
- se $y=v(t)$ è la velocità, $v'(t)$ è l'**accelerazione istantanea**;
- se $y=\theta(t)$ è un angolo di rotazione (ad es. in un pendolo), $\theta'(t)$ è la **velocità angolare istantanea**;
- $\dots$ (ecc.)

## Note collegate
- [[121_Problemi_Motivanti_delle_Derivate]]
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/interpretazione
