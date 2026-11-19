---
tags:
  - AM1
  - derivate
  - valore-assoluto
  - esempi
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 2-3)"
---

# Derivate con valore assoluto e segno

Esempi di calcolo della funzione derivata quando compare un [[09_Valore_Assoluto|valore assoluto]]: si passa alla definizione a tratti e si deriva ramo per ramo, studiando a parte i punti di raccordo.

## $f(x)=|x|$, $x\in\mathbb{R}$
$$f(x)=\begin{cases}x&x\ge0\\-x&x<0\end{cases}$$
In $x_0=0$ non esiste $f'(0)$, perché $f'_+(0)=1$ e $f'_-(0)=-1$ (vedi [[129_Derivabilita_e_Continuita]]). Per $x\neq0$:
$$f'(x)=\begin{cases}1&x>0\\-1&x<0\end{cases}=\operatorname{sgn}x\qquad x\neq0$$

## $f(x)=\log|x|$, $x\neq0$
$$f'(x)=\frac1{|x|}\cdot\operatorname{sgn}x=\frac1x\qquad x\neq0$$

> [!note] Osservazione
> $x=|x|\operatorname{sgn}x$ per ogni $x\in\mathbb{R}$; è questa identità che permette di ottenere $\dfrac1{|x|}\operatorname{sgn}x=\dfrac1x$.

## $f(x)=|x^2-2|$, $x\in\mathbb{R}$
$$f'(x)=\operatorname{sgn}(x^2-2)\cdot2x\qquad\forall x:\ x^2-2\neq0,\ \text{cioè }\forall x\neq\pm\sqrt2$$

**Alternativamente**, scrivendo la funzione a tratti:
$$|x^2-2|=\begin{cases}x^2-2&\text{se }x^2-2\ge0\\2-x^2&\text{se }x^2-2<0\end{cases}$$

## Note collegate
- [[123_Esempi_di_Derivata_e_Retta_Tangente]]
- [[130_Classificazione_dei_Punti_di_Non_Derivabilita]]
- [[131_Algebra_delle_Derivate]]
- [[132_Regola_della_Catena]]
- [[128_Derivate_delle_Funzioni_Elementari]]
- [[00_MOC_Analisi_1]]
- [[148_Teorema_di_Prolungamento_della_Derivata_Prima]]

#AM1/derivate/esempi
