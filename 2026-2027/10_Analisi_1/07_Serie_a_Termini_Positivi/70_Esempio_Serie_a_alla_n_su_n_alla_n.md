---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - criterio-del-rapporto
  - criterio-della-radice
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 6-7)"
---

# Esempio: la serie $\sum \frac{a^n}{n^n}$

> [!example] Esempio
> $$\sum_{n=1}^\infty\frac{a^n}{n^n}\qquad a\geq0$$
> Sia $a_n=\dfrac{a^n}{n^n}$.

**Criterio della radice** ([[65_Criterio_della_Radice_per_Serie]]):
$$\sqrt[n]{a_n}=\frac{a}{n}\to0\in[0,1)$$
$\Rightarrow$ la serie converge per il criterio della radice, $\forall a\geq0$.

**Criterio del rapporto** ([[64_Criterio_del_Rapporto_per_Serie]]). Per $a>0$ (il caso $a=0$ è ovvio…):
$$\frac{a_{n+1}}{a_n}=\frac{a^{n+1}}{(n+1)^{n+1}}\cdot\frac{n^n}{a^n}=a\,\frac{n^n}{(n+1)(n+1)^n}=\frac{a}{n+1}\left(\frac{n}{n+1}\right)^n=\frac{a}{n+1}\left(1-\frac{1}{n+1}\right)^n$$
$$=\frac{a}{n+1}\left(1+\frac{-1}{n+1}\right)^{n+1}\left(1-\frac{1}{n+1}\right)^{-1}\to0\in[0,1)$$
dove, nell'ultimo prodotto, $\frac{a}{n+1}\to0$, $\left(1+\frac{-1}{n+1}\right)^{n+1}\to e^{-1}$ (vedi [[38_Numero_di_Nepero]]) e $\left(1-\frac{1}{n+1}\right)^{-1}\to1$.

$\Rightarrow$ la serie converge per il criterio del rapporto $\forall a\geq0$.

> [!note] Confronto con un caso analogo
> Per la serie $\sum\frac{n!}{n^n}$ si veda [[67_Esempio_Serie_n_Fattoriale_su_n_alla_n]].

## Note collegate
- [[64_Criterio_del_Rapporto_per_Serie]]
- [[65_Criterio_della_Radice_per_Serie]]
- [[69_Dimostrazione_del_Criterio_del_Rapporto_per_Serie]]
- [[38_Numero_di_Nepero]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-a-alla-n-su-n-alla-n
