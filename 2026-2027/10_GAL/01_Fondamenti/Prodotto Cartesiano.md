---
created: 2026-09-16
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/0
  - argomento/fondamenti
aliases: []
---
[[00_GAL_Fondamenti|⬅️ Torna a Fondamenti]]

# Prodotto Cartesiano

### Definizione 0.1

Dati due insiemi $A$ e $B$ qualsiasi, il **prodotto cartesiano** $A \times B$ è l'insieme delle coppie **ordinate** $(a,b)$ con $a \in A$ e $b \in B$:

$$
A \times B = \{ (a,b) \mid a \in A,\ b \in B \}
$$

### Esempio 1 — il piano cartesiano

$\mathbb{R}^2 = \mathbb{R} \times \mathbb{R}$. Gli elementi del piano cartesiano sono **punti**. Fissato un sistema di riferimento (gli assi cartesiani), ogni punto è identificato in modo univoco da una coppia $(x,y)$ con $x \in \mathbb{R}$, $y \in \mathbb{R}$.

![[Pasted image 20261014151604.png]]

### Esempio 2 — voti sufficienti

$A = \{\text{valutazioni sufficienti per la parte di esercizi}\} = \{16,17,18,\dots,32\}$

$B = \{\text{valutazioni sufficienti per la parte di teoria}\} = \{16,17,\dots,32\}$

$A \times B$ è l'insieme delle coppie di valutazioni sufficienti per esercizi e teoria (in quest'ordine).

- $a = 28,\ b = 22 \;\leadsto\; \text{voto} = 70\%\, a + 30\%\, b = \frac{7}{10}\cdot 28 + \frac{3}{10}\cdot 22$
- $a = 22,\ b = 28 \;\leadsto\; \text{voto} = \frac{7}{10}\cdot 22 + \frac{3}{10}\cdot 28$

Le due coppie danno voti diversi, perché $(28,22) \neq (22,28)$.

### Esempio 3 — moneta e dado

- $A = \{\text{esiti del lancio della moneta}\} = \{T, C\}$
- $B = \{\text{esiti del lancio del dado}\} = \{1,2,3,4,5,6\}$

$$
A \times B = \{(T,1),(T,2),\dots,(T,6),(C,1),(C,2),\dots,(C,6)\}
$$

è l'insieme degli esiti del lancio simultaneo di una moneta e di un dado.

---
Successivo: [[Relazione Binaria]]
