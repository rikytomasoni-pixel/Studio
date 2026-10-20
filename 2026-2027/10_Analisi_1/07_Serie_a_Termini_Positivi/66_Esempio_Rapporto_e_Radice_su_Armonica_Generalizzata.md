---
tags:
  - AM1
  - serie
  - esempio
  - criterio-del-rapporto
  - criterio-della-radice
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 16-17)"
---

# Esempio: rapporto e radice sulla serie armonica generalizzata ($\ell=1$)

Sia $\displaystyle\sum_{n=1}^\infty\frac1{n^\alpha}$, $\alpha\in\mathbb{R}$, $a_n=\dfrac1{n^\alpha}$. La serie converge se $\alpha>1$, diverge se $\alpha\leq1$ ([[60_Serie_Armonica_Generalizzata]]).

**Criterio del rapporto.**
$$\frac{a_{n+1}}{a_n}=\frac1{(n+1)^\alpha}\cdot n^\alpha=\left(\frac n{n+1}\right)^\alpha\longrightarrow1$$

**Criterio della radice.**
$$\sqrt[n]{a_n}=\left(\frac1{n^\alpha}\right)^{\frac1n}=n^{-\frac\alpha n}=e^{\log n^{-\frac\alpha n}}=e^{-\frac\alpha n\log n}$$
Poiché $\displaystyle\lim_{n\to\infty}-\alpha\cdot\frac{\log n}{n}=0$ per la [[36_Gerarchia_degli_Infiniti]], troviamo
$$\sqrt[n]{a_n}=e^{-\frac\alpha n\log n}\longrightarrow e^0=1$$

> [!danger] Conclusione
> Per ogni $\alpha\in\mathbb{R}$
> $$\lim_{n\to\infty}\sqrt[n]{a_n}=1\qquad\lim_{n\to\infty}\frac{a_{n+1}}{a_n}=1$$
> ma la serie converge per $\alpha>1$ e diverge per $\alpha\leq1$: i criteri del rapporto e della radice **non decidono** quando $\ell=1$.

## Note collegate
- [[64_Criterio_del_Rapporto_per_Serie]]
- [[65_Criterio_della_Radice_per_Serie]]
- [[60_Serie_Armonica_Generalizzata]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempi
