---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - criterio-della-radice
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 7-8)"
---

# Esempio: la serie $\sum n^a b^n$

> [!example] Esempio
> $$\sum_{n=1}^\infty n^a b^n\qquad a\in\mathbb{R},\ b\geq0$$
> $a_n=n^ab^n\geq0$.

**Risultato** (da dimostrare):
- **converge** se $0\leq b<1$ $\ \forall a\in\mathbb{R}$, oppure se $b=1$ e $a<-1$;
- **diverge** se $b>1$ $\ \forall a\in\mathbb{R}$, oppure se $b=1$ e $a\geq-1$.

## Uso il criterio della radice ([[65_Criterio_della_Radice_per_Serie]])
$$\sqrt[n]{n^ab^n}=b\,n^{a/n}=b\,e^{\log n^{a/n}}=b\,e^{\frac an\log n}\longrightarrow b\,e^0=b$$
perché, per la gerarchia degli infiniti ([[36_Gerarchia_degli_Infiniti]]),
$$\lim_{n\to\infty}\frac an\log n=a\lim_{n\to\infty}\frac{\log n}{n}=0$$

- Se $0\leq b<1$, per il criterio della radice $\sum n^ab^n$ converge ($\forall a\in\mathbb{R}$).
- Se $b>1$, per il criterio della radice $\sum n^ab^n$ diverge ($\forall a\in\mathbb{R}$).
- Se $b=1$ il criterio non dà informazioni; la serie diventa
$$\sum_{n=1}^\infty n^a=\sum_{n=1}^\infty\frac{1}{n^{-a}}$$
che converge se $a<-1$ e diverge se $a\geq-1$ (serie armonica generalizzata $\sum\frac1{n^\alpha}$ con $\alpha=-a$, vedi [[60_Serie_Armonica_Generalizzata]]).

## Note collegate
- [[65_Criterio_della_Radice_per_Serie]]
- [[60_Serie_Armonica_Generalizzata]]
- [[36_Gerarchia_degli_Infiniti]]
- [[66_Esempio_Rapporto_e_Radice_su_Armonica_Generalizzata]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-n-alla-a-per-b-alla-n
