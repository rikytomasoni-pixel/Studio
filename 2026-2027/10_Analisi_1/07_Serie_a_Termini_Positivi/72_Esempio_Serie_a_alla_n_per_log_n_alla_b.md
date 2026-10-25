---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - criterio-del-rapporto
  - condizione-necessaria
  - esempio
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 9-10)"
---

# Esempio: la serie $\sum a^n(\log n)^b$

> [!example] Esempio
> $$\sum_{n=2}^\infty a^n(\log n)^b\qquad a>0,\ b\in\mathbb{R}$$
> $a_n=a^n(\log n)^b>0$.

**Risultato** (da dimostrare):
- **converge** se $a\in(0,1)$ $\ \forall b\in\mathbb{R}$;
- **diverge** se $a\in[1,\infty)$ $\ \forall b\in\mathbb{R}$.

## Criterio del rapporto ([[64_Criterio_del_Rapporto_per_Serie]]), $\forall b\in\mathbb{R}$
$$\frac{a_{n+1}}{a_n}=\frac{a^{n+1}(\log(n+1))^b}{a^n(\log n)^b}=a\left(\frac{\log(n+1)}{\log n}\right)^b\longrightarrow a$$
- Se $a\in(0,1)$ la serie converge ($\forall b\in\mathbb{R}$).
- Se $a>1$ la serie diverge ($\forall b\in\mathbb{R}$).

## Caso $a=1$
La serie diventa $\displaystyle\sum_{n=2}^\infty(\log n)^b$. **Diverge $\forall b\in\mathbb{R}$**: infatti è a termini positivi e

$$\lim_{n\to\infty}(\log n)^b=\begin{cases}+\infty & b>0\\ 1 & b=0\end{cases}$$

- Per $b\geq0$ non è soddisfatta la condizione necessaria $\lim(\log n)^b=0$ ([[54_Condizione_Necessaria_di_Convergenza]]), quindi la serie a termini positivi $\sum(\log n)^b$ diverge.
- Per $b<0$ vale definitivamente
$$(\log n)^b=\frac{1}{(\log n)^{|b|}}>\frac1n$$
per la gerarchia degli infiniti ([[36_Gerarchia_degli_Infiniti]]). Poiché $\sum\frac1n$ diverge (serie armonica, [[55_Serie_Armonica]]), per il criterio del confronto per serie ([[58_Criterio_del_Confronto_per_Serie]]) diverge anche $\sum(\log n)^b$.

## Note collegate
- [[64_Criterio_del_Rapporto_per_Serie]]
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[55_Serie_Armonica]]
- [[58_Criterio_del_Confronto_per_Serie]]
- [[36_Gerarchia_degli_Infiniti]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempio-a-alla-n-per-log-n-alla-b
