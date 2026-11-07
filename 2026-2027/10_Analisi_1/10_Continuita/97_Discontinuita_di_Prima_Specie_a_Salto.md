---
tags:
  - AM1
  - continuita
  - discontinuita
  - discontinuita-a-salto
  - definizione
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 15-16)"
---

# Classificazione dei punti di discontinuità — 2) discontinuità di I specie (a salto)

> [!abstract] Definizione — discontinuità di I specie (tipo salto)
> Se $\exists\displaystyle\lim_{x\to x_0^-}f(x)=\ell_1\in\mathbb{R}$ e $\displaystyle\lim_{x\to x_0^+}f(x)=\ell_2\in\mathbb{R}$, ma $\ell_1\neq\ell_2$, allora $x_0$ è **punto di discontinuità di I specie** o **di tipo salto** per $f$, con **salto**
> $$s(x_0)=\ell_2-\ell_1$$

- Se $f(x_0)=\displaystyle\lim_{x\to x_0^+}f(x)=\ell_2$ diremo che $f$ è **continua da destra** in $x_0$.
- Se $f(x_0)=\displaystyle\lim_{x\to x_0^-}f(x)=\ell_1$ diremo che $f$ è **continua da sinistra** in $x_0$.

> [!example] Esempio — $f(x)=\operatorname{sign}x$
> $f$ ha discontinuità a salto in $x_0=0$ con salto pari a $+2$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L14 pag. 16: grafico di $\operatorname{sign}x$: semiretta orizzontale a quota $-1$ per $x<0$, punto $(0,0)$ evidenziato in rosso, semiretta a quota $1$ per $x>0$.

> [!example] Esempio — funzione indicatrice di $(a,b)$
> $$f(x)=\begin{cases}1&x\in(a,b)\\0&x\notin(a,b)\end{cases}$$
> $f$ è discontinua in $a,b$, con discontinuità a salto e salto $+1$ e $-1$ rispettivamente.

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L14 pag. 16: grafico a "gradino" in rosso: tratto a quota $1$ tra $a$ e $b$, quota $0$ altrove.

> [!note] Osservazione (non presente negli appunti)
> Nell'ultimo esempio $f(a)=0=\displaystyle\lim_{x\to a^-}f(x)$ e $f(b)=0=\displaystyle\lim_{x\to b^+}f(x)$: $f$ è quindi continua da sinistra in $a$ e continua da destra in $b$.

## Note collegate
- [[93_Continuita_in_un_Punto]]
- [[91_Limiti_Destro_e_Sinistro_e_Asintoto_Verticale]]
- [[96_Discontinuita_Eliminabile_e_Prolungamento_per_Continuita]]
- [[98_Discontinuita_di_Seconda_Specie]]
- [[115_Teorema_sui_Limiti_di_Funzioni_Monotone]] (le funzioni monotone hanno solo discontinuità a salto)
- [[00_MOC_Analisi_1]]

#AM1/continuita/discontinuita-a-salto
