---
tags:
  - AM1
  - serie
  - rappresentazione-decimale
  - serie-geometrica
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 7, 14-15)"
stato: da_verificare
immagini_mancanti: false
---

# Rappresentazione decimale come serie e $0,\overline9=1$

## Numeri reali e serie
Sia $r\in\mathbb{R}$, $\ r=\pm a_0,a_1a_2a_3\dots$ con $a_0\in\mathbb{N}$, $a_k\in\{0,\dots,9\}$ $\forall k\geq1$:
$$r=\pm\left[a_0+\frac{a_1}{10}+\frac{a_2}{10^2}+\frac{a_3}{10^3}+\dots\right]=\pm\sum_{n=0}^\infty\frac{a_n}{10^n}$$

In particolare, per $r\in[0,1]$, $\ r=0,a_1a_2a_3\dots$ ($a_0=0$):
$$r=\sum_{n=1}^\infty\frac{a_n}{10^n}\qquad a_n\in\{0,\dots,9\}\ \ \forall n\geq1$$

## Verifica che $0,\overline9=1$
$$0,\overline9=\sum_{n=1}^\infty\frac9{10^n}=\lim_{N\to\infty}\sum_{n=1}^N\frac9{10^n}=9\lim_{N\to\infty}\sum_{n=1}^N\frac1{10^n}=9\sum_{n=1}^\infty\frac1{10^n}$$
Il sommatorio parte da $n=1$: riconduco alla [[50_Serie_Geometrica]] con ragione $q=\frac1{10}$ (che parte da $n=0$):
$$=9\left[\sum_{n=0}^\infty\frac1{10^n}-1\right]=9\left[\frac1{1-\frac1{10}}-1\right]=9\left(\frac{10}9-1\right)=1$$

Analogamente in base $8$: $\ 0,\overline7=1$.

## Note collegate
- [[50_Serie_Geometrica]]
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[52_Linearita_delle_Serie]]
- [[00_MOC_Analisi_1]]

#AM1/serie/rappresentazione-decimale
