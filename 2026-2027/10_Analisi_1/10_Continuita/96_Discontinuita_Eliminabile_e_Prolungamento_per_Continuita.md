---
tags:
  - AM1
  - continuita
  - discontinuita
  - discontinuita-eliminabile
  - definizione
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 13-15)"
---

# Classificazione dei punti di discontinuità — 1) discontinuità eliminabile

Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in I$, $x_0$ di accumulazione per $I$.

> [!abstract] Definizione — discontinuità eliminabile
> Se $\exists\displaystyle\lim_{x\to x_0}f(x)=\ell\in\mathbb{R}$, ma $\ell\neq f(x_0)$, diremo che $x_0$ è **punto di discontinuità eliminabile** per $f$.

> [!example] Esempio
> $f(x)=(\operatorname{sign}x)^2$, dove
> $$\operatorname{sign}(x)=\begin{cases}1&x>0\\0&x=0\\-1&x<0\end{cases}\quad\Rightarrow\quad f(x)=\begin{cases}1&x\neq0\\0&x=0\end{cases}$$
> e $\displaystyle\lim_{x\to0}f(x)=1\neq0=f(0)$.

È possibile **ridefinire** $f$ in $x_0$ ponendo
$$\tilde f(x)=\begin{cases}f(x)&x\neq x_0\\ \ell&x=x_0\end{cases}$$
La funzione così definita risulta continua in $x_0$ perché
$$\lim_{x\to x_0}\tilde f(x)=\lim_{x\to x_0}f(x)=\ell=\tilde f(x_0)$$

## Prolungamento per continuità
> [!note] Osservazione
> Se $f$ **non** è definita in $x_0$ ma esiste $\ell=\displaystyle\lim_{x\to x_0}f(x)\in\mathbb{R}$, si può **estendere per continuità** $f$ in $x_0$ ponendo
> $$\tilde f(x)=\begin{cases}f(x)&x\neq x_0\\ \ell&x=x_0\end{cases}$$
> La funzione $\tilde f$ ha dominio più grande del dominio di $f$ perché è definita anche in $x_0$, coincide con $f(x)$ sul dominio di $f$, ed è continua in $x_0$: $\displaystyle\lim_{x\to x_0}\tilde f(x)=\lim_{x\to x_0}f(x)=\ell=\tilde f(x_0)$.

> [!example] Esempio
> Vedremo ad esempio ([[108_Limiti_Notevoli_di_Funzioni]]) che $\displaystyle\lim_{x\to0}\frac{\sin x}{x}=1$, quindi si può estendere $f(x)=\dfrac{\sin x}{x}$ per continuità in $x_0=0$ ponendo $f(0)=1$.

## Note collegate
- [[93_Continuita_in_un_Punto]]
- [[97_Discontinuita_di_Prima_Specie_a_Salto]]
- [[98_Discontinuita_di_Seconda_Specie]]
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/continuita/discontinuita-eliminabile
