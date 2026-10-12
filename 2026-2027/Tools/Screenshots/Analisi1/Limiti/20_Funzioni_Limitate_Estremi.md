---
tags:
  - AM1
  - funzioni
  - funzioni-limitate
  - estremo-superiore
  - estremo-inferiore
  - massimo
  - minimo
data: 2026-09-25
fonte: Lezione 5
---

# Funzioni limitate, estremo superiore, inferiore, massimo e minimo

## Funzioni limitate

> [!info] Definizione — Limitatezza di una funzione
> Data $f:A\subseteq\mathbb{R}\to\mathbb{R}$, diremo che essa:
> - è **limitata superiormente** (dall'alto) se $\operatorname{Im}f\subseteq\mathbb{R}$ è limitato superiormente, cioè $\exists\, M\in\mathbb{R}$ tale che
> $$f(x)\leq M \qquad \forall\, x\in A$$
> - è **limitata inferiormente** (dal basso) se $\operatorname{Im}f\subseteq\mathbb{R}$ è limitato inferiormente, cioè $\exists\, m\in\mathbb{R}$ tale che
> $$f(x)\geq m \qquad \forall\, x\in A$$
> - è **limitata** (sia dall'alto che dal basso) se $\operatorname{Im}f\subseteq\mathbb{R}$ è limitato, cioè $\exists\, m,M\in\mathbb{R}$ tali che
> $$m\leq f(x)\leq M \qquad \forall\, x\in A$$

![[limitazione di un grafico.png]]

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

![[ImmagineDiF.png]]
$$\operatorname{Im}f = (0,1]$$
$$0=\inf_{x\in\mathbb{R}}f, \qquad \nexists\, \min_{x\in\mathbb{R}}f, \qquad \sup_{x\in\mathbb{R}}f = \max_{x\in\mathbb{R}}f = 1 = f(0)$$

### Note collegate
- [[00_MOC_A1]]
- [[19_Funzioni_Generalita]] — $\operatorname{Im}f$, dominio, codominio
- [[07_Insiemi_Limitati_Max_Min]] — insiemi limitati, massimo e minimo
- [[08_Estremo_Superiore_Inferiore]] — $\sup$ e $\inf$ di un insieme
- [[10_Retta_Reale_Intervalli]] — intervalli, $\overline{\mathbb{R}}$