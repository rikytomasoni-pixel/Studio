---
tags:
  - AM1
  - taylor
  - corollario
  - estremi-locali
  - flessi
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 7)"
---

# Corollario: classificazione con le derivate successive

> [!abstract] Corollario (del teorema di Taylor con resto di Peano)
> Sia $f:(a,b)\to\mathbb{R}$ derivabile $n$ volte in $x_0\in(a,b)$, $n\ge2$, con
> $$f'(x_0)=f''(x_0)=\dots=f^{(n-1)}(x_0)=0\qquad\text{e}\qquad f^{(n)}(x_0)\ne0.$$
> Allora:
> 1. se $n$ è **dispari**, $x_0$ è un **flesso a tangente orizzontale**;
> 2. se $n$ è **pari** e $f^{(n)}(x_0)>0$, $x_0$ è un punto di **minimo locale**;
> 3. se $n$ è **pari** e $f^{(n)}(x_0)<0$, $x_0$ è un punto di **massimo locale**.

*(negli appunti: "no dim.")*

> [!tip] Idea (non negli appunti)
> Segue da $f(x)-f(x_0)=\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n+o\big((x-x_0)^n\big)$: il segno di $f(x)-f(x_0)$ vicino a $x_0$ è quello di $f^{(n)}(x_0)(x-x_0)^n$.

Per $n=2$ si ritrova il criterio con la derivata seconda ([[165_Flessi_e_Derivata_Seconda]]); gli esempi $x^3$ ($n=3$) e $x^4$ ($n=4$) in $x_0=0$ sono già in [[138_Punti_Stazionari_e_Punti_Critici]] e [[165_Flessi_e_Derivata_Seconda]].

## Note collegate
- [[168_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[137_Teorema_di_Fermat]]
- [[138_Punti_Stazionari_e_Punti_Critici]]
- [[163_Punti_di_Flesso]]
- [[165_Flessi_e_Derivata_Seconda]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/classificazione-stazionari
