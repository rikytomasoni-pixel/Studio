---
tags:
  - AM1
  - successioni
  - asintotico
  - limiti
  - logaritmo
  - esempio
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 5-6)"
---

# Esempio: limite con asintotici, logaritmo e arctan

## Esempio
$$a_n=\frac{\log(1+e^n)\,\log\left(\cos\frac1n\right)}{\arctan n\ \sin\frac2n}$$

> [!abstract] Regola (annotazione in rosso)
> Se $a_n\to\ell$, $\ell\neq1$ e $a_n\sim a_n'$ $\Rightarrow$ $\log a_n\sim\log a_n'$

(Confronta con l'avvertimento di [[42_Confronti_Asintotici_Proprieta_e_Notevoli]]: in generale $\log a_n\sim\log a_n'$ non è garantito; la condizione è $\ell\neq1$.)

## Sviluppo dei singoli fattori
- $\log(1+e^n)=\log\left(e^n(1+e^{-n})\right)=\log e^n+\log(1+e^{-n})=n+e^{-n}+o(e^{-n})\sim n$

- $\log\left(\cos\frac1n\right)=\log\left(1+\left(\cos\frac1n-1\right)\right)\sim\cos\frac1n-1\sim-\frac1{2n^2}$
  perché $\frac1n$ e $\cos\frac1n-1$ sono infinitesimi.

- $\sin\frac2n\sim\frac2n$ perché $\frac2n\to0$

- $\arctan n\sim\frac\pi2$

## Conclusione
$$\Rightarrow a_n\sim\frac{\not n\cdot\left(-\frac1{2n^{\not2}}\right)}{\frac\pi2\cdot\frac{\not2}{\not n}}=-\frac1{2\pi}\ \Rightarrow\ \lim_{n\to\infty}a_n=-\frac1{2\pi}$$

Più precisamente: $a_n\sim\dfrac{n\cdot\left(-\frac1{2n^2}\right)}{\frac\pi2\cdot\frac2n}=-\dfrac{1}{2\pi}$.

## Note collegate
- [[43_Asintotici_con_Funzioni_Composte]]
- [[46_Asintotici_Notevoli_e_Limiti_Notevoli]]
- [[42_Confronti_Asintotici_Proprieta_e_Notevoli]]
- [[41_o_piccolo_e_Asintotico]]
- [[00_MOC_Analisi_1]]

#AM1/successioni-e-limiti/esempio-asintotici-logaritmo-arctan
