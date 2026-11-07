---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - convergenza-assoluta
  - teorema
  - dimostrazione
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 12-15)"
---

# Criterio di convergenza assoluta

> [!abstract] Teorema (criterio di convergenza assoluta)
> Se la serie $\displaystyle\sum_{n=0}^\infty a_n$ converge assolutamente, allora essa converge anche semplicemente. Inoltre, in tal caso,
> $$\left|\sum_{n=0}^\infty a_n\right|\leq\sum_{n=0}^\infty|a_n|$$

Definizioni in [[73_Convergenza_Assoluta_e_Semplice]]. Il viceversa è falso.

## Dimostrazione
Osserviamo che $\forall n\in\mathbb{N}$
$$0\leq a_n+|a_n|\leq2|a_n|$$
Per ipotesi $\sum_{n=0}^\infty|a_n|$ è convergente, quindi anche $\sum_{n=0}^\infty2|a_n|$ lo è. Per il criterio del confronto per serie (a termini non negativi, [[58_Criterio_del_Confronto_per_Serie]]) converge anche
$$\sum_{n=0}^\infty(a_n+|a_n|)\in\mathbb{R}$$
Inoltre
$$\sum_{n=0}^\infty a_n=\sum_{n=0}^\infty\big(a_n+|a_n|-|a_n|\big)=\underbrace{\sum_{n=0}^\infty(a_n+|a_n|)}_{\in\mathbb{R}}-\underbrace{\sum_{n=0}^\infty|a_n|}_{\in\mathbb{R}}\in\mathbb{R}$$
essendo le due serie a ultimo membro convergenti (linearità, [[52_Linearita_delle_Serie]]). $\Rightarrow$ converge anche $\sum_{n=0}^\infty a_n$.

Sotto queste ipotesi, dalla disuguaglianza triangolare segue che
$$\left|\sum_{n=0}^Na_n\right|\leq\sum_{n=0}^N|a_n|\qquad\forall N\in\mathbb{N}$$
e passando al limite (per permanenza del segno, [[33_Teorema_Permanenza_del_Segno]])
$$\left|\sum_{n=0}^\infty a_n\right|\leq\sum_{n=0}^\infty|a_n|$$
perché entrambe le serie convergono. $\blacksquare$

## Esempio
Vedi [[75_Esempio_Convergenza_Assoluta_sin_n_su_n_alla_3_su_2]].

## Note collegate
- [[73_Convergenza_Assoluta_e_Semplice]]
- [[75_Esempio_Convergenza_Assoluta_sin_n_su_n_alla_3_su_2]]
- [[58_Criterio_del_Confronto_per_Serie]]
- [[52_Linearita_delle_Serie]]
- [[33_Teorema_Permanenza_del_Segno]]
- [[00_MOC_Analisi_1]]

#AM1/serie/criterio-di-convergenza-assoluta
