---
tags:
  - AM1
  - serie
  - serie-armonica
  - divergenza
  - dimostrazione
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 19-21)"
stato: da_verificare
immagini_mancanti: true
---

# Serie armonica

$$\sum_{n=1}^\infty\frac1n$$
Vale $\lim_{n\to\infty}\frac1n=0$ e
$$\sum_{n=1}^\infty\frac1n=+\infty$$
È il controesempio all'inversione della [[54_Condizione_Necessaria_di_Convergenza]].

## Dimostrazione

**Passo 1.** Osserviamo che
$$\frac1n\geq\log\left(1+\frac1n\right)\qquad\forall n\geq1$$
Infatti, per il [[38_Numero_di_Nepero]],
$$e=\lim_{n\to\infty}\left(1+\frac1n\right)^n=\sup_{n\geq1}\left(1+\frac1n\right)^n\ \Rightarrow\ \left(1+\frac1n\right)^n\leq e$$
$$\Rightarrow\log\left(1+\frac1n\right)^n\leq\log e=1\ \Rightarrow\ n\log\left(1+\frac1n\right)\leq1\ \Rightarrow\ \log\left(1+\frac1n\right)\leq\frac1n$$

![[graficoLogeDerivata.png]]

**Passo 2.** Allora
$$S_N=\sum_{n=1}^N\frac1n\geq\sum_{n=1}^N\log\left(1+\frac1n\right)=\sum_{n=1}^N\log\left(\frac{n+1}n\right)=\sum_{n=1}^N\left(\log(n+1)-\log n\right)$$
$$=(\cancel{\log2}-\log1)+(\cancel{\log3}-\cancel{\log2})+\dots+(\log(N+1)-\cancel{\log N})=\log(N+1)-\log1=\log(N+1)$$
(somma telescopica, vedi [[53_Serie_Telescopiche_e_Mengoli]]).

$$\Rightarrow S_N\geq\log(N+1)\qquad\forall N\geq1$$

**Passo 3.** Poiché $\lim_{N\to\infty}\log(N+1)=+\infty$, per il teorema del confronto per successioni divergenti ([[35_Teoremi_del_Confronto]]) vale
$$\lim_{N\to\infty}S_N=+\infty\ \Rightarrow\ \sum_{n=1}^\infty\frac1n=\lim_{N\to\infty}S_N=+\infty$$
e la serie **diverge** (anche se $\lim_{n\to\infty}\frac1n=0$). $\square$

## Note collegate
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[53_Serie_Telescopiche_e_Mengoli]]
- [[38_Numero_di_Nepero]]
- [[35_Teoremi_del_Confronto]]
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[00_MOC_Analisi_1]]

#AM1/serie/serie-armonica
