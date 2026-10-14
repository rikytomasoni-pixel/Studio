---
created: 2026-09-14
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/1
  - argomento/fondamenti
aliases: []
---
[[00_A1_Fondamenti|⬅️ Torna a Fondamenti]]

# Insiemi Numerici

$\mathbb{N}, \mathbb{Z}, \mathbb{Q}, \mathbb{R}, \mathbb{C}$

- $\mathbb{N} = \{0,1,2,3,\dots\}$: insieme dei **numeri naturali** (interi non negativi).
- $\mathbb{Z} = \{\dots,-3,-2,-1,0,1,2,3,\dots\}$: insieme degli **interi relativi**.
- $\mathbb{Q} = \left\{ \frac{m}{n} : m,n \in \mathbb{Z},\ n \neq 0 \right\}$: **numeri razionali**.

### Notazione

- $:$ «tale che» (anche $\mid$);
- $\in$ «appartiene»: $a \in A$ significa che l'elemento $a$ appartiene all'insieme $A$;
- $\notin$ «non appartiene»;
- $\setminus$: $A \setminus B$ è l'insieme degli elementi di $A$ che non sono elementi di $B$;
- $\subset$: $A \subset B$ significa che $A$ è un sottoinsieme di $B$;
- $\forall$ «per ogni».

### Frazioni equivalenti e rappresentazione decimale

Identifichiamo $\frac{m}{n} = \frac{a}{b}$ in $\mathbb{Q}$ (con $m,n,a,b \in \mathbb{Z}$, $n \neq 0$, $b \neq 0$) se $mb = na$. Ogni numero razionale $r \in \mathbb{Q}$ può essere rappresentato da infinite frazioni equivalenti; ad esempio $\frac37 = \frac{6}{14} = \frac{-12}{-28} = \dots$

Ogni numero razionale può essere rappresentato anche in **forma decimale**:

$$
r = \pm a_0,a_1a_2a_3a_4\dots a_k\dots, \qquad a_0 \in \mathbb{N},\ a_k \in \{0,1,\dots,9\}\ \ \forall k \in \mathbb{N},\ k \neq 0
$$

*Esempi*: $\frac32 = 1{,}50000\dots$; $\frac13 = \frac{-5}{-15} = 0{,}3333\dots = 0{,}\overline{3}$.

Le rappresentazioni decimali dei numeri razionali sono tutte **finite** (cioè solo un numero finito di cifre decimali è diverso da 0) oppure **infinite e periodiche** (un numero infinito di cifre decimali non nulle che, da un certo punto in poi, si ripetono periodicamente). Si può quindi scrivere

$$
\mathbb{Q} = \left\{ \frac{m}{n} : m,n \in \mathbb{Z},\ n \neq 0 \right\} = \{ r = \pm a_0,a_1a_2a_3\dots a_k\dots \,:\, a_0 \in \mathbb{N},\ a_k \in \{0,\dots,9\},\ \text{rappresentazione decimale finita o infinita e periodica}\}
$$

> **Osservazione**: $0{,}\overline{9} = 1 = 1{,}000\dots$; $0{,}4\overline{9} = 0{,}5$; $0{,}475\overline{9} = 0{,}476$; ecc.

### I numeri reali e i complessi

$$
\mathbb{R} = \{ r = \pm a_0,a_1a_2a_3\dots a_k\dots \,:\, a_0 \in \mathbb{N},\ a_k \in \{0,\dots,9\},\ \text{rappresentazione decimale finita o infinita, periodica o no} \}
$$

$\mathbb{R}$ è l'insieme dei **numeri reali**. I numeri in $\mathbb{R} \setminus \mathbb{Q}$, cioè i numeri $r \in \mathbb{R}$ tali che $r \notin \mathbb{Q}$, si dicono **irrazionali**.

$$
\mathbb{C} = \{ z = a + ib : a,b \in \mathbb{R},\ i^2 = -1 \}
$$

è l'insieme dei **numeri complessi**. Vale la catena di inclusioni

$$
\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}
$$

---
Successivo: [[Logica e Quantificatori]]
