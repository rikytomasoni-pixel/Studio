---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - leibniz
  - derivate
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 22-24)"
---

# Esempio: la serie $\sum(-1)^n\frac{\log n}{n}$

> [!example] Esempio
> $$\sum_{n=1}^\infty(-1)^n\frac{\log n}{n}=\sum_{n=1}^\infty(-1)^na_n,\qquad a_n=\frac{\log n}{n}$$

- $a_n=\dfrac{\log n}{n}\geq0$ $\ \forall n\geq1$;
- $\displaystyle\lim_{n\to\infty}a_n=\lim_{n\to\infty}\frac{\log n}{n}=0$;
- **non converge assolutamente**: $\displaystyle\sum_{n=1}^\infty|(-1)^na_n|=\sum_{n=1}^\infty\frac{\log n}{n}=+\infty$ per confronto con la serie armonica: $\dfrac{\log n}{n}\geq\dfrac1n$ definitivamente e $\sum\frac1n$ diverge ([[55_Serie_Armonica]], [[58_Criterio_del_Confronto_per_Serie]]).

> [!tip] Oppure
> Con la serie di Bertrand ([[61_Serie_di_Bertrand_Generalizzata]])
> $$\sum_{n=2}^\infty\frac{1}{n^\alpha(\log n)^\beta}$$
> che diverge per $\alpha<1$, $\forall\beta\in\mathbb{R}$, e per $\alpha=1$, $\beta\leq1$: qui siamo nel caso $\alpha=1$, $\beta=-1$.

## Uso il criterio di Leibniz
Vogliamo $a_{n+1}\leq a_n$ definitivamente, cioè
$$\frac{\log(n+1)}{n+1}\leq\frac{\log n}{n}$$
**complicato…** Avendo a disposizione le derivate e il test di monotonia per funzioni derivabili su un intervallo sarà tutto più semplice.

Sia $f(x)=\dfrac{\log x}{x}$: è una funzione derivabile, che interpola i valori della successione $a_n$ (cioè $f(n)=a_n$ $\forall n\geq1$) e che è definitivamente decrescente. Infatti
$$f'(x)=\frac{1-\log x}{x^2}\quad\forall x>0\ \Rightarrow\ f'(x)\leq0\ \ \forall x\geq e\ \Rightarrow\ f\text{ decresce in }[e,\infty)\ \Rightarrow\ a_n=f(n)\text{ decresce }\forall n\geq3>e$$

Pertanto, per Leibniz ([[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]), $\displaystyle\sum_{n=1}^\infty(-1)^n\frac{\log n}{n}$ **converge semplicemente** (ma non assolutamente).

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** pag. 24, in alto. **Cosa cercare:** grafico di $f(x)=\frac{\log x}{x}$ in rosso (sale fino a un massimo vicino a $x=e$ e poi decresce verso $0$), con le ascisse $1,2,e,3,4,5$ segnate sull'asse e i punti $a_2,a_3,a_4,a_5$ evidenziati sul grafico.

> [!note] Osservazione
> $a_n=\dfrac{\log n}{n}\not\sim\dfrac1n$, anche se $\displaystyle\lim_{n\to\infty}a_n=\lim_{n\to\infty}\frac{\log n}{n}=0=\lim_{n\to\infty}\frac1n$: il limite $\frac{\log n}{n}\to0$ vale per la gerarchia degli infiniti ([[36_Gerarchia_degli_Infiniti]]), non per $\sim$.

## Note collegate
- [[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]
- [[61_Serie_di_Bertrand_Generalizzata]]
- [[55_Serie_Armonica]]
- [[36_Gerarchia_degli_Infiniti]]
- [[78_Osservazioni_sul_Criterio_di_Leibniz]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-serie-alternata-log-n-su-n
