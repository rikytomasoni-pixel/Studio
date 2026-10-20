---
tags:
  - AM1
  - serie
  - esempio
  - criterio-del-confronto
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 11-12)"
---

# Esempio: $\displaystyle\sum_{n=2}^\infty\frac{18+\cos n}{n^2\log n}$

Sia $a_n=\dfrac{18+\cos n}{n^2\log n}$. Poiché $\cos n\leq1$ e $\log n$ è crescente in $n$ (quindi $\log n\geq\log2$ per $n\geq2$):
$$0\leq a_n\leq\frac{19}{n^2\log n}\leq\frac{19}{\log2}\cdot\frac1{n^2}$$

Poiché $\displaystyle\sum_{n=1}^\infty\frac1{n^2}$ converge (serie armonica generalizzata di esponente $\alpha=2>1$, vedi [[60_Serie_Armonica_Generalizzata]]), per il [[58_Criterio_del_Confronto_per_Serie]] converge anche $\displaystyle\sum_{n=2}^\infty a_n$.

## Note collegate
- [[58_Criterio_del_Confronto_per_Serie]]
- [[60_Serie_Armonica_Generalizzata]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempi
