---
created: 2026-09-25
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
origine: UpdateVault
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Funzioni Limitate ed Estremi

## Funzioni limitate

> [!info] Definizione — Limitatezza di una funzione
> Data $f:A\subseteq\mathbb{R}\to\mathbb{R}$, diremo che essa:
> - è **limitata superiormente** (dall'alto) se $\operatorname{Im}f\subseteq\mathbb{R}$ è limitato superiormente, cioè $\exists\, M\in\mathbb{R}$ tale che
> $$f(x)\leq M \qquad \forall\, x\in A$$
> - è **limitata inferiormente** (dal basso) se $\operatorname{Im}f\subseteq\mathbb{R}$ è limitato inferiormente, cioè $\exists\, m\in\mathbb{R}$ tale che
> $$f(x)\geq m \qquad \forall\, x\in A$$
> - è **limitata** (sia dall'alto che dal basso) se $\operatorname{Im}f\subseteq\mathbb{R}$ è limitato, cioè $\exists\, m,M\in\mathbb{R}$ tali che
> $$m\leq f(x)\leq M \qquad \forall\, x\in A$$

![[funzione-limitata-grafico.png]]

## Estremo superiore, inferiore, massimo, minimo di una funzione

> [!info] Definizione
> Data $f:A\subseteq\mathbb{R}\to\mathbb{R}$ definiamo:
> - $\displaystyle\sup_{x\in A} f(x) = \sup \operatorname{Im}f$ — **estremo superiore**
> - $\displaystyle\inf_{x\in A} f(x) = \inf \operatorname{Im}f$ — **estremo inferiore**
> - $\displaystyle\max_{x\in A} f(x) = \max \operatorname{Im}f$ — **massimo** (se esiste)
> - $\displaystyle\min_{x\in A} f(x) = \min \operatorname{Im}f$ — **minimo** (se esiste)

**Osservazioni.**
- Massimo e minimo sono **assoluti**.
- $\displaystyle\sup_{x\in A}f$, $\displaystyle\inf_{x\in A}f$ esistono sempre in $\mathbb{R}\cup\{\pm\infty\}=\overline{\mathbb{R}}$.
- Se esistono massimo o minimo, $\displaystyle\max_{x\in A}f = \sup_{x\in A}f$ e $\displaystyle\min_{x\in A}f = \inf_{x\in A}f$.

**Esempio.** $f(x) = \dfrac{1}{1+x^2}$, $f:\mathbb{R}\to\mathbb{R}$

![[grafico-1-su-1-piu-x-quadro.png]]
$$\operatorname{Im}f = (0,1]$$
$$0=\inf_{x\in\mathbb{R}}f, \qquad \nexists\, \min_{x\in\mathbb{R}}f, \qquad \sup_{x\in\mathbb{R}}f = \max_{x\in\mathbb{R}}f = 1 = f(0)$$

---
Precedente: [[Generalità sulle Funzioni]] · Successivo: [[Campo di Esistenza]]
