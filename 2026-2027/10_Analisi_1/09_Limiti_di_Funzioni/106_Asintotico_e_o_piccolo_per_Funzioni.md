---
tags:
  - AM1
  - limiti-di-funzioni
  - asintotico
  - o-piccolo
  - infinitesimo
  - definizione
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 6-8)"
---

# Asintotico e o piccolo per funzioni

Estensione ai limiti di funzioni di quanto visto per le successioni ([[40_Confronti_Asintotici]], [[41_o_piccolo_e_Asintotico]]).

> [!abstract] Definizione
> Date due funzioni $f,g$ e $x_0\in\overline{\mathbb{R}}$, diremo che
> - $f(x)\sim g(x)$ per $x\to x_0$ se $\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=1$
> - $f(x)=o(g(x))$ per $x\to x_0$ se $\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=0$

> [!abstract] Definizione — infinitesima e infinita
> Data una funzione $f$ e $x_0\in\overline{\mathbb{R}}$, diremo che
> - $f$ è **infinitesima** per $x\to x_0$ se $\displaystyle\lim_{x\to x_0}f(x)=0$
> - $f$ è **infinita** per $x\to x_0$ se $\displaystyle\lim_{x\to x_0}f(x)=\infty$

> [!note] Osservazioni
> - Se $\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=\lambda\in\mathbb{R}\setminus\{0\}$, allora $\displaystyle\lim_{x\to x_0}\frac{f(x)}{\lambda g(x)}=1$, quindi $f(x)\sim\lambda g(x)$ per $x\to x_0$.
> - Se $\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=\infty$, allora $\displaystyle\lim_{x\to x_0}\frac{g(x)}{f(x)}=0$, quindi $g(x)=o(f(x))$ per $x\to x_0$.

> [!note] Osservazione — asintotico e o piccolo
> $f(x)\sim g(x)$ per $x\to x_0$ se e solo se $f(x)=g(x)+o(g(x))$ per $x\to x_0$. Infatti
> $$f\sim g\iff\lim\frac{f}{g}=1\iff\lim\Big(\frac fg-1\Big)=0\iff\lim\frac{f-g}{g}=0\iff f-g=o(g)\iff f=g+o(g)$$
> (tutti i limiti per $x\to x_0$).

## Note collegate
- [[107_Proprieta_degli_Asintotici_per_Funzioni]]
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[40_Confronti_Asintotici]]
- [[41_o_piccolo_e_Asintotico]]
- [[00_MOC_Analisi_1]]
- [[127_Differenziabilita_e_Approssimazione_Lineare]] (derivabilità riscritta con l'o piccolo)

#AM1/limiti-di-funzioni/asintotico-o-piccolo
