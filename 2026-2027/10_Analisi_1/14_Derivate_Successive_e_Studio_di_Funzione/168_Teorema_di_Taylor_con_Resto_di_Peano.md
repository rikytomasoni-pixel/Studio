---
tags:
  - AM1
  - taylor
  - resto-di-peano
  - teorema
  - dimostrazione-richiesta
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 20-21)"
---

# Teorema di Taylor con resto in forma di Peano

> [!abstract] Teorema (di Taylor, con resto in forma di Peano) — **D24**
> Sia $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, $f$ derivabile $n$ volte in $x_0$, $n\ge1$. Allora per $x\to x_0$
> $$f(x)=P_n(x)+o\big((x-x_0)^n\big)=\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k+o\big((x-x_0)^n\big)$$
> cioè
> $$\lim_{x\to x_0}\frac{f(x)-P_n(x)}{(x-x_0)^n}=0$$

con $P_n$ [[167_Polinomio_di_Taylor|polinomio di Taylor]] di $f$ centrato in $x_0$ di ordine $n$.

> [!todo] Dimostrazione
> La dimostrazione non è presente negli appunti di L20; è nell'elenco delle dimostrazioni richieste allo scritto (**D24**): nota da integrare quando verrà svolta a lezione.

## Osservazioni

- $P_n(x)$ ha grado **al più** $n$, ma potrebbe avere grado inferiore, se $f^{(n)}(x_0)=0$.
- Se $n=1$
  $$P_1(x)=\sum_{k=0}^1\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k=f(x_0)+f'(x_0)(x-x_0)$$
  che è l'espressione analitica della **retta tangente** in $(x_0,f(x_0))$ al grafico di $f$ (e il teorema ridà la [[127_Differenziabilita_e_Approssimazione_Lineare|differenziabilità]]).

## Esempio

Con $f=\sin$, $x_0=0$, $n=3$: $\sin x=x-\frac{x^3}{6}+o(x^3)$ per $x\to0$ ([[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]], [[167_Polinomio_di_Taylor]]).

## Note collegate
- [[167_Polinomio_di_Taylor]]
- [[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]]
- [[127_Differenziabilita_e_Approssimazione_Lineare]]
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/peano
