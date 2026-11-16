---
tags:
  - AM1
  - derivate
  - funzione-inversa
  - esempi
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 3-5)"
---

# Derivate di $\arctan$, $\log$, $\arcsin$ (con la funzione inversa)

Applicazioni del [[134_Teorema_della_Derivata_della_Funzione_Inversa]].

## $y=\tan x\ \Rightarrow\ x=\arctan y$
Qui $y=f(x)=\tan x$, $x\in\left(-\frac\pi2,\frac\pi2\right)$, e $x=f^{-1}(y)=\arctan y$, $y\in\mathbb{R}$.
$$(\arctan)'(y)=\frac1{(\tan)'(x)}=\frac1{1+(\tan x)^2}=\frac1{1+y^2}\qquad\forall y\in\mathbb{R}$$

## $y=e^x\ \Rightarrow\ x=\log y$
Qui $y=f(x)=e^x$, $x\in\mathbb{R}$, e $x=f^{-1}(y)=\log y$, $y>0$.
$$(\log)'(y)=\frac1{(e^x)'}=\frac1{e^x}=\frac1y\qquad\forall y>0$$

## $y=\sin x\ \Rightarrow\ x=\arcsin y$
Qui $y=f(x)=\sin x$, $x\in\left[-\frac\pi2,\frac\pi2\right]$, e $x=f^{-1}(y)=\arcsin y$, $y\in[-1,1]$.
$$(\arcsin)'(y)=\frac1{(\sin)'(x)}=\frac1{\cos x}=\frac1{+\sqrt{1-\sin^2x}}=\frac1{\sqrt{1-y^2}}\qquad\forall y\in(-1,1)$$

> [!note] Osservazione
> Il segno $+$ davanti alla radice è dovuto al fatto che $\cos x\ge0$ per $x\in\left[-\frac\pi2,\frac\pi2\right]$. La derivata è calcolata solo in $(-1,1)$ perché in $y=\pm1$ si avrebbe $\cos x=0$, cioè $f'(x)=0$ e il teorema non si applica.

## Note collegate
- [[134_Teorema_della_Derivata_della_Funzione_Inversa]]
- [[128_Derivate_delle_Funzioni_Elementari]]
- [[132_Regola_della_Catena]]
- [[28_Esempi_Funzioni_Inverse]]
- [[12_Logaritmi]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/funzione-inversa
