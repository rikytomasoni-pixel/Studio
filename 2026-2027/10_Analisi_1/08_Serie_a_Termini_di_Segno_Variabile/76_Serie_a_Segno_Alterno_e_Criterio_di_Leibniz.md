---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - serie-alternate
  - leibniz
  - teorema
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 16-17)"
---

# Serie a termini di segno alterno e criterio di Leibniz

> [!abstract] Definizione — serie a termini di segno alterno
> Una serie si dice **a termini di segno alterno** se ha la forma
> $$\sum_{n=0}^\infty(-1)^na_n\qquad\text{con }a_n\geq0\ \text{(definitivamente in }n\in\mathbb{N})$$

> [!abstract] Teorema (criterio di Leibniz)
> Data una serie a termini di segno alterno $\displaystyle\sum_{n=0}^\infty(-1)^na_n$ con
> 1. $a_n\geq0$ (definitivamente);
> 2. $a_{n+1}\leq a_n$ $\ \forall n$ (definitivamente), cioè $a_n$ **decrescente**;
> 3. $\displaystyle\lim_{n\to\infty}a_n=0$;
>
> allora $\displaystyle\sum_{n=0}^\infty(-1)^na_n$ **converge semplicemente**.
>
> Inoltre, se $S=\displaystyle\sum_{n=0}^\infty(-1)^na_n$, allora
> - $S_{2N}=\displaystyle\sum_{n=0}^{2N}(-1)^na_n\searrow S$ (le somme parziali di indice pari **decrescono** definitivamente verso $S$);
> - $S_{2N+1}=\displaystyle\sum_{n=0}^{2N+1}(-1)^na_n\nearrow S$ (le somme parziali di indice dispari **crescono** definitivamente verso $S$);
> - $|R_N|=|S-S_N|\leq a_{N+1}$ $\ \forall N\in\mathbb{N}$ (stima del resto, vedi [[56_Resto_N-esimo_della_Serie]]).

> [!info] Dimostrazione
> Non svolta a lezione ("no dim.").

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** pag. 17, sotto i due punti sulle somme parziali. **Cosa cercare:** una retta orizzontale con il valore $S$ e, a destra, una successione di punti rossi che si avvicinano a $S$ alternandosi: i punti $S_{2N}$ stanno sopra la retta (decrescono verso $S$), i punti $S_{2N+1}$ sotto (crescono verso $S$).

Applicazioni: [[77_Esempio_Serie_Alternata_con_Parametro_alpha]], [[78_Osservazioni_sul_Criterio_di_Leibniz]], [[79_Esempio_Serie_Alternata_log_n_su_n]].

## Note collegate
- [[73_Convergenza_Assoluta_e_Semplice]]
- [[77_Esempio_Serie_Alternata_con_Parametro_alpha]]
- [[78_Osservazioni_sul_Criterio_di_Leibniz]]
- [[79_Esempio_Serie_Alternata_log_n_su_n]]
- [[56_Resto_N-esimo_della_Serie]]
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[00_MOC_Analisi_1]]

#AM1/serie/criterio-di-leibniz
