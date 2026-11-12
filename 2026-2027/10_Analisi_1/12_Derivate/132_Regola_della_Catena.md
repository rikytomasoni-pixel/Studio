---
tags:
  - AM1
  - derivate
  - regola-della-catena
  - funzione-composta
  - teorema
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 32-33)"
---

# Regola della catena (derivata della funzione composta)

> [!abstract] Teorema (regola della catena)
> Sia $g\circ f(x)=g(f(x))$ composizione di due funzioni. Se $f$ è derivabile in $x_0$ e $g$ è derivabile in $t_0=f(x_0)$, allora $g\circ f$ è derivabile in $x_0$ e vale
> $$(g\circ f)'(x_0)=g'\big(\underbrace{f(x_0)}_{t_0}\big)\cdot f'(x_0)$$

(La dimostrazione non è presente negli appunti di L17.)

## Esempi
**$h(x)=e^{\sin x}$.** Con $f(x)=\sin x$, $g(t)=e^t$, $h(x)=g\circ f(x)$:
$$h'(x)=e^{\sin x}\cdot\cos x$$

**$h(x)=a^x$, $a>0$, $a\neq1$.**
$$h(x)=e^{\log(a^x)}=e^{(\log a)\cdot x}\ \Rightarrow\ h'(x)=e^{(\log a)x}\cdot\log a=\log a\cdot a^x$$

**$h(x)=x^{\sin x}$, $x>0$.**
$$h(x)=e^{\log x^{\sin x}}=e^{\sin x\cdot\log x}$$
$$h'(x)=e^{\sin x\log x}\Big(\cos x\log x+\sin x\cdot\frac1x\Big)=x^{\sin x}\Big(\cos x\log x+\sin x\cdot\frac1x\Big)$$

## Note collegate
- [[131_Algebra_delle_Derivate]]
- [[128_Derivate_delle_Funzioni_Elementari]]
- [[105_Continuita_della_Funzione_Composta]]
- [[25_Composizione_di_Funzioni]]
- [[12_Logaritmi]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/regola-della-catena
