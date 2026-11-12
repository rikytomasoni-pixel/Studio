---
tags:
  - AM1
  - derivate
  - funzioni-elementari
  - limiti-notevoli
  - tabella
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 21-23)"
---

# Derivate delle funzioni elementari

| $f(x)$ | $f'(x)$ | |
| :-- | :-- | :-- |
| $c\in\mathbb{R}$ | $0$ | |
| $x^n$ | $n\,x^{n-1}$ | $n\in\mathbb{N}$ |
| $x^\alpha$ | $\alpha\,x^{\alpha-1}$ | $\alpha\in\mathbb{R}$ |
| $\sin x$ | $\cos x$ | |
| $\cos x$ | $-\sin x$ | |
| $e^x$ | $e^x$ | |
| $\log x$ | $\dfrac1x$ | |
| $\dfrac1x$ | $-\dfrac1{x^2}$ | |
| $\sqrt x$ | $\dfrac1{2\sqrt x}$ | |
| $\dots$ | $\dots$ | |

## Esempio: $f(x)=\sin x\ \Rightarrow\ f'(x)=\cos x$
$$f'(x)=\lim_{h\to0}\frac{\sin(x+h)-\sin x}{h}=\lim_{h\to0}\frac{\sin x\cos h+\sin h\cos x-\sin x}{h}$$
$$=\lim_{h\to0}\Big(\underbrace{\sin x}_{\in\mathbb{R}}\ \underbrace{\frac{\cos h-1}{h^2}}_{\to-\frac12}\ \underbrace{h}_{\to0}+\underbrace{\frac{\sin h}{h}}_{\to1}\ \underbrace{\cos x}_{\in\mathbb{R}}\Big)=\cos x$$
Qui si usano i limiti notevoli $\dfrac{\sin h}{h}\to1$ ([[119_Dimostrazione_del_Limite_Notevole_sin_x_su_x]]) e $\dfrac{\cos h-1}{h^2}\to-\dfrac12$ ([[120_Dimostrazione_del_Limite_Notevole_1_meno_cos_x_su_x_quadro]]).

## Esempio: $f(x)=e^x\ \Rightarrow\ f'(x)=e^x$
$$f'(x)=\lim_{h\to0}\frac{e^{x+h}-e^x}{h}=\lim_{h\to0}\underbrace{e^x}_{\in\mathbb{R}}\ \underbrace{\frac{e^h-1}{h}}_{\to1}=e^x$$
(limite notevole $\dfrac{e^h-1}{h}\to1$, vedi [[118_Dimostrazione_dei_Limiti_Notevoli]]).

## Note collegate
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[131_Algebra_delle_Derivate]]
- [[132_Regola_della_Catena]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/funzioni-elementari
