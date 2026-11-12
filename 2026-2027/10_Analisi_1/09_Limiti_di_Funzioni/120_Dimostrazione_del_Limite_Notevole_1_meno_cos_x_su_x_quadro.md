---
tags:
  - AM1
  - limiti-di-funzioni
  - limiti-notevoli
  - dimostrazione
  - trigonometria
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 3); Dimostrazioni primi limiti notevoli.pdf (pag. 1)"
---

# Dimostrazione di $\displaystyle\lim_{x\to0}\frac{1-\cos x}{x^2}=\frac12$

Dimostrazione del secondo limite notevole di [[108_Limiti_Notevoli_di_Funzioni]], che si deduce da $\displaystyle\lim_{x\to0}\frac{\sin x}{x}=1$ ([[119_Dimostrazione_del_Limite_Notevole_sin_x_su_x]]).

## Versione di lezione (formula di bisezione)
Poiché $\cos x=1-2\sin^2\frac x2$:
$$\frac{1-\cos x}{x^2}=\frac{1-\big(1-2\sin^2\frac x2\big)}{x^2}=\frac{2\sin\frac x2\ \sin\frac x2}{\frac x2\ \cdot\ \frac x2}\cdot\frac14\ \longrightarrow\ 2\cdot1\cdot1\cdot\frac14=\frac12\qquad(x\to0)$$
perché $\dfrac{\sin\frac x2}{\frac x2}\to1$ (cambio di variabile $t=\frac x2$, [[104_Cambio_di_Variabile_nei_Limiti]]).

## Versione delle esercitazioni (moltiplicando per il coniugato)
Moltiplicando e dividendo per $1+\cos x$:
$$\frac{1-\cos x}{x^2}\cdot\frac{1+\cos x}{1+\cos x}=\frac{1-\cos^2x}{x^2}\cdot\frac1{1+\cos x}=\underbrace{\frac{\sin^2x}{x^2}}_{\to\,1^2=1}\cdot\underbrace{\frac1{1+\cos x}}_{\to\,\frac12}\ \longrightarrow\ \frac12$$

## Conseguenza
$1-\cos x\sim\frac12x^2$ e $\cos x=1-\frac12x^2+o(x^2)$ per $x\to0$.

## Note collegate
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[119_Dimostrazione_del_Limite_Notevole_sin_x_su_x]]
- [[118_Dimostrazione_dei_Limiti_Notevoli]]
- [[128_Derivate_delle_Funzioni_Elementari]] (serve per la derivata del seno)
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/dimostrazione-1-meno-cos-x
