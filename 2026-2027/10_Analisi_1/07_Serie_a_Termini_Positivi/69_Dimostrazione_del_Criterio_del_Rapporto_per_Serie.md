---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - criterio-del-rapporto
  - dimostrazione
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 2-6)"
---

# Dimostrazione del criterio del rapporto per serie

> [!abstract] Teorema (criterio del rapporto per serie)
> Sia $a_n$ una successione a termini (definitivamente) positivi ed esista
> $$\ell=\lim_{n\to\infty}\frac{a_{n+1}}{a_n}\in\overline{\mathbb{R}}$$
> Allora:
> 1. se $\ell>1$ (incluso $+\infty$), allora $\displaystyle\sum_{n=1}^\infty a_n$ **diverge** e $\displaystyle\lim_{n\to\infty}a_n=+\infty$;
> 2. se $0\leq\ell<1$, allora $\displaystyle\sum_{n=1}^\infty a_n$ **converge** e $\displaystyle\lim_{n\to\infty}a_n=0$.

L'enunciato è in [[64_Criterio_del_Rapporto_per_Serie]]. Qui si riporta la dimostrazione.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** pag. 2, subito sotto l'enunciato. **Cosa cercare:** retta reale con i punti $0$ e $1$ e due piccoli intorni di $\ell$ (di ampiezza $\varepsilon$, estremi $\ell-\varepsilon$ e $\ell+\varepsilon$): in rosso per il caso $\ell<1$ (a sinistra di $1$), in blu per il caso $\ell>1$ (a destra di $1$).

## Dimostrazione

Per semplicità supponiamo $a_n>0$ $\forall n\in\mathbb{N}$ e $\ell=\lim\frac{a_{n+1}}{a_n}\in\overline{\mathbb{R}}$, $\ell\neq1$.

### Caso 1: $\ell>1$
Ci sono due casi: $\ell\in(1,+\infty)$ oppure $\ell=+\infty$.

**Se $\ell\in(1,+\infty)$**, scegliamo $\varepsilon=\frac{\ell-1}{2}>0$ nella definizione di limite. Allora esiste $N\in\mathbb{N}$ tale che $\forall n\geq N$
$$1<\frac{\ell+1}{2}=\ell-\varepsilon<\frac{a_{n+1}}{a_n}\ (<\ell+\varepsilon)$$
Dunque $\forall n\geq N$ vale $\dfrac{a_{n+1}}{a_n}>\dfrac{\ell+1}{2}>1$. Se chiamiamo $q=\dfrac{\ell+1}{2}>1$:
$$a_{n+1}>q\,a_n\qquad\forall n\geq N\qquad(\ast)$$
Per iterazione della formula $(\ast)$, $\forall n\geq N$:
$$a_{n+1}>q\,a_n>q^2a_{n-1}>q^3a_{n-2}>\dots>q^{n+1-N}a_N$$
cioè $a_{n+1}>\dfrac{a_N}{q^N}\,q^{n+1}$ e quindi, definitivamente in $n\in\mathbb{N}$ ($\forall n\geq N+1$),
$$a_n>\frac{a_N}{q^N}\,q^n>0\qquad(\ast\ast)$$

- Per il teorema del confronto per serie ([[58_Criterio_del_Confronto_per_Serie]]), poiché $\sum_{n=0}^\infty q^n$ con $q>1$ diverge (serie geometrica di ragione $q=\frac{\ell+1}{2}>1$, vedi [[50_Serie_Geometrica]]), diverge anche la serie $\sum a_n$.
- Per il teorema del confronto per successioni divergenti ([[35_Teoremi_del_Confronto]]), poiché $\lim q^n=+\infty$, per $(\ast\ast)$ vale $\lim a_n=+\infty$.

**Se $\ell=+\infty$**, per definizione di limite infinito per $M=2$ esiste $N\in\mathbb{N}$ tale che $\forall n\geq N$
$$\frac{a_{n+1}}{a_n}>M=2\ \Rightarrow\ a_{n+1}>q\,a_n\ \text{ con }q=2>1\ \ \forall n\geq N$$
e da qui si ripete l'argomento precedente, da $(\ast)$ in poi.

### Caso 2: $0\leq\ell<1$
Per $\varepsilon=\frac{1-\ell}{2}>0$ esiste $N\in\mathbb{N}$ tale che $\forall n\geq N$
$$(\ell-\varepsilon<)\ \frac{a_{n+1}}{a_n}<\ell+\varepsilon=\frac{1+\ell}{2}<1\ \Rightarrow\ \frac{a_{n+1}}{a_n}<\frac{1+\ell}{2}=q<1$$
Definiamo $q=\dfrac{1+\ell}{2}\in(0,1)$; allora
$$0<a_{n+1}<q\,a_n\qquad\forall n\geq N\qquad(\ast\ast\ast)$$
Quindi $\forall n\geq N$
$$0<a_{n+1}<q\,a_n<q^2a_{n-1}<q^3a_{n-2}<\dots<q^{n+1-N}a_N$$
$$\Rightarrow\ 0<a_{n+1}<\frac{a_N}{q^N}\,q^{n+1}\ \Rightarrow\ \text{definitivamente in }n\ (\forall n\geq N+1)\quad 0<a_n<\frac{a_N}{q^N}\,q^n$$

- Poiché $0<q<1$, per il criterio del confronto per serie, essendo $\sum_{n=0}^\infty q^n=\frac{1}{1-q}$ convergente (serie geometrica di ragione $q=\frac{1+\ell}{2}\in(0,1)$), deve essere convergente anche $\sum a_n$.
- Per confronto per successioni (due carabinieri), essendo $\lim q^n=0$, deve essere $\lim a_n=0$.

$\blacksquare$

## Note collegate
- [[64_Criterio_del_Rapporto_per_Serie]]
- [[65_Criterio_della_Radice_per_Serie]]
- [[50_Serie_Geometrica]]
- [[58_Criterio_del_Confronto_per_Serie]]
- [[39_Criterio_del_Rapporto]] (versione per successioni)
- [[70_Esempio_Serie_a_alla_n_su_n_alla_n]]
- [[00_MOC_Analisi_1]]

#AM1/serie/dimostrazione-criterio-del-rapporto
