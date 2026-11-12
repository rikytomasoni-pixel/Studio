---
tags:
  - AM1
  - limiti-di-funzioni
  - limiti-notevoli
  - cambio-di-variabile
  - dimostrazione
data: 2026-11-06
lezione: 16
fonte: "AM1 L16 26-27.pdf (pag. 19-20)"
---

# Dimostrazione dei limiti notevoli (logaritmo, esponenziale, potenza)

Dimostrazioni dei limiti notevoli elencati in [[108_Limiti_Notevoli_di_Funzioni]] che si ottengono dal limite di Nepero con il [[104_Cambio_di_Variabile_nei_Limiti|cambio di variabile]].

## Il limite di Nepero
$$\lim_{x\to\pm\infty}\Big(1+\frac1x\Big)^x=e\qquad(*)$$
Per la [[84_Definizione_Successionale_di_Limite|definizione successionale di limite]], questo equivale a
$$\lim_{n\to+\infty}\Big(1+\frac1{c_n}\Big)^{c_n}=e$$
per ogni successione $c_n$ tale che $\displaystyle\lim_{n\to\infty}c_n=\pm\infty$. Questo risultato è stato enunciato (ma non dimostrato) quando abbiamo definito $e$ come
$$e=\lim_{n\to\infty}\Big(1+\frac1n\Big)^n$$
([[38_Numero_di_Nepero]]). Quindi vale $(*)$.

## $\displaystyle\lim_{x\to0}\frac{\log(1+x)}{x}=1$
Poiché $\log t$ è funzione continua, per $(*)$
$$\lim_{t\to\pm\infty}\log\Big(\Big(1+\frac1t\Big)^t\Big)=\log(e)=1\ \Rightarrow\ \lim_{t\to\pm\infty}t\log\Big(1+\frac1t\Big)=1$$
Per cambio di variabile $x=\frac1t$
$$1=\lim_{t\to\pm\infty}t\log\Big(1+\frac1t\Big)=\lim_{x\to0^{\pm}}\frac1x\log(1+x)\ \Rightarrow\ \lim_{x\to0}\frac{\log(1+x)}{x}=1$$

## $\displaystyle\lim_{x\to0}\frac{e^x-1}{x}=1$
Per cambio di variabile
$$e^x-1=t\iff e^x=t+1\iff x=\log(t+1)$$
$$\lim_{x\to0}\frac{e^x-1}{x}=\lim_{t\to0}\frac{t}{\log(t+1)}=\lim_{t\to0}\Big(\frac{\log(t+1)}{t}\Big)^{-1}=1$$

## $\displaystyle\lim_{x\to0}\frac{(1+x)^\alpha-1}{x}=\alpha$, $\alpha\in\mathbb{R}$
Ovvio se $\alpha=0$. Altrimenti $\alpha\neq0$:
$$(1+x)^\alpha-1=e^{\log(1+x)^\alpha}-1=e^{\alpha\log(1+x)}-1$$
$$\lim_{x\to0}\frac{(1+x)^\alpha-1}{x}=\lim_{x\to0}\frac{e^{\alpha\log(1+x)}-1}{x}=\lim_{x\to0}\frac{e^{\alpha\log(1+x)}-1}{\alpha\log(1+x)}\cdot\frac{\alpha\log(1+x)}{x}$$
Posto $t=\alpha\log(1+x)$:
$$=\Big(\lim_{t\to0}\frac{e^t-1}{t}\Big)\cdot\alpha\cdot\Big(\lim_{x\to0}\frac{\log(1+x)}{x}\Big)=1\cdot\alpha\cdot1=\alpha$$

> [!note] Osservazione (non presente negli appunti)
> In L16 non compaiono le dimostrazioni di $\frac{\sin x}{x}\to1$ e $\frac{1-\cos x}{x^2}\to\frac12$: sono state date in L17 ([[119_Dimostrazione_del_Limite_Notevole_sin_x_su_x]], [[120_Dimostrazione_del_Limite_Notevole_1_meno_cos_x_su_x_quadro]]). Restano non dimostrati $\frac{\tan x}{x}\to1$ e $\frac{\arctan x}{x}\to1$.

## Note collegate
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[38_Numero_di_Nepero]]
- [[104_Cambio_di_Variabile_nei_Limiti]]
- [[117_Continuita_delle_Funzioni_Elementari]]
- [[00_MOC_Analisi_1]]
- [[119_Dimostrazione_del_Limite_Notevole_sin_x_su_x]]
- [[120_Dimostrazione_del_Limite_Notevole_1_meno_cos_x_su_x_quadro]]

#AM1/limiti-di-funzioni/dimostrazione-limiti-notevoli
