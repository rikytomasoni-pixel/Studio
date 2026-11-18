---
tags:
  - AM1
  - derivate
  - teorema
  - dimostrazione
  - rolle
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 17-18)"
---

# Teorema di Rolle

> [!abstract] Teorema (di Rolle)
> Sia $f:[a,b]\to\mathbb{R}$ continua in $[a,b]$ e derivabile in $(a,b)$. Inoltre sia $f(a)=f(b)$. Allora esiste $c\in(a,b)$ tale che
> $$f'(c)=0$$

**Dimostrazione.** Poiché $f$ è continua in $[a,b]$, per il [[112_Teorema_di_Weierstrass]] ammette massimo e minimo globali
$$M=\max_{[a,b]}f(x)\in\mathbb{R}\qquad m=\min_{[a,b]}f(x)\in\mathbb{R}$$

- **Se $M=m$**, allora $f$ è costante in $[a,b]$. Segue che $f'(x)=0$ per ogni $x\in(a,b)$:
$$f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}h=\lim_{h\to0}\frac0h=0\qquad\forall x\in(a,b)$$
- **Se $m<M$**, poiché $f(a)=f(b)$, almeno uno tra $m$ e $M$ deve essere assunto in un punto $c\in(a,b)$, cioè esiste $c\in(a,b)$ tale che $f(c)=m$ oppure $f(c)=M$. Quindi esiste $c\in(a,b)$ punto di estremo per $f$, con $f$ derivabile in $(a,b)$. Per il [[137_Teorema_di_Fermat]] deve essere $f'(c)=0$. $\square$

![[MassimiMinimiLocali.png|408]]

## Note collegate
- [[142_Teorema_di_Lagrange]]
- [[137_Teorema_di_Fermat]]
- [[112_Teorema_di_Weierstrass]]
- [[140_Test_di_Monotonia]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/rolle
