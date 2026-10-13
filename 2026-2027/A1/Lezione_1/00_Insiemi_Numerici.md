---
tags:
  - AM1
  - matematica
  - analisi
  - insiemi-numerici
data: 2026-09-14
fonte: Lezione 1
---

# Insiemi Numerici

$$\mathbb{N},\ \mathbb{Z},\ \mathbb{Q},\ \mathbb{R},\ \mathbb{C}$$

- $\mathbb{N} = \{0, 1, 2, 3, \dots\}$ — numeri naturali, interi non negativi
- $\mathbb{Z} = \{\dots, -3, -2, -1, 0, 1, 2, 3, \dots\}$ — numeri interi relativi
- $$\mathbb{Q} = \left\{ \frac{m}{n} : m, n \in \mathbb{Z},\ n \neq 0 \right\} \quad \text{numeri razionali}$$

> [!info] Notazione
> - $:$ "tale che" (anche $\mid$)
> - $\in$ "appartiene" — $a \in A$: l'elemento $a$ appartiene all'insieme $A$
> - $\forall$ "per ogni"
> - $\notin$ "non appartiene" — $a \notin A$: l'elemento $a$ non appartiene all'insieme $A$
> - $\setminus$ — $A \setminus B$ è l'insieme degli elementi di $A$ che non sono elementi di $B$
> - $\subset$ — $A \subset B$: $A$ è un sottoinsieme di $B$

Identifichiamo $\dfrac{m}{n} = \dfrac{a}{b}$ in $\mathbb{Q}$, con $m, n, a, b \in \mathbb{Z}$, $n \neq 0$ e $b \neq 0$, se $mb = na$.

Ogni numero razionale $r \in \mathbb{Q}$ può essere rappresentato da infinite frazioni equivalenti.

Ad esempio: $\dfrac{3}{7} = \dfrac{6}{14} = \dfrac{-12}{-28} = \dots$

Ogni numero razionale $r \in \mathbb{Q}$ può essere rappresentato anche in formato decimale:

$$r = \pm a_0,\, a_1 a_2 a_3 a_4 \dots a_k \dots \quad a_0 \in \mathbb{N},\ a_k \in \{0,1,2,3,4,5,6,7,8,9\}\ \forall k \in \mathbb{N},\ k \neq 0$$

Es: $\dfrac{3}{2} = 1{,}50000\dots$ ; $\dfrac{1}{3} = \dfrac{-5}{-15} = 0{,}3333\dots = 0{,}\overline{3}$

Le rappresentazioni decimali dei numeri razionali sono tutte **o finite** (cioè solo un numero finito di cifre decimali è diverso da 0) **o infinite e periodiche** (cioè hanno un numero infinito di cifre decimali non nulle, che però da un certo punto in poi si ripetono periodicamente).

Es: $r = 7489\dots0723{,}894037\dots59\overline{749\dots187}$

$$\mathbb{Q} = \left\{ \frac{m}{n} : m, n \in \mathbb{Z},\ n \neq 0 \right\} = \left\{ r = \pm a_0,\, a_1 a_2 a_3 \dots a_k \dots : a_0 \in \mathbb{N},\ a_k \in \{0,1,2,3,4,5,6,7,8,9\}\ \forall k \in \mathbb{N},\ k \neq 0,\ \text{e la rappresentazione decimale è finita o infinita e periodica} \right\}$$

> [!note] Osservazione
> $0{,}\overline{9} = 1 = 1{,}000\dots$
> $0{,}4\overline{9} = 0{,}5$
> $0{,}475\overline{9} = 0{,}476$
> $\dots$

$$\mathbb{R} = \left\{ r = \pm a_0,\, a_1 a_2 a_3 \dots a_k \dots : a_0 \in \mathbb{N},\ a_k \in \{0,1,2,3,4,5,6,7,8,9\}\ \forall k \in \mathbb{N},\ k \neq 0 \right\} \quad \text{numeri reali}$$

con rappresentazione decimale finita o infinita, periodica o no.

I numeri in $\mathbb{R} \setminus \mathbb{Q}$, cioè i numeri $r \in \mathbb{R} : r \notin \mathbb{Q}$, si dicono **irrazionali**.

$$\mathbb{C} = \{ z = a + ib : a, b \in \mathbb{R},\ i^2 = -1 \} \quad \text{numeri complessi}$$

$$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}$$

> [!warning] Aggiunte presenti nella versione precedente ma non nel PDF manoscritto
> - Notazione: "elementi minuscoli, insiemi maiuscoli".
> - Osservazione: i numeri con rappresentazione decimale infinita e *non* periodica non compaiono in $\mathbb{Q}$: sono i numeri irrazionali.

### Note collegate
- [[00_MOC_A1]]
- [[01_Logica]] — simboli e notazione logica
- [[00_Campi_Ordinati]] — $\mathbb{R}$ e $\mathbb{Q}$ come campi ordinati
- [[02_Estremo_Superiore_Inferiore]] — $\mathbb{Q}$ non soddisfa la proprietà dell'estremo superiore
- [[04_Retta_Reale_Intervalli]] — rappresentazione geometrica e densità di $\mathbb{Q}$ in $\mathbb{R}$
- [[01_Numeri_Complessi]] — costruzione di $\mathbb{C}$