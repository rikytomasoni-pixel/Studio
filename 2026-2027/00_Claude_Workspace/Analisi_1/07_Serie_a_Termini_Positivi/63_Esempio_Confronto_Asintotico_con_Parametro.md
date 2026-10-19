---
tags:
  - AM1
  - serie
  - esempio
  - confronto-asintotico
  - parametro
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 12-13)"
stato: da_verificare
destinazione: 10_Analisi_1/07_Serie_a_Termini_Positivi (cartella nuova)
---

# Esempio: serie con parametro $\alpha$ e confronto asintotico

Studiare il carattere, al variare di $\alpha\in\mathbb{R}$, di
$$\sum_{k=1}^\infty\frac{5k^2-1}{k^\alpha+k}\arctan\frac1k$$

Sia $a_k=\dfrac{5k^2-1}{k^\alpha+k}\arctan\dfrac1k\geq0$ per ogni $k\geq1$ (serie a termini positivi). Usando $\arctan\frac1k\sim\frac1k$ ([[46_Asintotici_Notevoli_e_Limiti_Notevoli]]):
$$a_k\sim\begin{cases}\dfrac{5k^2}{k^\alpha}\cdot\dfrac1k&\alpha>1\\[3mm]\dfrac{5k^2}{2k}\cdot\dfrac1k&\alpha=1\\[3mm]\dfrac{5k^2}{k}\cdot\dfrac1k&\alpha<1\end{cases}\;=\;\begin{cases}\dfrac5{k^{\alpha-1}}&\alpha>1\\[3mm]\dfrac52&\alpha=1\\[3mm]5&\alpha<1\end{cases}$$

**Caso $\alpha\leq1$.**
$$\lim_{n\to\infty}a_n=\begin{cases}5/2&\alpha=1\\5&\alpha<1\end{cases}$$
Non è soddisfatta la [[54_Condizione_Necessaria_di_Convergenza]] $\lim a_n=0$, quindi $\sum a_n$ non converge. Essendo a termini positivi, $\sum a_n$ **diverge a $+\infty$**.

**Caso $\alpha>1$.** $a_n\sim\dfrac5{n^{\alpha-1}}$ e $\displaystyle\sum_{n=1}^\infty\frac1{n^{\alpha-1}}$ è una [[60_Serie_Armonica_Generalizzata]] di esponente $\alpha-1$: converge se $\alpha-1>1$ (cioè $\alpha>2$), diverge se $\alpha-1\leq1$ (cioè $\alpha\leq2$).

Per il [[62_Criterio_del_Confronto_Asintotico_per_Serie]]:

> [!success] Risultato
> la serie $\sum a_n$ **converge se $\alpha>2$**, **diverge se $1<\alpha\leq2$** (e diverge anche per $\alpha\leq1$, vedi sopra).

## Note collegate
- [[62_Criterio_del_Confronto_Asintotico_per_Serie]]
- [[60_Serie_Armonica_Generalizzata]]
- [[44_Esempio_Asintotici_con_Logaritmo_e_Arctan]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempi
