---
created: 2026-10-09
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/forme_indeterminate_e_asintotici
aliases: []
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Asintotici Notevoli

Se $\varepsilon_n\to0$ ($\varepsilon_n\neq0$ definitivamente), per $n\to\infty$ valgono:

| Asintotico | Sviluppo con o-piccolo |
|---|---|
| $\sin\varepsilon_n\sim\varepsilon_n$ | $\sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$ |
| $1-\cos\varepsilon_n\sim\dfrac{\varepsilon_n^2}2$ | $\cos\varepsilon_n=1-\dfrac{\varepsilon_n^2}2+o(\varepsilon_n^2)$ |
| $e^{\varepsilon_n}-1\sim\varepsilon_n$ | $e^{\varepsilon_n}=1+\varepsilon_n+o(\varepsilon_n)$ |
| $\log(1+\varepsilon_n)\sim\varepsilon_n$ | $\log(1+\varepsilon_n)=\varepsilon_n+o(\varepsilon_n)$ |
| $(1+\varepsilon_n)^\alpha-1\sim\alpha\varepsilon_n\ \ (\alpha\neq0)$ | $(1+\varepsilon_n)^\alpha=1+\alpha\varepsilon_n+o(\varepsilon_n)$ |
| $\arctan\varepsilon_n\sim\varepsilon_n$ | $\arctan\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$ |

Casi particolari con $\varepsilon_n=\frac1n$:
$$\sin\frac1n\sim\frac1n,\quad e^{1/n}-1\sim\frac1n,\quad\log\left(1+\frac1n\right)\sim\frac1n,\quad1-\cos\frac1n\sim\frac1{2n^2},\quad\left(1+\frac1n\right)^\alpha-1\sim\frac\alpha n,\quad\arctan\frac1n\sim\frac1n.$$
*(Il foglio degli asintotici notevoli è disponibile su WeBeep.)*

> **Figura (disegno senza immagine disponibile):**
>
> Grafico di una successione infinitesima $\varepsilon_n$: punti rossi $\varepsilon_0,\varepsilon_1,\varepsilon_2,\varepsilon_3,\dots,\varepsilon_n$ che oscillano sopra e sotto l'asse orizzontale, con ampiezza decrescente verso $0$ al crescere di $n$; sull'asse sono segnati $0,1,2,3,\dots,n$.

---
Precedente: [[Relazione di Equivalenza Asintotica]] · Successivo: [[Proprietà del Calcolo Asintotico]]
