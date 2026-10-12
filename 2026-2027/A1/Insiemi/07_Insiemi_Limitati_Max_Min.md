---
tags:
  - AM1
  - insiemi-limitati
  - massimo
  - minimo
  - insiemi
data: 2026-09-16
fonte: Lezione 2
---

# Insiemi limitati, massimo e minimo

> [!note] Convenzione
> D'ora in poi $X = \mathbb{R}$ oppure $\mathbb{Q}$. Consideriamo sempre $E\subseteq X$ non vuoto.

## Insiemi limitati

> [!warning] Definizione — Limitatezza
> Dato $E\subseteq X$ non vuoto, $E$ si dice:
> - **limitato dall'alto** (o superiormente) se $\exists\, k\in X$ tale che
> $$x\leq k \qquad \forall\, x\in E$$
> - **limitato dal basso** (o inferiormente) se $\exists\, h\in X$ tale che
> $$h\leq x \qquad \forall\, x\in E$$
> - **limitato** se è limitato sia dall'alto che dal basso, cioè se $\exists\, h,k\in X$ tali che
> $$h\leq x\leq k \qquad \forall\, x\in E$$

## Massimo e minimo

> [!warning] Definizione — Massimo e minimo
> Dato $E\subseteq X$ non vuoto, $x_0\in X$ si dice **massimo** di $E$, e scriviamo $x_0=\max E$, se:
> - $x_0\in E$
> - $x\leq x_0\ \ \forall\, x\in E$
>
> Dato $E\subseteq X$ non vuoto, $x_1\in X$ si dice **minimo** di $E$, e scriviamo $x_1=\min E$, se:
> - $x_1\in E$
> - $x_1\leq x\ \ \forall\, x\in E$

**Osservazione.** Condizione *necessaria* affinché esistano $\max E$ / $\min E$ è che $E$ sia limitato dall'alto/dal basso rispettivamente — ma **non è sufficiente**.

## Esempi

**Esempio.** $E=\mathbb{N}$: limitato dal basso, non limitato dall'alto.
$$\min \mathbb{N} = 0, \qquad \nexists\, \max \mathbb{N}$$

**Esempio.** $E=\left\{\dfrac{1}{n} : n\in\mathbb{N},\ n\neq 0\right\} = \left\{1,\ \dfrac{1}{2},\ \dfrac{1}{3},\ \dfrac{1}{4},\ \dots\right\}$

$E$ è limitato, $\max E = 1$, $\nexists\, \min E$.

**Osservazione.** $\max E$ / $\min E$ non sempre esistono, anche quando $E$ è limitato.

### Note collegate
- [[00_MOC_A1]]
- [[06_Campi_Ordinati]] — $X$ come campo ordinato
- [[08_Estremo_Superiore_Inferiore]] — maggioranti, minoranti, $\sup$ e $\inf$
- [[20_Funzioni_Limitate_Estremi]] — massimo, minimo, $\sup$, $\inf$ di una funzione