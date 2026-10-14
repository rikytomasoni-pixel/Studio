---
created: 2026-09-17
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/1
  - argomento/fondamenti
aliases: []
origine: UpdateVault
---
[[00_GAL_Fondamenti|⬅️ Torna a Fondamenti]]

# Prodotto Cartesiano di più Insiemi

> [!note] Osservazione (Domanda)
> D. è possibile considerare prodotti cartesiani che coinvolgono più di 2 insiemi?
> R. Sì.

> [!warning] Def. Prodotto cartesiano di tre insiemi
> $A, B, C$ tre insiemi arbitrari.
> $$A \times B \times C = \{\, (a,b,c) \mid a \in A,\ b \in B,\ c \in C \,\}$$
> **Terne ordinate** di elementi scelti in $A$, poi $B$, poi $C$.

> [!example] Esempio
> $\mathbb{R}^3 = \mathbb{R} \times \mathbb{R} \times \mathbb{R} = \{\, (x,y,z) \mid x \in \mathbb{R},\ y \in \mathbb{R},\ z \in \mathbb{R} \,\}$
> - $x$: spostamento nella direzione dell'asse $x$
> - $y$: spostamento nella direzione dell'asse $y$
> - $z$: spostamento nella direzione dell'asse $z$

> [!note] Osservazione (Domanda)
> D. perché non ne abbiamo parlato prima?
> R. in realtà l'abbiamo fatto! Dati $A, B, C$:
> - Step 1: $A \times B = S = \{(a,b) \mid a \in A,\ b \in B\}$
> - Step 2: $S \times C = \{(s,c) \mid s \in S,\ c \in C\}$
> - Step 3: $(A \times B) \times C = \{((a,b),c) \mid (a,b) \in A \times B,\ c \in C\}$

> [!note] Osservazione (Domanda)
> D. Che relazione c'è tra la costruzione delle terne e la costruzione con due coppie (consecutive)?
> $$F : (A \times B) \times C \to A \times B \times C,\qquad ((a,b),c) \mapsto (a,b,c)$$
> $F$ è sia iniettiva sia suriettiva ([[Iniettività Surgettività Biettività]]).
> **MORALE:** le due costruzioni producono sempre due insiemi con una naturale funzione biettiva tra essi, cioè dal punto di vista insiemistico sono portatori della stessa informazione!

---
Precedente: [[Iniettività Surgettività Biettività]]
