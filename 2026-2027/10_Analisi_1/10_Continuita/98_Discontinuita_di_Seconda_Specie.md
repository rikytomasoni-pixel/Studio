---
tags:
  - AM1
  - continuita
  - discontinuita
  - definizione
  - esempio
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 16-18)"
---

# Classificazione dei punti di discontinuità — 3) discontinuità di II specie

> [!abstract] Definizione — discontinuità di II specie
> Se $\exists\displaystyle\lim_{x\to x_0^-}f(x)=\ell_1$ e $\displaystyle\lim_{x\to x_0^+}f(x)=\ell_2$ con almeno uno dei due infinito, oppure se $\nexists$ almeno uno dei due limiti $\displaystyle\lim_{x\to x_0^+}f(x)$, $\displaystyle\lim_{x\to x_0^-}f(x)$ in $\overline{\mathbb{R}}$, allora $x_0$ si dice **punto di discontinuità di II specie**.

## Esempi (con $a\in\mathbb{R}$ valore arbitrario in $x=0$)

> [!example] $f(x)=\begin{cases}\frac1x&x\neq0\\a&x=0\end{cases}$
> > [!warning] DISEGNO NON RAPPRESENTABILE
> > AM1 L14 pag. 17: grafico di $1/x$ in rosso (ramo positivo a destra, ramo negativo a sinistra) e punto isolato in $(0,a)$ sull'asse $y$.

> [!example] $f(x)=\begin{cases}\frac1{x^2}&x\neq0\\a&x=0\end{cases}$
> > [!warning] DISEGNO NON RAPPRESENTABILE
> > AM1 L14 pag. 17: grafico di $1/x^2$ (due rami sopra l'asse $x$) e punto isolato $(0,a)$ (disegnato sotto l'asse $x$).

> [!example] $f(x)=\begin{cases}e^{1/x}&x\neq0\\a&x=0\end{cases}$
> > [!warning] DISEGNO NON RAPPRESENTABILE
> > AM1 L14 pag. 17: grafico di $e^{1/x}$: per $x>0$ ramo che sale verso l'alto vicino a $0$ e si avvicina a quota $1$ (tratteggio azzurro) per $x\to+\infty$; per $x<0$ ramo sotto la quota $1$ che arriva all'origine con un cerchietto vuoto; punto isolato $(0,a)$.

> [!example] $f(x)=\begin{cases}\sin\frac1x&x\neq0\\a&x=0\end{cases}$
> > [!warning] DISEGNO NON RAPPRESENTABILE
> > AM1 L14 pag. 18: grafico di $\sin(1/x)$ che oscilla rapidamente tra $-1$ e $1$ avvicinandosi a $x=0$ (disegnato per $x>0$, con due rette azzurre a quote $\pm1$).

> [!note] Osservazione (non presente negli appunti)
> Per leggere i limiti dai grafici: in $e^{1/x}$ si ha $\lim_{x\to0^+}=+\infty$ e $\lim_{x\to0^-}=0$; in $1/x$ i limiti laterali sono $+\infty$ e $-\infty$; in $1/x^2$ entrambi $+\infty$; in $\sin\frac1x$ nessuno dei due limiti laterali esiste (oscillazione). In tutti i casi il valore $a$ assegnato in $0$ non cambia il tipo di discontinuità.

## Note collegate
- [[93_Continuita_in_un_Punto]]
- [[95_Funzione_di_Dirichlet]]
- [[96_Discontinuita_Eliminabile_e_Prolungamento_per_Continuita]]
- [[97_Discontinuita_di_Prima_Specie_a_Salto]]
- [[91_Limiti_Destro_e_Sinistro_e_Asintoto_Verticale]]
- [[00_MOC_Analisi_1]]

#AM1/continuita/discontinuita-seconda-specie
