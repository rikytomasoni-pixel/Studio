---
tags:
  - AM1
  - serie
  - resto
  - teorema
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 2-3)"
---

# Resto N-esimo di una serie

> [!abstract] Teorema
> Data una serie $\displaystyle\sum_{n=1}^\infty a_n$, essa è **convergente / divergente / indeterminata** se e solo se, per ogni $N\in\mathbb{N}$, la serie
> $$R_N=\sum_{n=N+1}^\infty a_n$$
> converge / diverge / è indeterminata.
>
> In particolare, se la serie $\displaystyle\sum_{n=1}^\infty a_n$ converge, allora
> $$\lim_{N\to\infty}R_N=0$$

> [!note] Osservazione
> Se la serie converge a $S\in\mathbb{R}$, allora per ogni $N\in\mathbb{N}$, $N\geq1$,
> $$R_N=\sum_{n=N+1}^\infty a_n=\sum_{n=1}^\infty a_n-\sum_{n=1}^N a_n=S-S_N$$
> (da cui $R_N\to0$, perché $S_N\to S$).

> [!info] Definizione — Resto N-esimo
> $R_N=\displaystyle\sum_{n=N+1}^\infty a_n$ si chiama **resto N-esimo** della serie (convergente) $\displaystyle\sum_{n=1}^\infty a_n$.

## Note collegate
- [[47_Serie_Introduzione_e_Somme_Parziali]] (somme parziali $S_N$)
- [[48_Studio_del_Carattere_di_una_Serie]]
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[00_MOC_Analisi_1]]

#AM1/serie/resto
