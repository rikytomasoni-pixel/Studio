---
tags:
  - AM1
  - derivate
  - esempio
  - retta-tangente
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 10-11)"
---

# Esempi di derivata e retta tangente

Esempi che rispondono alle domande di [[121_Problemi_Motivanti_delle_Derivate]], usando la definizione di [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto|derivata]].

## Parabola $f(x)=\alpha x^2+\beta x+\gamma$, $\alpha\neq0$
La retta tangente al grafico di $f$ in $P_0=(x_0,f(x_0))$ è data da
$$y=\underbrace{(2\alpha x_0+\beta)}_{f'(x_0)}(x-x_0)+\underbrace{(\alpha x_0^2+\beta x_0+\gamma)}_{f(x_0)}$$
e coincide con l'unica retta (non verticale) che ha una sola intersezione col grafico di $f$ in $(x_0,f(x_0))$.

## Valore assoluto $f(x)=|x|$, $x_0=0$, $P_0=(0,0)$
$$\lim_{h\to0^\pm}\frac{f(0+h)-f(0)}{h}=\lim_{h\to0^\pm}\frac{|h|}{h}=\lim_{h\to0^\pm}\operatorname{sgn}h=\pm1$$
Quindi $f'_+(0)=+1$, $f'_-(0)=-1$, dunque non esiste $\displaystyle\lim_{h\to0}\frac{f(0+h)-f(0)}{h}$ e $f$ **non è derivabile** in $x_0=0$. Di conseguenza non esiste la retta tangente al grafico di $f$ in $P_0=(0,0)$ (esistono solo le rette tangenti da destra e da sinistra, $y=x$ e $y=-x$; vedi [[130_Classificazione_dei_Punti_di_Non_Derivabilita|punto angoloso]]).

## $f(x)=\begin{cases}x^2\sin\frac1x&x\neq0\\0&x=0\end{cases}$, $x_0=0$, $P_0=(0,0)$
$$f'(0)=\lim_{h\to0}\frac{f(h)-f(0)}{h}=\lim_{h\to0}\frac{h^2\sin\frac1h-0}{h}=\lim_{h\to0}h\sin\frac1h=0$$
(infinitesima per limitata). Dunque $f$ è derivabile in $x_0=0$ e
$$y=0\cdot(x-0)+0=0$$
è la retta tangente al suo grafico in $P_0$.

## Note collegate
- [[121_Problemi_Motivanti_delle_Derivate]]
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[130_Classificazione_dei_Punti_di_Non_Derivabilita]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/esempi
