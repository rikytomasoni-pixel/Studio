---
tags:
  - AM1
  - taylor
  - resto-di-lagrange
  - esempio
  - stima-dell-errore
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 12)"
---

# Esempio: stima del resto di $e^x$ con Lagrange

Sia $f(x)=e^x$, $n=18$, intervallo $[-1,43]$, $x_0=0$. Per il [[174_Teorema_di_Taylor_con_Resto_di_Lagrange|teorema di Taylor con resto di Lagrange]], per ogni $x$ dell'intervallo esiste $c$ tra $0$ e $x$ tale che
$$e^x=\sum_{k=0}^{18}\frac{x^k}{k!}+\frac{e^c}{19!}x^{19}$$

Quindi
$$|\text{Resto}|=\big|e^x-P_{18}(x)\big|=\frac{e^c}{19!}|x|^{19}\le\frac{e^{43}\cdot43^{19}}{19!}$$
perché $c\le43$ (e $e^c$ è crescente) e $|x|\le43$.

> [!note] Osservazione (non presente negli appunti)
> Il quaderno scrive l'intervallo come $[-1,43]$ e maggiora con $x=43$: la maggiorazione vale perché $e^c\le e^{43}$ e $|x|\le 43$ su tutto l'intervallo.

## Note collegate
- [[174_Teorema_di_Taylor_con_Resto_di_Lagrange]]
- [[172_Sviluppi_di_Maclaurin_di_e_alla_x_sin_cos]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/stima-resto
