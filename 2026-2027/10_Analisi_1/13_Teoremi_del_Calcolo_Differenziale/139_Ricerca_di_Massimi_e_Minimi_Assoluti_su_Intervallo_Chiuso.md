---
tags:
  - AM1
  - derivate
  - estremi
  - weierstrass
  - esercizi
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 12-15)"
---

# Ricerca di massimi e minimi assoluti su un intervallo chiuso

Si possono combinare il [[112_Teorema_di_Weierstrass]] e il [[137_Teorema_di_Fermat]] per studiare massimi e minimi **assoluti** (non locali) di una funzione $f:[a,b]\subseteq\mathbb{R}\to\mathbb{R}$ continua.

Per Weierstrass i punti di massimo e di minimo globali esistono in $[a,b]$. Per Fermat tali punti possono trovarsi solamente in:
1. un **punto stazionario** di $f$, cioè in un punto $x_0\in(a,b)$ dove $f$ sia derivabile e $f'(x_0)=0$;
2. un punto $x_0\in(a,b)$ dove $f$ **non** sia derivabile;
3. uno degli **estremi** $a,b$ dell'intervallo.

Tra questi punti, dove $f$ assume il valore più grande sarà punto di massimo assoluto, dove assume il valore più piccolo sarà punto di minimo assoluto.

## Esempio
$f:[-2,3]\to\mathbb{R}$, $\ f(x)=\dfrac12|x|+e^{-x}$.

- $f$ è continua perché somma e composizione di funzioni continue.
- $f$ è derivabile per ogni $x\neq0$ perché somma e composizione di funzioni derivabili per $x\neq0$.
- Per Weierstrass massimo e minimo globali esistono in $[-2,3]$.
- Per $x\neq0$:
$$f'(x)=\frac12\operatorname{sgn}x-e^{-x}=\begin{cases}\frac12-e^{-x}&x\in(0,3]\\-\frac12-e^{-x}&x\in[-2,0)\end{cases}$$
- $\nexists f'(0)$: $f'_+(0)=-\frac12$, $f'_-(0)=-\frac32$.
- $f'(x)=0$ se e solo se $x>0$ e $\frac12-e^{-x}=0$, se e solo se $x=\log2\in(0,3)$.
- I possibili punti di estremo per $f$ in $[-2,3]$ sono quindi
  - $\log2$ (punto stazionario),
  - $0$ (punto di non derivabilità),
  - $-2,\,3$ (estremi dell'intervallo).

Valori di $f$ nei candidati:
$$f(-2)=1+e^2\qquad f(3)=\frac32+e^{-3}\qquad f(\log2)=\frac12(\log2+1)\qquad f(0)=1$$
Il valore più grande è $1+e^2=f(-2)$, il più piccolo è $\frac12(\log2+1)=f(\log2)$. Quindi
$$\max_{[-2,3]}f(x)=f(-2)=1+e^2\qquad\min_{[-2,3]}f(x)=f(\log2)=\frac12(\log2+1)$$

## Note collegate
- [[112_Teorema_di_Weierstrass]]
- [[137_Teorema_di_Fermat]]
- [[138_Punti_Stazionari_e_Punti_Critici]]
- [[136_Massimi_e_Minimi_Locali_e_Globali]]
- [[133_Derivate_con_Valore_Assoluto_e_Segno]]
- [[114_Immagine_di_una_Funzione_Continua_su_un_Intervallo_Chiuso]]
- [[00_MOC_Analisi_1]]
- [[146_Test_di_Monotonia_e_Estremi_Locali]]

#AM1/derivate/massimi-minimi-assoluti
