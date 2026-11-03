---
tags: [GAL, dimensione, generatori, indipendenza-lineare, proprieta, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 122-123)"
---

# Significato della dimensione

Conseguenza del [[117_Lemma_Fondamentale_Teorema_15_1|lemma fondamentale]]: se $V$ è uno spazio vettoriale **finitamente generato** (cioè esistono $\underline{v}_1,\dots,\underline{v}_n$ tali che $V=\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$), il numero massimo di vettori linearmente indipendenti è **limitato**.

> [!tip] Proprietà
> - La dimensione di $V$ è il **numero massimo** di vettori linearmente indipendenti.
> - La dimensione di $V$ è il **numero minimo** di vettori generatori.

> [!note] N.B. Estendere un insieme indipendente
> Se $\{\underline{w}_1,\dots,\underline{w}_k\}$ è linearmente indipendente e $k<\dim V$, allora esiste $\underline{u}$ tale che $\{\underline{w}_1,\dots,\underline{w}_k,\underline{u}\}$ è ancora linearmente indipendente. In tal caso
> $$\operatorname{Span}(\underline{w}_1,\dots,\underline{w}_k)\subsetneq\operatorname{Span}(\underline{w}_1,\dots,\underline{w}_k,\underline{u})$$
> con dimensioni rispettivamente $k$ e $k+1$.

## Relazione tra dimensione, generatori e indipendenza lineare
Sia $\dim(V)=n$ e consideriamo $n$ vettori $\{\underline{v}_1,\dots,\underline{v}_n\}$ di $V$:

| Se... | ...allora |
|---|---|
| $\{\underline{v}_1,\dots,\underline{v}_n\}$ generatori **e** linearmente indipendenti | $\dim(V)=n$ (è una base, vedi [[100_Base_di_uno_Spazio_Vettoriale]]) |
| $\{\underline{v}_1,\dots,\underline{v}_n\}$ generatori e $\dim(V)=n$ | $\{\underline{v}_1,\dots,\underline{v}_n\}$ linearmente indipendenti |
| $\{\underline{v}_1,\dots,\underline{v}_n\}$ linearmente indipendenti e $\dim(V)=n$ | $\{\underline{v}_1,\dots,\underline{v}_n\}$ generatori |

> [!note] Osservazione (non presente negli appunti)
> Perché valgono le ultime due righe (ragionamento mio, da confrontare con la prof):
> - *Generatori $\Rightarrow$ indipendenti.* Se fossero dipendenti, uno sarebbe ridondante ([[99_Dipendenza_Lineare_e_Vettori_Ridondanti]]) e $V$ sarebbe generato da $n-1$ vettori; per il lemma fondamentale ogni insieme indipendente avrebbe al più $n-1$ elementi, ma una base ne ha $n$: assurdo.
> - *Indipendenti $\Rightarrow$ generatori.* Se non generassero $V$, per il N.B. precedente si potrebbe aggiungere $\underline{u}$ restando indipendenti, ottenendo $n+1$ vettori indipendenti: assurdo perché il massimo è $\dim V=n$.

## Note collegate
- [[117_Lemma_Fondamentale_Teorema_15_1]]
- [[118_Teorema_della_Dimensione_Teorema_15_2]]
- [[102_Dimensione_di_uno_Spazio_Vettoriale]]
- [[98_Vettori_Linearmente_Indipendenti]]
- [[96_Insieme_di_Generatori]]
- Successiva: [[120_Spazi_Vettoriali_Finitamente_Generati_e_Non]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/dimensione/significato
