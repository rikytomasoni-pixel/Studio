---
tags:
  - AM1
  - limiti-di-funzioni
  - limiti-notevoli
  - dimostrazione
  - trigonometria
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 2-3); Dimostrazioni primi limiti notevoli.pdf (pag. 1)"
---

# Dimostrazione di $\displaystyle\lim_{x\to0}\frac{\sin x}{x}=1$

Dimostrazione del primo limite notevole elencato in [[108_Limiti_Notevoli_di_Funzioni]] (viste a esercitazioni e riprese a lezione). Sono riportate due versioni: quella a lezione (confronto tra lunghezze) e quella dei fogli di esercitazione (confronto tra aree).

## Versione di lezione (confronto tra lunghezze)

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 2**: circonferenza goniometrica di centro $O$ e raggio $1$ con l'angolo $x$ (in rosso) tra l'asse $x$ e il raggio $OP$. Sono indicati: $P$ sulla circonferenza, $H$ proiezione di $P$ sull'asse $x$, $K$ proiezione di $P$ sull'asse $y$, $A=(1,0)$, $T$ punto della retta $OP$ sulla tangente verticale in $A$.

Dalla figura: $\overline{OP}=1$, $\overline{PH}=\sin x$, $\overline{TA}=\tan x$, $\widehat{PA}=x$ (lunghezza dell'arco). Quindi
$$0\le\sin x\le x\le\tan x\qquad x\in\Big[0,\frac\pi2\Big)$$
dove $\textcircled{1}$ è $\sin x\le x$ e $\textcircled{2}$ è $x\le\tan x$. Dividendo per $\sin x>0$ (usando $\textcircled{2}$ con $\tan x=\frac{\sin x}{\cos x}$ e $\textcircled{1}$):
$$\cos x\ \overset{\textcircled{2}}{\le}\ \frac{\sin x}{x}\ \overset{\textcircled{1}}{\le}\ 1\qquad x\in\Big(0,\frac\pi2\Big)$$
Per simmetria ($\frac{\sin x}{x}$ è pari)
$$\cos x\le\frac{\sin x}{x}\le1\qquad x\in\Big(-\frac\pi2,\frac\pi2\Big)\setminus\{0\}$$
Per confronto (teorema dei due carabinieri, [[100_Teorema_del_Confronto_per_Limiti_di_Funzioni]]), essendo $\cos x\to1$ per $x\to0$:
$$\lim_{x\to0}\frac{\sin x}{x}=1\qquad\square$$

## Versione delle esercitazioni (confronto tra aree)

**1) Parità.** $f(x)=\dfrac{\sin x}{x}$ è pari:
$$f(-x)=\frac{\sin(-x)}{-x}=\frac{-\sin x}{-x}=\frac{\sin x}{x}=f(x)$$
quindi $\displaystyle\lim_{x\to0^+}f(x)=\lim_{x\to0^-}f(x)$ ed è sufficiente studiare il limite destro.

**2) Confronto tra aree.**

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dimostrazioni primi limiti notevoli.pdf, pag. 1 (punto 2)**: circonferenza unitaria di centro $O$ con angolo $x$; $A$ punto sulla circonferenza (segmento $OA$ rosso), $B=(1,0)$ sull'asse $x$, $C$ sulla tangente verticale in $B$ (segmento verde $BC$), arco $AB$ in blu. Servono per il confronto tra triangolo $OAB$, settore circolare $OAB$ e triangolo $OBC$.

$$A(\text{triangolo }OAB)<A(\text{settore }OAB)<A(\text{triangolo }OBC)$$
$$\tfrac12\,\overline{OA}\cdot\overline{OB}\cdot\sin x<\tfrac12\,\overline{OA}^{\,2}\cdot x<\tfrac12\,\overline{OB}\tan x\cdot\overline{OA}$$
Con $\overline{OA}=\overline{OB}=1$:
$$\sin x<x<\tan x\ \Rightarrow\ \sin x<x<\frac{\sin x}{\cos x}\ \Rightarrow\ 1<\frac{x}{\sin x}<\frac1{\cos x}\ \Rightarrow\ \cos x<\frac{\sin x}{x}<1$$
Passando al limite per $x\to0^+$ e per il teorema del confronto
$$\lim_{x\to0}\frac{\sin x}{x}=1$$

## Conseguenza
$\sin x\sim x$ e $\sin x=x+o(x)$ per $x\to0$ ([[106_Asintotico_e_o_piccolo_per_Funzioni]]).

## Note collegate
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[120_Dimostrazione_del_Limite_Notevole_1_meno_cos_x_su_x_quadro]] (usa questo limite)
- [[118_Dimostrazione_dei_Limiti_Notevoli]]
- [[100_Teorema_del_Confronto_per_Limiti_di_Funzioni]]
- [[117_Continuita_delle_Funzioni_Elementari]]
- [[128_Derivate_delle_Funzioni_Elementari]] (derivata del seno)
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/dimostrazione-sin-x-su-x
