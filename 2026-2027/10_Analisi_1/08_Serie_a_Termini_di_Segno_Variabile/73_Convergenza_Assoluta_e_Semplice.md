---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - convergenza-assoluta
  - definizione
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 11-13)"
---

# Convergenza assoluta e convergenza semplice

## Serie a termini di segno variabile

> [!abstract] Definizione — convergenza assoluta
> Data una serie $\displaystyle\sum_{n=0}^\infty a_n$, diremo che essa **converge assolutamente** se la serie $\displaystyle\sum_{n=0}^\infty|a_n|$ converge
> (secondo la definizione di serie convergente già vista, cioè $\displaystyle\exists\lim_{N\to\infty}\sum_{n=0}^N|a_n|=M\in\mathbb{R}$, vedi [[48_Studio_del_Carattere_di_una_Serie]]).

> [!note] Osservazione — convergenza semplice
> Per distinguere questa nuova definizione dalla definizione di serie convergente che abbiamo già dato, chiameremo la vecchia nozione di convergenza **«convergenza semplice»**. Se non specificato, si sottintende di parlare di convergenza semplice.

> [!note] Osservazioni
> - $\displaystyle\sum_{n=0}^\infty|a_n|$ converge oppure diverge a $+\infty$, essendo una serie a termini positivi ([[57_Serie_a_Termini_Positivi]]).
> - Una serie a termini positivi converge semplicemente se e solo se converge assolutamente (le due nozioni coincidono).

## Il legame tra le due nozioni
Vale: convergenza assoluta $\Rightarrow$ convergenza semplice ([[74_Criterio_di_Convergenza_Assoluta]]); non vale il viceversa:

$$\text{convergenza assoluta}\ \Rightarrow\ \text{convergenza semplice},\qquad\text{convergenza assoluta}\ \not\Leftarrow\ \text{convergenza semplice}$$

> [!example] Esempio — convergenza semplice ma non assoluta
> Esistono serie che convergono semplicemente ma non assolutamente. Ad esempio
> $$\sum_{n=1}^\infty\frac{(-1)^n}{n^\alpha}\qquad\alpha\in(0,1]$$
> - converge semplicemente per il criterio di Leibniz ([[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]);
> - non converge assolutamente (quindi «diverge assolutamente») perché la serie dei moduli è $\displaystyle\sum_{n=1}^\infty\frac{1}{n^\alpha}$, serie armonica generalizzata con esponente $\alpha\in(0,1]$, che diverge ([[60_Serie_Armonica_Generalizzata]]).

## Note collegate
- [[74_Criterio_di_Convergenza_Assoluta]]
- [[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]
- [[77_Esempio_Serie_Alternata_con_Parametro_alpha]]
- [[57_Serie_a_Termini_Positivi]]
- [[48_Studio_del_Carattere_di_una_Serie]]
- [[00_MOC_Analisi_1]]

#AM1/serie/convergenza-assoluta
