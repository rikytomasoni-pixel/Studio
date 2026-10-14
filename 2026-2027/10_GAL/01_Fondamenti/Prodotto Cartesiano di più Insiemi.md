---
created: 2026-09-17
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/1
  - argomento/fondamenti
aliases: []
---
[[00_GAL_Fondamenti|⬅️ Torna a Fondamenti]]

# Prodotto Cartesiano di più Insiemi

**Domanda**: è possibile considerare prodotti cartesiani che coinvolgono più di 2 insiemi? **Risposta**: sì.

Siano $A, B, C$ tre insiemi arbitrari:

$$
A \times B \times C = \{(a,b,c) \mid a \in A,\ b \in B,\ c \in C\}
$$

sono **terne ordinate** di elementi scelti in $A$, poi $B$, poi $C$. Ad esempio:

$$
\mathbb{R}^3 = \mathbb{R} \times \mathbb{R} \times \mathbb{R} = \{(x,y,z) \mid x \in \mathbb{R},\ y \in \mathbb{R},\ z \in \mathbb{R}\}
$$

dove $x$ è lo spostamento nella direzione dell'asse $x$, $y$ nella direzione dell'asse $y$, $z$ nella direzione dell'asse $z$.

**Domanda**: perché non ne abbiamo parlato prima? **Risposta**: in realtà l'abbiamo fatto! Procedendo a passi:

1. $A \times B = S = \{(a,b) \mid a \in A,\ b \in B\}$
2. $S \times C = \{(s,c) \mid s \in S,\ c \in C\}$
3. $(A \times B) \times C = \{((a,b),c) \mid (a,b) \in A \times B,\ c \in C\}$

**Domanda**: che relazione c'è tra la costruzione delle terne e la costruzione con due coppie (consecutive)?

$$
\begin{aligned}
F &: (A \times B) \times C \to A \times B \times C \\
&\ \ ((a,b),c) \longmapsto (a,b,c)
\end{aligned}
$$

$F$ è sia iniettiva sia surgettiva, cioè **biettiva**.

> **Morale**: le due costruzioni producono sempre due insiemi con una naturale funzione biettiva tra essi, cioè dal punto di vista insiemistico sono portatori della stessa informazione!

---
Precedente: [[Iniettività Surgettività Biettività]]
