---
tags:
  - AM1
  - numeri-complessi
  - esponenziale-complesso
  - formula-di-eulero
  - serie
  - dimostrazione
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 19-20)"
---

# Esponenziale complesso e formula di Eulero

> [!abstract] Definizione
> $\forall z\in\mathbb{C}$
> $$e^z=\sum_{k=0}^\infty\frac{z^k}{k!}$$
> Questa serie converge **assolutamente** (e quindi semplicemente) in $\mathbb{C}$ e
> $$e^{z+w}=e^z\cdot e^w\qquad\forall z,w\in\mathbb{C}$$

È la stessa serie di [[179_Serie_di_Taylor|Taylor di $e^x$]], estesa a $z$ complesso.

> [!abstract] Formula di Eulero
> $$e^{i\theta}=\cos\theta+i\sin\theta\qquad\forall\theta\in\mathbb{R}$$

## Dimostrazione

$$e^{i\theta}=\sum_{k=0}^\infty\frac{(i\theta)^k}{k!}=\sum_{k=0}^\infty\frac{i^k\theta^k}{k!}=\sum_{j=0}^\infty\frac{i^{2j}\theta^{2j}}{(2j)!}+\sum_{j=0}^\infty\frac{i^{2j+1}\theta^{2j+1}}{(2j+1)!}$$
Questo passaggio (separare i termini pari e dispari) è lecito **perché la serie converge assolutamente**. Poiché $i^{2j}=(-1)^j$ e $i^{2j+1}=i(-1)^j$:
$$e^{i\theta}=\sum_{j=0}^\infty(-1)^j\frac{\theta^{2j}}{(2j)!}+i\sum_{j=0}^\infty(-1)^j\frac{\theta^{2j+1}}{(2j+1)!}=\cos\theta+i\sin\theta\qquad\square$$

## Conseguenza

Per ogni $z=a+ib\in\mathbb{C}$:
$$e^{a+ib}=e^a\cdot e^{ib}=e^a(\cos b+i\sin b)$$

## Note collegate
- [[179_Serie_di_Taylor]]
- [[172_Sviluppi_di_Maclaurin_di_e_alla_x_sin_cos]]
- [[15_Forma_Trigonometrica_Esponenziale]] (forma esponenziale dei complessi)
- [[73_Convergenza_Assoluta_e_Semplice]]
- [[13_Numeri_Complessi]]
- [[00_MOC_Analisi_1]]

#AM1/numeri-complessi/esponenziale-complesso
