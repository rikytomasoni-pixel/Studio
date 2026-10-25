---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - convergenza-assoluta
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 15-16)"
---

# Esempio: convergenza assoluta di $\sum\frac{\sin n}{n^{3/2}}$ e $\sum\frac{(-1)^n}{n^{3/2}}$

> [!example] Esempio
> $$\sum_{n=1}^\infty\frac{\sin n}{n^{3/2}}\qquad\text{e}\qquad\sum_{n=1}^\infty\frac{(-1)^n}{n^{3/2}}$$
> Poniamo $a_n=\dfrac{\sin n}{n^{3/2}}$ nel primo caso, $a_n=\dfrac{(-1)^n}{n^{3/2}}$ nel secondo.

In entrambi i casi
$$0\leq|a_n|\leq\frac{1}{n^{3/2}}\qquad\forall n\geq1$$
Poiché $\displaystyle\sum_{n=1}^\infty\frac{1}{n^{3/2}}$ converge (serie armonica generalizzata con esponente $\alpha=\frac32>1$, [[60_Serie_Armonica_Generalizzata]]), per il confronto per serie ([[58_Criterio_del_Confronto_per_Serie]]) converge anche $\sum_{n=1}^\infty|a_n|$, cioè $\sum a_n$ **converge assolutamente**.

Quindi, per convergenza assoluta ([[74_Criterio_di_Convergenza_Assoluta]]), $\sum a_n$ converge anche semplicemente.

## Note collegate
- [[74_Criterio_di_Convergenza_Assoluta]]
- [[73_Convergenza_Assoluta_e_Semplice]]
- [[60_Serie_Armonica_Generalizzata]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-convergenza-assoluta
