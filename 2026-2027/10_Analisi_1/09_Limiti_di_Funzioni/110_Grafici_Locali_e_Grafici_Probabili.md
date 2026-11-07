---
tags:
  - AM1
  - limiti-di-funzioni
  - grafici
  - asintotico
  - esempio
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 18-20)"
---

# Grafici locali / grafici probabili

Le stime tramite gli sviluppi asintotici servono per il calcolo dei limiti, ma anche per tracciare grafici qualitativi (**solo probabili**) di una funzione in un intorno di un certo $x_0\in\overline{\mathbb{R}}$.

Per uno studio più rigoroso e preciso del grafico serve comunque uno studio completo, anche con l'uso di derivate.

> [!warning] Attenzione
> In generale **non è vero** che se $f\sim g$ per $x\to x_0$, $x_0\in\overline{\mathbb{R}}$, allora vicino a $x_0$ i grafici di $f,g$ si assomigliano.

## Esempio: funzioni tutte $\sim x^2$ in $0$
$$g(x)=x^2+x^4,\qquad h(x)=x^2-x^4,\qquad u(x)=x^2,\qquad f(x)=x^2+x^4\sin\frac1{x^3}$$
- $\sin\frac1x\in[-1,1]\ \Rightarrow\ h(x)\le f(x)\le g(x)$ in $\mathbb{R}\setminus\{0\}$
- $g\sim h\sim f\sim x^2$ per $x\to0$

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L15 pag. 19: grafici in $\mathbb{R}^2$ vicino all'origine: $g$ in rosso (parabola più stretta), $u=x^2$ in verde, $h$ in blu (più larga); $f$ in nero oscilla tra $h$ e $g$ sul lato destro avvicinandosi all'origine.

## Esempio: $f(x)=\sqrt[3]{x}+x^2$
- $\mathcal{D}(f)=\mathbb{R}$, $f$ continua
- $\displaystyle\lim_{x\to+\infty}f(x)=+\infty$, $\ f(x)\sim x^2$ per $x\to+\infty$
- $\displaystyle\lim_{x\to-\infty}f(x)=+\infty$, $\ f(x)\sim x^2$ per $x\to-\infty$
- in $x=0$: $f(0)=0$, $\ f(x)\sim\sqrt[3]{x}$ per $x\to0$

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L15 pag. 20: grafico probabile di $f$: a sinistra e a destra sale come una parabola, passa dall'origine con tangente verticale (comportamento da radice cubica), con un piccolo avvallamento a sinistra dell'origine (zeri a sinistra e in $0$).

## Esempio: $f(x)=\sin\sqrt{|x|}$
In un intorno di $x_0=0$ ha grafico come uno dei quattro seguenti; $f(x)\sim\sqrt{|x|}$ per $x\to0$. **L'unico grafico compatibile è il primo.**

> [!warning] DISEGNO NON RAPPRESENTABILE
> AM1 L15 pag. 20: quattro grafici candidati in rosso: (1) cuspide a "V" arrotondata verso l'alto, simmetrica (tipo $\sqrt{|x|}$); (2) retta/curva crescente passante per l'origine; (3) parabola con tratto piatto a destra; (4) curva a "S" con tangente verticale (tipo $\sqrt[3]{x}$).

## Note collegate
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[107_Proprieta_degli_Asintotici_per_Funzioni]]
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[46_Asintotici_Notevoli_e_Limiti_Notevoli]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/grafici-locali
