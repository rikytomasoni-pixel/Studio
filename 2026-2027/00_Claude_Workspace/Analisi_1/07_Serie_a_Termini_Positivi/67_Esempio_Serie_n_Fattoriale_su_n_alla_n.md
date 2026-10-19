---
tags:
  - AM1
  - serie
  - esempio
  - criterio-del-rapporto
  - confronto-asintotico
  - stirling
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 18-19)"
stato: da_verificare
destinazione: 10_Analisi_1/07_Serie_a_Termini_Positivi (cartella nuova)
---

# Esempio: $\displaystyle\sum_{n=1}^\infty\frac{n!}{n^n}$

Sia $a_n=\dfrac{n!}{n^n}>0$.

## Metodo 1: criterio del rapporto
$$\frac{a_{n+1}}{a_n}=\frac{(n+1)!}{(n+1)^{n+1}}\cdot\frac{n^n}{n!}=\frac{\cancel{(n+1)}\,\cancel{n!}\,n^n}{(n+1)^n\,\cancel{(n+1)}\,\cancel{n!}}=\left(\frac n{n+1}\right)^n=\left(1-\frac1{n+1}\right)^{n+1}\left(1-\frac1{n+1}\right)^{-1}$$
$$\longrightarrow e^{-1}\cdot1=e^{-1}\in[0,1)$$
Per il [[64_Criterio_del_Rapporto_per_Serie]] la serie **converge**.

## Metodo 2: confronto asintotico con la formula di Stirling
Per la [[68_Formula_di_Stirling]]
$$n!\sim\sqrt{2\pi n}\left(\frac ne\right)^n$$
$$\Rightarrow a_n=\frac{n!}{n^n}\sim\sqrt{2\pi n}\left(\frac{\cancel n}{e}\right)^{\!n}\cdot\frac1{\cancel{n^n}}=\sqrt{2\pi n}\cdot\frac1{e^n}$$
Notiamo che, essendo $\displaystyle\lim_{n\to\infty}\frac{\sqrt{2\pi n}}{2^n}=0$, vale
$$0\leq\frac{\sqrt{2\pi n}}{e^n}=\frac{\sqrt{2\pi n}}{2^n}\left(\frac2e\right)^n\leq1\cdot\left(\frac2e\right)^n$$
definitivamente in $n\in\mathbb{N}$. Poiché $\displaystyle\sum_{n=1}^\infty\left(\frac2e\right)^n$ converge (serie geometrica di ragione $q=\frac2e\in[0,1)$, [[50_Serie_Geometrica]]), per il [[58_Criterio_del_Confronto_per_Serie]] converge anche $\displaystyle\sum_{n=1}^\infty\frac{\sqrt{2\pi n}}{e^n}$.

Per il [[62_Criterio_del_Confronto_Asintotico_per_Serie]] converge anche $\displaystyle\sum_{n=1}^\infty\frac{n!}{n^n}$, essendo $\dfrac{n!}{n^n}\sim\dfrac{\sqrt{2\pi n}}{e^n}$.

## Note collegate
- [[64_Criterio_del_Rapporto_per_Serie]]
- [[62_Criterio_del_Confronto_Asintotico_per_Serie]]
- [[68_Formula_di_Stirling]]
- [[38_Numero_di_Nepero]]
- [[39_Criterio_del_Rapporto]] (vedi anche $n^n/n!\to+\infty$)
- [[00_MOC_Analisi_1]]

#AM1/serie/esempi
