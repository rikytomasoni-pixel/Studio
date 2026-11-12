---
tags:
  - AM1
  - derivate
  - algebra-delle-derivate
  - teorema
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 30-32)"
---

# Algebra delle derivate

> [!abstract] Teorema (algebra delle derivate)
> Siano $f,g:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, e $f,g$ derivabili in $x_0$. Allora:
> 1. $f\pm g$ è derivabile in $x_0$ e
>    $$(f\pm g)'(x_0)=f'(x_0)\pm g'(x_0)$$
> 2. $f\cdot g$ è derivabile in $x_0$ e
>    $$(f\cdot g)'(x_0)=f'(x_0)g(x_0)+f(x_0)g'(x_0)$$
>    In particolare $\forall\alpha\in\mathbb{R}$: $(\alpha\cdot f)'(x_0)=\alpha f'(x_0)$.
> 3. Se $g(x_0)\neq0$, $\dfrac fg$ è derivabile in $x_0$ e
>    $$\Big(\frac fg\Big)'(x_0)=\frac{f'(x_0)g(x_0)-f(x_0)g'(x_0)}{\big(g(x_0)\big)^2}$$

(La dimostrazione non è presente negli appunti di L17.)

> [!note] Osservazione — linearità
> Se $f,g$ sono derivabili in $x_0$, $\alpha,\beta\in\mathbb{R}$, allora $\alpha f+\beta g$ è derivabile in $x_0$ e
> $$(\alpha f+\beta g)'(x_0)=\alpha f'(x_0)+\beta g'(x_0)$$
> cioè la derivazione è **lineare**.

## Esempi
**$f(x)=\tan x=\dfrac{\sin x}{\cos x}$**
$$f'(x)=\frac{(\cos x)^2+(\sin x)^2}{(\cos x)^2}=\frac1{(\cos x)^2}=1+(\tan x)^2$$

**$f(x)=\sinh x=\dfrac{e^x-e^{-x}}2$**
$$f'(x)=\frac{e^x}2-\frac12\big(e^{-x}\big)'=\frac{e^x}2+\frac12e^{-x}=\frac{e^x+e^{-x}}2=\cosh x$$

**$f(x)=\cosh x=\dfrac{e^x+e^{-x}}2$**
$$f'(x)=\frac{e^x-e^{-x}}2=\sinh x$$

> [!note] Osservazione (non presente negli appunti)
> Il passaggio $\big(e^{-x}\big)'=-e^{-x}$ usato negli esempi con $\sinh x$ e $\cosh x$ segue dalla [[132_Regola_della_Catena|regola della catena]] (vista subito dopo nella stessa lezione).

## Note collegate
- [[128_Derivate_delle_Funzioni_Elementari]]
- [[132_Regola_della_Catena]]
- [[102_Algebra_dei_Limiti_di_Funzioni]]
- [[103_Algebra_delle_Funzioni_Continue]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/algebra-delle-derivate
