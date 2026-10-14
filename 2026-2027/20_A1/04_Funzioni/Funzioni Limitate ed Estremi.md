---
created: 2026-09-25
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Funzioni Limitate ed Estremi

**Definizione.** Data $f:A\subseteq\mathbb{R}\to\mathbb{R}$, diciamo che $f$ è:

- **limitata superiormente** (dall'alto) se $\operatorname{Im}f\subseteq\mathbb{R}$ è limitato superiormente, cioè $\exists M\in\mathbb{R}$ tale che $f(x)\le M\ \ \forall x\in A$;
- **limitata inferiormente** (dal basso) se $\operatorname{Im}f$ è limitato inferiormente, cioè $\exists m\in\mathbb{R}$ tale che $f(x)\ge m\ \ \forall x\in A$;
- **limitata** se $\operatorname{Im}f$ è limitato, cioè $\exists m,M\in\mathbb{R}$ tali che $m\le f(x)\le M\ \ \forall x\in A$.

![[funzione-limitata-grafico.png]]



## 2. Estremi e massimo/minimo di una funzione

Data $f:A\subseteq\mathbb{R}\to\mathbb{R}$ (cfr. [[2026-09-16 A1 Lezione 2|estremo superiore]]) si definiscono:

- $\displaystyle\sup_{x\in A}f(x)=\sup\operatorname{Im}f$ (**estremo superiore**)
- $\displaystyle\inf_{x\in A}f(x)=\inf\operatorname{Im}f$ (**estremo inferiore**)
- $\displaystyle\max_{x\in A}f(x)=\max\operatorname{Im}f$ (**massimo**, se esiste)
- $\displaystyle\min_{x\in A}f(x)=\min\operatorname{Im}f$ (**minimo**, se esiste)

**Osservazioni.**
- Sono massimo e minimo **assoluti**.
- $\sup f$ e $\inf f$ esistono **sempre** in $\overline{\mathbb{R}}=\mathbb{R}\cup\{\pm\infty\}$.
- Se esistono massimo o minimo, allora $\max f=\sup f$ e $\min f=\inf f$.

**Esempio.** $f:\mathbb{R}\to\mathbb{R}$, $f(x)=\dfrac1{1+x^2}$: $\operatorname{Im}f=(0,1]$. Allora $\inf f=0$ ma non esiste $\min f$; $\sup f=\max f=1=f(0)$.

![[grafico-1-su-1-piu-x-quadro.png]]

---
Precedente: [[Generalità sulle Funzioni]] · Successivo: [[Campo di Esistenza]]
