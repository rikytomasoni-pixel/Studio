---
tags:
  - AM1
  - continuita
  - esempio
  - esponenziale
data: 2026-10-28
lezione: 14
fonte: "AM1 L14 26-27.pdf (pag. 9-11)"
---

# Esempio: $e^x$ è continua in ogni punto

Sia $f(x)=e^x$.

## Caso $x_0=0$
$f(0)=1$. Verifichiamo che $e^x$ è continua in $0$. Fissiamo $\varepsilon>0$ (con $\varepsilon\in(0,1)$):
$$1-\varepsilon<e^x<1+\varepsilon\iff\begin{cases}e^x<1+\varepsilon\\ e^x>1-\varepsilon\end{cases}\iff\begin{cases}x<\log(1+\varepsilon)\\ x>\log(1-\varepsilon)\end{cases}$$
cioè $\log(1-\varepsilon)<x<\log(1+\varepsilon)$, con $\log(1-\varepsilon)\in(-\infty,0)$ e $\log(1+\varepsilon)\in(0,\infty)$. Sulla retta: $-\log\frac1{1-\varepsilon}<0<\log(1+\varepsilon)$.

Con
$$\delta=\min\Big\{\log(1+\varepsilon),\ \log\big((1-\varepsilon)^{-1}\big)\Big\}>0$$
allora
$$x\in(-\delta,\delta)\ \Rightarrow\ x\in\big(\log(1-\varepsilon),\log(1+\varepsilon)\big)\ \Rightarrow\ e^x\in(1-\varepsilon,1+\varepsilon)$$
Quindi, per definizione di limite, $\displaystyle\lim_{x\to0}e^x=1=e^0$, cioè $e^x$ è continua in $0$.

## Caso $x_0\neq0$
$$e^x-e^{x_0}=e^{x_0}\big(e^{x-x_0}-1\big)$$
$$\Rightarrow\ \lim_{x\to x_0}\big(e^x-e^{x_0}\big)=\lim_{x\to x_0}e^{x_0}\big(e^{x-x_0}-1\big)=e^{x_0}\lim_{x\to x_0}\big(e^{x-x_0}-1\big)=e^{x_0}\lim_{t\to0}\big(e^t-1\big)=0$$
(con $t=x-x_0$). Quindi $\displaystyle\lim_{x\to x_0}e^x=e^{x_0}$: $e^x$ è continua in $x_0$, $\forall x_0\in\mathbb{R}$.

## Note collegate
- [[93_Continuita_in_un_Punto]]
- [[104_Cambio_di_Variabile_nei_Limiti]] (la sostituzione $t=x-x_0$)
- [[117_Continuita_delle_Funzioni_Elementari]]
- [[38_Numero_di_Nepero]]
- [[00_MOC_Analisi_1]]

#AM1/continuita/esempio-esponenziale
