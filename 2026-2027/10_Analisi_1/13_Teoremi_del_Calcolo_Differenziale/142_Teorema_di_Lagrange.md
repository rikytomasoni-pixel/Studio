---
tags:
  - AM1
  - derivate
  - teorema
  - dimostrazione
  - lagrange
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 18-20)"
---

# Teorema del valor medio di Lagrange

> [!abstract] Teorema (del valor medio di Lagrange)
> Sia $f:[a,b]\to\mathbb{R}$ continua in $[a,b]$ e derivabile in $(a,b)$. Allora esiste $c\in(a,b)$ tale che
> $$f'(c)=\frac{f(b)-f(a)}{b-a}\tag{$*$}$$

**Nota.** $\dfrac{f(b)-f(a)}{b-a}$ è il coefficiente angolare della retta per $(b,f(b))$ e $(a,f(a))$: il teorema afferma che esiste un punto in cui la tangente è parallela a tale retta.

![[thmLagrange.png]]

> [!note] Osservazioni
> - Se si aggiunge l'ipotesi $f(b)=f(a)$ si ritrova il [[141_Teorema_di_Rolle]].
> - Spesso si usa $(*)$ nella forma equivalente $f(b)-f(a)=f'(c)(b-a)$.

**Dimostrazione.** Vogliamo ricondurci al teorema di Rolle. Introduciamo la funzione ausiliaria
$$g(x)=f(x)-\Big(\underbrace{\frac{f(b)-f(a)}{b-a}(x-a)+f(a)}_{\text{equazione della retta per }(b,f(b)),\,(a,f(a))}\Big)$$
Allora $g:[a,b]\to\mathbb{R}$ e
- $g$ è continua perché lo è $f$ in $[a,b]$;
- $g$ è derivabile perché lo è $f$ in $(a,b)$ (l'equazione della retta è un polinomio di grado al più 1, quindi una funzione continua e derivabile);
- $g(a)=0$, $g(b)=0$, quindi $g(a)=g(b)=0$.

Per il teorema di Rolle esiste $c\in(a,b)$ tale che $g'(c)=0$. Per l'[[131_Algebra_delle_Derivate|algebra delle derivate]]
$$0=g'(c)=f'(c)-\frac{f(b)-f(a)}{b-a}\ \Rightarrow\ f'(c)=\frac{f(b)-f(a)}{b-a}\qquad\square$$

## Note collegate
- [[141_Teorema_di_Rolle]]
- [[143_Caratterizzazione_delle_Funzioni_Costanti_su_un_Intervallo]]
- [[140_Test_di_Monotonia]]
- [[131_Algebra_delle_Derivate]]
- [[00_MOC_Analisi_1]]
- [[144_Dimostrazione_del_Test_di_Monotonia]]
- [[149_Dimostrazione_del_Teorema_di_Prolungamento_della_Derivata]]

#AM1/derivate/lagrange
