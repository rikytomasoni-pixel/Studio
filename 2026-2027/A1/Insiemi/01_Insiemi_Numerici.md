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
> - $\forall$ "per ogni"
> - $\in$ "appartiene"
> - $\setminus$ (es. $A \setminus B$) "escluso"
> - elementi minuscoli, insiemi maiuscoli
> - $\subset$ "è contenuto"

Ogni numero razionale $x \in \mathbb{Q}$ può essere rappresentato da infinite frazioni equivalenti.

Ogni numero razionale $x \in \mathbb{Q}$ può essere rappresentato anche in formato decimale:

$$\mathbb{Q} = \left\{ x = \pm a_0,\, a_1 a_2 a_3 \dots a_k : a_0 \in \mathbb{N},\ a_k \in [0,9],\ \forall k \in \mathbb{N},\ k \neq 0 \right\}$$

Le rappresentazioni decimali dei numeri razionali sono tutte **o finite** (c'è solo un numero finito di cifre decimali $\neq 0$) **o infinite e periodiche** (numero infinito di cifre decimali che però ad un certo punto si ripetono periodicamente).

> [!note] Osservazione
> Mancano gli infiniti non periodici — cioè i numeri la cui rappresentazione decimale è infinita e *non* periodica: sono i numeri irrazionali (vedi sotto).

$$\mathbb{R} = \left\{ x = \pm a_0,\, a_1 a_2 a_3 \dots a_k : a_0 \in \mathbb{N},\ a_k \in [0,9],\ \forall k \in \mathbb{N},\ k \neq 0 \right\} \quad \text{numeri reali}$$

con rappresentazione decimale finita o infinita, periodica o no.

I numeri in $\mathbb{R} \setminus \mathbb{Q}$, cioè i numeri $x \in \mathbb{R} : x \notin \mathbb{Q}$, si dicono **irrazionali**.

$$\mathbb{C} = \{ z = a + ib : a, b \in \mathbb{R},\ i^2 = -1 \} \quad \text{numeri complessi}$$

$$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}$$

### Note collegate
- [[00_MOC_A1]]
- [[02_Logica]] — simboli e notazione logica
- [[06_Campi_Ordinati]] — $\mathbb{R}$ e $\mathbb{Q}$ come campi ordinati
- [[08_Estremo_Superiore_Inferiore]] — $\mathbb{Q}$ non soddisfa la proprietà dell'estremo superiore
- [[10_Retta_Reale_Intervalli]] — rappresentazione geometrica e densità di $\mathbb{Q}$ in $\mathbb{R}$
- [[13_Numeri_Complessi]] — costruzione di $\mathbb{C}$