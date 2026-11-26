---
tags:
  - AM1
  - taylor
  - resto-di-lagrange
  - teorema
  - formula-di-maclaurin
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 11-13)"
---

# Teorema di Taylor con resto in forma di Lagrange

> [!abstract] Teorema (di Taylor, con resto in forma di Lagrange)
> Sia $f:[a,b]\to\mathbb{R}$ derivabile $(n+1)$ volte in $[a,b]$, $n\in\mathbb{N}$, $x_0\in[a,b]$. Allora per ogni $x\in[a,b]$ esiste $c$ compreso tra $x$ e $x_0$ ($c$ dipende da $n,x_0,x$) tale che
> $$f(x)=P_n(x)+\frac{f^{(n+1)}(c)}{(n+1)!}(x-x_0)^{n+1}=\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k+\frac{f^{(n+1)}(c)}{(n+1)!}(x-x_0)^{n+1}$$

*(negli appunti: "no dim.")*

## Osservazioni

- La formula si chiama **formula di Taylor centrata in $x_0$** (di **Mac Laurin** se $x_0=0$) **di ordine $n$** per $f$, **con resto di Lagrange**.
- Per $n=0$ diventa
  $$f(x)=f(x_0)+f'(c)(x-x_0)\iff\frac{f(x)-f(x_0)}{x-x_0}=f'(c)$$
  cioè è sostanzialmente il [[142_Teorema_di_Lagrange|teorema del valor medio di Lagrange]].
- Rispetto al [[168_Teorema_di_Taylor_con_Resto_di_Peano|resto di Peano]] (informazione **locale**, $o((x-x_0)^n)$) il resto di Lagrange dà un'espressione **esatta** su tutto l'intervallo, utile per **stimare l'errore** ([[175_Esempio_Stima_del_Resto_di_e_alla_x]]).
- Si può dimostrare che $e\notin\mathbb{Q}$ tramite il teorema di Taylor-Lagrange.

## Note collegate
- [[167_Polinomio_di_Taylor]]
- [[168_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[142_Teorema_di_Lagrange]]
- [[175_Esempio_Stima_del_Resto_di_e_alla_x]]
- [[38_Numero_di_Nepero]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/lagrange
