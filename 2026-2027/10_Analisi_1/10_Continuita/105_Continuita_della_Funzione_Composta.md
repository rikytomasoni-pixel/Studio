---
tags:
  - AM1
  - continuita
  - funzione-composta
  - corollario
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 4-5)"
---

# Continuità della funzione composta

> [!abstract] Corollario
> Sia $g$ definita in un intorno di $x_0$ e continua in $x_0$, $\displaystyle\lim_{x\to x_0}g(x)=g(x_0)$; sia $f$ definita in un intorno di $t_0=g(x_0)$ e continua in $t_0$, $\displaystyle\lim_{t\to t_0}f(t)=f(t_0)$.
> Allora $f\circ g(x)$ è definita in un intorno di $x_0$ ed è continua in $x_0$:
> $$\lim_{x\to x_0}f(g(x))=f(g(x_0))$$

**Dimostrazione.** Per il [[104_Cambio_di_Variabile_nei_Limiti|teorema di cambio di variabile nei limiti]], essendo entrambe le funzioni continue,
$$\lim_{x\to x_0}f(g(x))\overset{t=g(x)}{=}\lim_{t\to t_0}f(t)=f(t_0)=f(g(x_0))\qquad\square$$

> [!note] Osservazione
> Se $f$ è continua in $t_0$:
> $$\lim_{x\to x_0}f(g(x))=\lim_{t\to t_0}f(t)=f(t_0)=f\Big(\lim_{x\to x_0}g(x)\Big)$$

## Note collegate
- [[103_Algebra_delle_Funzioni_Continue]]
- [[93_Continuita_in_un_Punto]]
- [[117_Continuita_delle_Funzioni_Elementari]]
- [[25_Composizione_di_Funzioni]]
- [[00_MOC_Analisi_1]]
- [[132_Regola_della_Catena]] (versione per le derivate)

#AM1/continuita/funzione-composta
