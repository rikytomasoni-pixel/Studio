---
tags:
  - AM1
  - limiti-di-funzioni
  - limiti-notevoli
  - asintotico
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 11-15)"
---

# Limiti notevoli di funzioni

*(dimostrazioni in seguito: vedi [[118_Dimostrazione_dei_Limiti_Notevoli]])*

Per $x\to0$:

1. $\displaystyle\lim_{x\to0}\frac{\sin x}{x}=1$ $\qquad\sin x\sim x\qquad\sin x=x+o(x)$
2. $\displaystyle\lim_{x\to0}\frac{1-\cos x}{x^2}=\frac12$ $\qquad1-\cos x\sim\tfrac12x^2\qquad1-\cos x=\tfrac12x^2+o(x^2)\qquad\cos x=1-\tfrac12x^2+o(x^2)$
3. $\displaystyle\lim_{x\to\pm\infty}\Big(1+\frac1x\Big)^x=e$
4. $\displaystyle\lim_{x\to0}\frac{\log(1+x)}{x}=1$ $\qquad\log(1+x)\sim x\qquad\log(1+x)=x+o(x)$
5. $\displaystyle\lim_{x\to0}\frac{e^x-1}{x}=1$ $\qquad e^x-1\sim x\qquad e^x-1=x+o(x)\qquad e^x=1+x+o(x)$
6. $\displaystyle\lim_{x\to0}\frac{(1+x)^\alpha-1}{x}=\alpha\quad\forall\alpha\in\mathbb{R}$ $\qquad(\alpha\neq0)$: $(1+x)^\alpha-1\sim\alpha x\qquad(1+x)^\alpha-1=\alpha x+o(x)\qquad(1+x)^\alpha=1+\alpha x+o(x)$
7. $\displaystyle\lim_{x\to0}\frac{\tan x}{x}=1$ $\qquad\tan x\sim x\qquad\tan x=x+o(x)$
8. $\displaystyle\lim_{x\to0}\frac{\arctan x}{x}=1$ $\qquad\arctan x\sim x\qquad\arctan x=x+o(x)$

$\dots$

## Versione con funzione infinitesima $\varepsilon(x)$
> [!note] Osservazione
> Dalle formule precedenti e dal [[104_Cambio_di_Variabile_nei_Limiti|teorema di cambio di variabile nei limiti]] segue che se $\varepsilon(x)$ è una funzione tale che
> $$\lim_{x\to x_0}\varepsilon(x)=0\qquad x_0\in\overline{\mathbb{R}}\quad(\text{con }\varepsilon(x)\neq0\text{ definitivamente per }x\to x_0)$$
> allora per $x\to x_0$
> $$\lim\frac{\sin\varepsilon(x)}{\varepsilon(x)}\overset{t=\varepsilon(x)}{=}\lim_{t\to0}\frac{\sin t}{t}=1\ \Rightarrow\ \sin\varepsilon(x)\sim\varepsilon(x),\quad\sin\varepsilon(x)=\varepsilon(x)+o(\varepsilon(x))$$
> Similmente per gli altri limiti notevoli:
> $$1-\cos\varepsilon(x)\sim\tfrac12\varepsilon(x)^2,\quad\log(1+\varepsilon(x))\sim\varepsilon(x),\quad e^{\varepsilon(x)}-1\sim\varepsilon(x),\quad(1+\varepsilon(x))^\alpha-1\sim\alpha\varepsilon(x)\ (\alpha\neq0)$$

In particolare se $\varepsilon_n$ è una **successione infinitesima**, cioè $\displaystyle\lim_{n\to\infty}\varepsilon_n=0$ (con $\varepsilon_n\neq0$ definitivamente in $n\in\mathbb{N}$), si ritrovano gli asintotici notevoli per successioni già visti ([[46_Asintotici_Notevoli_e_Limiti_Notevoli]]):
$$\sin\varepsilon_n\sim\varepsilon_n,\quad1-\cos\varepsilon_n\sim\tfrac12\varepsilon_n^2,\quad\log(1+\varepsilon_n)\sim\varepsilon_n,\quad e^{\varepsilon_n}-1\sim\varepsilon_n,\quad(1+\varepsilon_n)^\alpha-1\sim\alpha\varepsilon_n\ (\alpha\neq0)\qquad\dots\quad\text{per }n\to\infty$$

## Note collegate
- [[46_Asintotici_Notevoli_e_Limiti_Notevoli]] (versione per successioni)
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[107_Proprieta_degli_Asintotici_per_Funzioni]]
- [[118_Dimostrazione_dei_Limiti_Notevoli]]
- [[38_Numero_di_Nepero]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/limiti-notevoli
