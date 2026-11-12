---
tags:
  - AM1
  - derivate
  - non-derivabilita
  - punto-angoloso
  - cuspide
  - flesso-a-tangente-verticale
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 25-29)"
---

# Classificazione dei punti di non derivabilità

Sia $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$, $f$ **continua** in $x_0$. Si usano le derivate destra e sinistra di [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]].

## Punto angoloso
> [!abstract] Definizione — punto angoloso
> Se esistono **finiti**
> $$f'_+(x_0)=\lim_{h\to0^+}\frac{f(x_0+h)-f(x_0)}{h}\in\mathbb{R}\qquad f'_-(x_0)=\lim_{h\to0^-}\frac{f(x_0+h)-f(x_0)}{h}\in\mathbb{R}$$
> ma $f'_+(x_0)\neq f'_-(x_0)$, $x_0$ si dice **punto angoloso** per $f$.

Esempio: $f(x)=|x|$, $x_0=0$: $1=f'_+(0)\neq f'_-(0)=-1$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 25**: grafico di $|x|$ (a V con vertice nell'origine) con $f'_+(0)=1$ e $f'_-(0)=-1$.

## Flesso a tangente verticale
> [!abstract] Definizione — flesso a tangente verticale
> Se esiste infinito
> $$f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}=\pm\infty$$
> diremo che $x_0$ è **punto di flesso a tangente verticale**, e $x=x_0$ è la retta tangente al grafico di $f$ in $P_0=(x_0,f(x_0))$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 26**: due grafici con retta verticale blu $x=x_0$ tangente nel punto: a sinistra curva crescente (caso $+\infty$), a destra curva decrescente (caso $-\infty$).

Esempio: $f(x)=x^{1/3}$, $f:\mathbb{R}\to\mathbb{R}$, $x_0=0$:
$$f'(0)=\lim_{h\to0}\frac{h^{1/3}}h=\lim_{h\to0}\frac1{h^{2/3}}=+\infty$$
con $f$ continua in $\mathbb{R}$ (vedi [[125_Derivata_Infinita_e_Tangente_Verticale]]).

## Cuspide
> [!abstract] Definizione — cuspide
> Se esistono infiniti e **discordi** in segno
> $$f'_+(x_0)=\lim_{h\to0^+}\frac{f(x_0+h)-f(x_0)}{h}=\pm\infty\qquad f'_-(x_0)=\lim_{h\to0^-}\frac{f(x_0+h)-f(x_0)}{h}=\mp\infty$$
> allora $x_0$ si dice **cuspide** per $f$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 27**: due grafici con cuspide in $x_0$. A sinistra la cuspide è un minimo a punta verso il basso (indicato "$-\infty/+\infty$", cioè $f'_-=-\infty$, $f'_+=+\infty$); a destra la cuspide è un massimo a punta verso l'alto (indicato "$+\infty/-\infty$").

Esempio: $f(x)=\sqrt{|x|}$, $f:\mathbb{R}\to\mathbb{R}$, $x_0=0$, $f$ continua:
$$f'_\pm(0)=\lim_{h\to0^\pm}\frac{f(h)-f(0)}h=\lim_{h\to0^\pm}\frac{|h|^{1/2}}h=\lim_{h\to0^\pm}\underbrace{\operatorname{sgn}h}_{\pm1}\cdot\underbrace{\frac1{|h|^{1/2}}}_{\to+\infty}=\pm\infty$$

## Altri casi
> [!note] Osservazione
> Se $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$, $f$ è continua in $x_0$ e
> - $\exists f'_+(x_0),f'_-(x_0)$ di cui **una finita e una infinita**, diremo che $x_0$ è un **punto angoloso** per $f$;
> - se $\nexists f'_+(x_0)$ oppure $\nexists f'_-(x_0)$, diremo solo che $f$ **non è derivabile** in $x_0$.

**Esempio.** $f(x)=\begin{cases}x\sin\frac1x&x\neq0\\0&x=0\end{cases}$, $x_0=0$. $f$ è continua in $\mathbb{R}$; per $x_0=0$
$$\lim_{x\to0}x\sin\frac1x=0=f(0)\quad(\text{infinitesima per limitata})$$
Ma $f$ non è derivabile in $x_0=0$:
$$\lim_{h\to0^\pm}\frac{f(h)-f(0)}h=\lim_{h\to0^\pm}\sin\frac1h\overset{t=\frac1h}{=}\lim_{t\to\pm\infty}\sin t\quad\nexists$$

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 29**: grafico di $x\sin\frac1x$ che oscilla (in rosso) tra le rette $y=x$ e $y=-x$ (in blu), con oscillazioni sempre più fitte vicino all'origine.

## Note collegate
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[125_Derivata_Infinita_e_Tangente_Verticale]]
- [[129_Derivabilita_e_Continuita]]
- [[123_Esempi_di_Derivata_e_Retta_Tangente]]
- [[93_Continuita_in_un_Punto]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/non-derivabilita
