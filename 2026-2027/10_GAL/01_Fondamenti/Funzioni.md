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

# Funzioni

### Definizione 1.1

Una **funzione** è una relazione $F$ tra due insiemi $A$ e $B$ ($F \subseteq A \times B$) tale che per ogni ($\forall$) $a \in A$ esiste **uno ed un solo** elemento $b \in B$ tale che $(a,b) \in F$.

- Il primo insieme $A$ si dice **dominio**.
- Il secondo insieme $B$ si dice **codominio**.

La funzione è caratterizzata da tre ingredienti: $A$, $B$ e $F \subseteq A \times B$. Si scrive

$$
F \subseteq A \times B,\ (a,b) \in F \qquad \Longleftrightarrow \qquad F : A \to B,\ F(a) = b
$$

### Esempi

1. $A = \{\text{studenti/studentesse}\}$, $B = \{\text{colori}\}$, $F = \{(\text{studente}, \text{colore}) \mid \text{il migliore di } \_ \text{ è di colore } \_\}$. $F$ è una funzione $F : A \to B$, con $F(x) = $ colore del migliore di $x$.
2. $A = \{\text{studenti/studentesse}\}$, $F \subseteq A \times A$, $F = \{(x,y) \mid \text{il colore del migliore di } x \text{ è lo stesso del migliore di } y\}$. **Questo non è una funzione!** Si prenda un colore per cui ci sono almeno 3 individui $x,y,z$ con il migliore di quel colore: allora $(x,y) \in F$, $(y,z) \in F$, $(x,z) \in F$, cioè ci sono **due coppie con $x$ come primo elemento**.
3. $A = \{\text{anguria, banana, limone, lampone}\}$, $B = \{\text{"a"},\text{"b"},\text{"l"}\}$, $F = \{(\text{anguria},\text{"a"}),(\text{banana},\text{"b"}),(\text{limone},\text{"l"}),(\text{lampone},\text{"l"})\}$ (la funzione «l'iniziale di $\_$ è $\_$»).

### Cardinalità e funzioni

> N.B. Nel caso di insiemi con un numero finito di elementi, il numero di coppie di $F$ (funzione) è uguale al numero di elementi di $A$ (dominio).

Indicando con $\#$ il «numero di elementi di»:

$$
F \subseteq A \times B \text{ funzione} \implies \#F = \#A
$$

**Obiettivo**: data una relazione, come faccio a dimostrare che *non* è una funzione?

---
Precedente: [[Relazione d'Ordine]] · Successivo: [[Excursus Logico, Negazione dell'Implicazione]]
