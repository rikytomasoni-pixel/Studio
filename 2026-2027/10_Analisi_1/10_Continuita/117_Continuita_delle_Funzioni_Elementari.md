---
tags:
  - AM1
  - continuita
  - funzioni-elementari
  - corollario
data: 2026-11-06
lezione: 16
fonte: "AM1 L16 26-27.pdf (pag. 14-19)"
---

# Continuità delle funzioni elementari

> [!abstract] Corollario
> Le funzioni elementari sono continue **sui loro domini**.

| Funzione | Perché è continua |
|---|---|
| $f(x)=x$ | ovvio |
| $f(x)=\lambda$, $\lambda\in\mathbb{R}$ | ovvio |
| $f(x)=x^m$, $\forall m\in\mathbb{N}$ | prodotto di funzioni continue |
| polinomi | somma e prodotto di funzioni continue |
| $f(x)=\dfrac1{x^m}$, $\forall m\in\mathbb{N}$ | reciproco di funzioni continue |
| $f(x)=x^{1/m}$, $\forall m\in\mathbb{N}$, $m\ge1$ | inversa di funzione continua su un intervallo |
| $f(x)=x^{n/m}$, $\forall n,m\in\mathbb{Z}$, $m\neq0$ | composizione di funzioni continue |
| $f(x)=e^x$ | continua (vedi lezioni passate: [[94_Esempio_Continuita_di_e_alla_x]]) |
| $f(x)=\log x$ | inversa di funzione continua su intervallo |
| $f(x)=a^x=e^{\log a^x}=e^{(\log a)\cdot x}$, $a>0$, $a\neq1$ | composizione di funzioni continue |
| $f(x)=\log_ax$, $a>0$, $a\neq1$ | inversa di funzione continua su intervallo |
| $f(x)=x^\alpha=e^{\log x^\alpha}=e^{\alpha\log x}$, $\alpha\in\mathbb{R}$ | composizione di funzioni continue |
| $\sin x$, $\cos x$ | vedi sotto |
| $\arcsin x$, $\arccos x$ | inverse di funzioni continue su intervalli |
| $\tan x=\dfrac{\sin x}{\cos x}$ | quoziente di funzioni continue |
| $\arctan x$ | inversa di funzione continua su intervallo |

$\dots$

## Continuità di $\sin x$ e $\cos x$
> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L16 pag. 16: circonferenza goniometrica con centro $O$, punto $A=(1,0)$, punto $P$ sulla circonferenza nel primo quadrante, $H$ proiezione di $P$ sull'asse $x$, $K$ proiezione di $P$ sull'asse $y$, angolo $x$ in $O$; segmento $\overline{PH}=\sin x$ e arco $\widehat{PA}=x$.

Per $x\ge0$: $\overline{PH}=\sin x$, $\ \widehat{PA}=x$, quindi
$$0\le\sin x\le x\quad\forall x\in\Big[0,\frac\pi2\Big)\ \Rightarrow\ 0\le|\sin x|\le|x|\quad\forall x\in\Big(-\frac\pi2,\frac\pi2\Big)$$
$$\Rightarrow\ \text{per confronto (due carabinieri)}\quad\lim_{x\to0}\sin x=0=\sin0\ \Rightarrow\ \sin x\text{ è continua in }x=0$$
Inoltre $\cos x=1-2\big(\sin\frac x2\big)^2$ e quindi, per algebra dei limiti,
$$\lim_{x\to0}\cos x=1=\cos0\ \Rightarrow\ \cos x\text{ è continua in }x=0$$
Inoltre $\forall x_0\in\mathbb{R}$, $\forall h\in\mathbb{R}$
$$\sin(x_0+h)=\sin x_0\cos h+\cos x_0\sin h\ \Rightarrow\ \lim_{h\to0}\sin(x_0+h)=\sin x_0\ \Rightarrow\ \sin x\text{ è continua in }x=x_0\in\mathbb{R}$$
$$\cos(x_0+h)=\cos x_0\cos h-\sin x_0\sin h\ \Rightarrow\ \lim_{h\to0}\cos(x_0+h)=\cos x_0\ \Rightarrow\ \cos x\text{ è continua in }x=x_0\in\mathbb{R}$$

## Note collegate
- [[116_Continuita_e_Invertibilita]]
- [[103_Algebra_delle_Funzioni_Continue]]
- [[105_Continuita_della_Funzione_Composta]]
- [[94_Esempio_Continuita_di_e_alla_x]]
- [[100_Teorema_del_Confronto_per_Limiti_di_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/continuita/funzioni-elementari
