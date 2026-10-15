---
tags:
  - AM1
  - serie
  - serie-geometrica
  - somme-parziali
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 13-14)"
stato: da_verificare
immagini_mancanti: true
---

# Serie geometrica

**Serie geometrica di ragione $q\in\mathbb{R}$:** $a_n=q^n$, $n\in\mathbb{N}$,
$$\sum_{n=0}^\infty q^n$$

## Somme parziali
$$S_N=\sum_{n=0}^Nq^n=1+q+q^2+q^3+\dots+q^{N-1}+q^N$$
Osserviamo che
$$qS_N=\sum_{n=0}^Nq^{n+1}=q+q^2+q^3+q^4+\dots+q^N+q^{N+1}$$
$$\Rightarrow S_N-qS_N=1-q^{N+1}\ \Rightarrow\ (1-q)S_N=1-q^{N+1}\qquad\forall q\in\mathbb{R},\ \forall N\in\mathbb{N}$$

$$\sum_{n=0}^Nq^n=S_N=\begin{cases}\dfrac{1-q^{N+1}}{1-q}&q\neq1\\[2mm]N+1&q=1\end{cases}$$

## Carattere e somma
$$\sum_{n=0}^\infty q^n=\lim_{N\to\infty}S_N=\begin{cases}+\infty&q\geq1\\[1mm]\dfrac1{1-q}&|q|<1\\[2mm]\nexists&q\leq-1\end{cases}$$
*(annotazione in rosso: vedere il limite della successione geometrica $q^n$)*

## Esempio: $q=\frac12$
$$\sum_{n=0}^\infty\frac1{2^n}=1+\frac12+\frac14+\frac18+\frac1{16}+\dots+\frac1{2^n}+\dots=\frac1{1-\frac12}=2$$

Vedi [[47_Serie_Introduzione_e_Somme_Parziali]].

## Note collegate
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[49_Esempi_Elementari_di_Serie]]
- [[51_Rappresentazione_Decimale_e_Serie]]
- [[52_Linearita_delle_Serie]]
- [[00_MOC_Analisi_1]]

#AM1/serie/serie-geometrica
