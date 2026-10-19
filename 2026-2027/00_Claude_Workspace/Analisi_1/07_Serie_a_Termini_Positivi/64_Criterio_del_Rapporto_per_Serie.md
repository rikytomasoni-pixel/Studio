---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - criterio-del-rapporto
  - teorema
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 14-15)"
stato: da_verificare
destinazione: 10_Analisi_1/07_Serie_a_Termini_Positivi (cartella nuova)
---

# Criterio del rapporto per serie

> [!abstract] Teorema — Criterio del rapporto
> Sia $a_n$ una successione a termini (definitivamente) positivi ed esista
> $$\ell=\lim_{n\to\infty}\frac{a_{n+1}}{a_n}\in\overline{\mathbb{R}}$$
> Allora:
> 1. se $\ell>1$ (incluso $+\infty$), allora $\displaystyle\sum_{n=1}^\infty a_n$ **diverge** e $\displaystyle\lim_{n\to\infty}a_n=+\infty$;
> 2. se $0\leq\ell<1$, allora $\displaystyle\sum_{n=1}^\infty a_n$ **converge** e $\displaystyle\lim_{n\to\infty}a_n=0$.

> [!warning] Caso $\ell=1$
> Se $\ell=1$ **non si può concludere nulla**: esistono serie $\sum a_n$ convergenti per le quali $\lim\frac{a_{n+1}}{a_n}=1$ ed esistono serie divergenti per le quali $\lim\frac{a_{n+1}}{a_n}=1$ (vedi [[66_Esempio_Rapporto_e_Radice_su_Armonica_Generalizzata]]).

> [!note] Conseguenza per le successioni
> - se $0\leq\ell<1$: $\lim_{n\to\infty}a_n=0$
> - se $\ell>1$: $\lim_{n\to\infty}a_n=+\infty$
>
> Questo è il **criterio del rapporto per successioni**, già enunciato in [[39_Criterio_del_Rapporto]].

> [!info] Dimostrazione
> Nel quaderno di questa lezione non è riportata la dimostrazione.

## Esempi
- [[66_Esempio_Rapporto_e_Radice_su_Armonica_Generalizzata]]
- [[67_Esempio_Serie_n_Fattoriale_su_n_alla_n]]

## Note collegate
- [[65_Criterio_della_Radice_per_Serie]]
- [[39_Criterio_del_Rapporto]]
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[00_MOC_Analisi_1]]

#AM1/serie/criterio-del-rapporto
