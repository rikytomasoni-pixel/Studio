---
tags:
  - AM1
  - successioni
  - limitatezza
  - convergenza
  - progressione-geometrica
data: 2026-10-02
fonte: Lezione 7
---

# Successione convergente $\Rightarrow$ limitata

> [!abstract] Teorema
> Data una successione $a_n$ convergente, cioè $\exists\, l=\lim_{n\to\infty} a_n \in\mathbb{R}$, allora $a_n$ è limitata.

**Osservazione.** Il viceversa non vale: $a_n$ limitata $\not\Rightarrow$ $\exists\, \lim_{n\to\infty} a_n = l\in\mathbb{R}$.

Ad esempio $a_n=(-1)^n$ è irregolare, ma è limitata.

**Dimostrazione.** Perché $l=\lim_{n\to\infty} a_n\in\mathbb{R}$ esiste, per definizione
$$\forall\, \varepsilon>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad l-\varepsilon<a_n<l+\varepsilon$$

Scegliendo $\varepsilon=1$: $\exists\, N\in\mathbb{N}$ tale che $\forall\, n\geq N$
$$l-1<a_n<l+1$$

Siano
$$M = \max\{a_0,a_1,a_2,\dots,a_N\}, \qquad m = \min\{a_0,a_1,a_2,\dots,a_N\}$$
Essi esistono (massimo e minimo) perché $\{a_0,a_1,\dots,a_N\}$ è un insieme finito e non vuoto di valori.

Siano
$$L = \max\{M, l+1\} \in\mathbb{R}, \qquad P = \min\{m, l-1\} \in\mathbb{R}$$

allora $\forall\, n\in\mathbb{N}$
$$P \leq a_n \leq L$$

![[ConvergenzaQuindiLimitata.png]]

Quindi $a_n$ è limitata. $\blacksquare$

## Esempio — successione geometrica

**Esempio.** Sia $q\in\mathbb{R}$, $a_n = q^n$ (progressione geometrica di ragione $q$).

$$\lim_{n\to\infty} q^n = \begin{cases} +\infty & \text{se } q>1 \quad \text{(crescente)} \\ 1 & \text{se } q=1 \\ 0 & \text{se } 0\leq q<1 \quad \text{(decrescente)} \\ 0 & \text{se } -1<q<0 \quad \text{(non monotona)} \\ \nexists & \text{se } q=-1 \quad \text{(limitata)} \\ \nexists & \text{se } q<-1 \quad \text{(illimitata)} \end{cases}$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[30_Limiti_di_Successioni]] — definizioni di convergenza, divergenza, regolarità
- [[31_Successioni_Monotone]]
- [[29_Successioni_Definizioni_Base]] — limitatezza
- [[11_Radici_e_Potenze]] — potenze

#AM1/successioni-e-limiti/successione-convergente-e-limitata
