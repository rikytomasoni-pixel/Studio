---
tags:
  - AM1
  - derivate
  - retta-tangente
  - tangente-verticale
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 14-16)"
---

# Derivata infinita e tangente verticale

> [!note] Osservazione
> Se $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$ e $f$ è **continua** in $x_0$, è interessante anche il caso in cui esista, infinito,
> $$\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}=\pm\infty$$
> In tal caso $f$ **non è derivabile** in $x_0$ ma, con abuso di notazione, scriveremo
> $$f'(x_0)=\pm\infty$$
> e la retta tangente al grafico di $f$ in $(x_0,f(x_0))=P_0$ risulta essere la **retta verticale** $x=x_0$.

## Esempio: $f(x)=\sqrt[3]{x}=x^{1/3}$, $x\in\mathbb{R}$, $x_0=0$
$f$ è continua in $\mathbb{R}$ e
$$f'(0)=\lim_{x\to0}\frac{f(x)-f(0)}{x}=\lim_{x\to0}\frac{x^{1/3}}{x}=\lim_{x\to0}x^{-2/3}=+\infty$$
Quindi $x=0$ è retta tangente verticale.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 15**: grafico di $x^{1/3}$, curva crescente che passa per l'origine con tangente verticale; l'asse $y$ (retta $x=0$) è evidenziato in rosso.

## Esempio: $f(x)=\operatorname{sgn}x=\begin{cases}-1&x<0\\0&x=0\\1&x>0\end{cases}$, $f:\mathbb{R}\to\mathbb{R}$, $x_0=0$
$f$ **non è continua** in $x_0=0$ (discontinuità a salto, [[97_Discontinuita_di_Prima_Specie_a_Salto]]).
$$\lim_{h\to0^\pm}\frac{f(h)-f(0)}{h}=\lim_{h\to0^\pm}\frac{\operatorname{sgn}h}{h}=\lim_{h\to0^\pm}\frac1{|h|}=+\infty$$
Non esiste retta tangente al grafico di $f$ in $(0,0)$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 16**: grafico di $\operatorname{sgn}x$: semiretta a quota $-1$ per $x<0$, semiretta a quota $1$ per $x>0$, punto pieno nell'origine.

## Note collegate
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[130_Classificazione_dei_Punti_di_Non_Derivabilita]] (flesso a tangente verticale e cuspide)
- [[97_Discontinuita_di_Prima_Specie_a_Salto]]
- [[90_Limite_Infinito_in_un_Punto_Finito]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/tangente-verticale
