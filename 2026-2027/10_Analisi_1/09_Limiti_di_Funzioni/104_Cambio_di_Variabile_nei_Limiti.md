---
tags:
  - AM1
  - limiti-di-funzioni
  - cambio-di-variabile
  - teorema
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 3-4)"
---

# Teorema di cambio di variabile nei limiti

> [!abstract] Teorema
> Siano $f,g$ due funzioni per cui sia ben definita la composizione
> $$f\circ g(x)=f(g(x))$$
> almeno in un intorno $\mathcal{U}(x_0)$ di $x_0$ in $\overline{\mathbb{R}}$, escluso al più $x_0$. Se
> 1. $\displaystyle\lim_{x\to x_0}g(x)=t_0\in\overline{\mathbb{R}}$
> 2. $\displaystyle\lim_{t\to t_0}f(t)=\ell\in\overline{\mathbb{R}}$
> 3. $g(x)\neq t_0$ definitivamente per $x\to x_0$
>
> allora
> $$\lim_{x\to x_0}f(g(x))=\lim_{t\to t_0}f(t)=\ell\qquad(t=g(x))$$

*Senza dimostrazione.*

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L15 pag. 4: schema con due ovali: nel primo il punto $x_0$, nel secondo il punto $t_0$, freccia $t=g(x)$ dal primo al secondo e freccia $f$ dal secondo verso $\mathbb{R}$.

> [!note] Osservazione
> L'ipotesi 3) **non serve** se $t_0=\pm\infty$ o se $f$ è continua in $t_0$, cioè $\ell=f(t_0)$.

## Note collegate
- [[105_Continuita_della_Funzione_Composta]] (corollario)
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[109_Gerarchia_degli_Infiniti_per_Funzioni]]
- [[118_Dimostrazione_dei_Limiti_Notevoli]]
- [[25_Composizione_di_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/cambio-di-variabile
