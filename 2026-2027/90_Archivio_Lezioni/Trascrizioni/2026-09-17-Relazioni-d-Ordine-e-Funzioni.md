---
created: 2026-09-17
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/1
aliases: []
---
[[00_GAL_Indice|⬅️ Torna all'Indice GAL]]

# Relazioni d'Ordine, Funzioni, Iniettività e Surgettività

> Lezione 1 — 17.09.2026. Dalla lezione di ieri: «non tutte le relazioni sono di equivalenza». Vedi [[2026-09-16-Prodotto-Cartesiano-e-Relazioni#Relazione di Equivalenza|Relazione di Equivalenza]] e [[2026-09-16-Prodotto-Cartesiano-e-Relazioni#Prodotto Cartesiano|Prodotto Cartesiano]].

## Relazione di inclusione tra insiemi

Sia $S = \{\text{insieme di tutti gli insiemi}\}$. Definiamo: $A$ è in relazione con $B$ se $A$ è contenuto in $B$:

$$
A \subseteq B \iff \forall a \in A \Rightarrow a \in B
$$

- **Riflessività**: ✓ — $A \subseteq A$ per ogni $A \in S$.
- **Simmetria**: ✗ — se $A \subsetneq B$ questa inclusione non può essere invertita.
- **Transitività**: ✓ — $A \subseteq B$ e $B \subseteq C$ $\Rightarrow$ $A \subseteq C$.

> **Figura (disegno senza immagine disponibile):**
>
> Diagrammi di Venn. Primo: un ovale rosso $A$ interamente contenuto in un ovale blu $B$, con un punto in $B \setminus A$ (nota: «questa inclusione non può essere invertita»). Secondo: tre ovali concentrici $A \subseteq B \subseteq C$ (rosso, blu, verde), accanto a $A$ dentro $C$, a illustrare la transitività.

### Proprietà antisimmetrica

Una relazione $R \subseteq S \times S$ si dice **antisimmetrica** se soddisfa la seguente proprietà:

$$
\left.\begin{array}{l}A \text{ è in relazione con } B \\ B \text{ è in relazione con } A\end{array}\right\} \Rightarrow A = B
$$

Nel caso dell'inclusione: $A \subseteq B$ e $B \subseteq A$ $\Rightarrow$ $A = B$.

### Relazione d'ordine

$$
\left.\begin{array}{l}\text{riflessività} \\ \text{antisimmetria} \\ \text{transitività}\end{array}\right\} \Longleftrightarrow \text{relazione d'ordine}
$$

Dunque l'inclusione $\subseteq$ è una [[#Relazione d'ordine|Relazione d'Ordine]].

## Funzioni

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

#### Excursus logico

«condizione 1» $\Rightarrow$ «condizione 2» equivale a «negazione di condizione 2» $\Rightarrow$ «negazione di condizione 1» (contronominale).

*Esempio*: «vado in bici in solito» $\Rightarrow$ «frequenza cardiaca aumenta» equivale a «frequenza cardiaca non aumenta» $\Rightarrow$ «non sono andato in bici in solito».

Applicando la contronominale:

$$
\#F \neq \#A \implies F \subseteq A \times B \text{ NON è una funzione}
$$

**Attenzione!** Il fatto che il numero di elementi di $F$ e $A$ sia lo stesso non garantisce che io abbia una funzione. Ci sono relazioni $F \subseteq A \times B$ con $\#F = \#A$ che non sono funzioni.

*Esempio*: $A = \{\text{anguria, banana, lampone, limone}\}$, $B = \{\text{"a"},\text{"b"},\text{"l"}\}$, $\#A = 4$. La relazione $\{(\text{anguria},\text{"a"}),(\text{banana},\text{"b"}),(\text{lampone},\text{"l"}),(\text{anguria},\text{"b"})\}$ ha $\#F = 4$ ma **non è una funzione** (anguria ha due immagini e limone nessuna).

## Iniettività e surgettività delle funzioni

> **Figura (disegno senza immagine disponibile):**
>
> Quattro diagrammi a frecce tra due insiemi $A$ e $B$ (ovali con punti). (1) Frutta → lettere: anguria→"a", banana→"b", limone→"l", lampone→"l" (frecce rosse), $F$ = «l'iniziale di $\_$ è $\_$»: **non iniettiva** (due frecce arrivano in "l") ma **surgettiva**. (2) Tre frecce blu da tre punti di $A$ verso tre punti distinti di $B$ (che ne ha di più): **iniettiva**, non surgettiva. (3) Tre frecce blu che convergono su uno stesso punto di $B$: non iniettiva. (4) Surgettività: «ogni elemento del codominio è raggiunto da almeno una freccia»; esempio con $B$ avente punti non raggiunti → **non è surgettiva**.

### Definizione 1.2

- Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **iniettiva** se, presi $a_1, a_2 \in A$ e $(a_1,b),(a_2,b) \in F$ (cioè $F(a_1) = b$, $F(a_2) = b$, cioè $F(a_1) = F(a_2)$), allora $a_1 = a_2$.

  Equivalentemente:

  $$
  \forall a_1, a_2 \in A:\ F(a_1) = F(a_2) \Rightarrow a_1 = a_2 \qquad (F \text{ iniettiva})
  $$

  $$
  a_1 \neq a_2 \Rightarrow F(a_1) \neq F(a_2)
  $$

- Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **surgettiva** se $\forall b \in B$ esiste ($\exists$) almeno un elemento $a \in A$ tale che $(a,b) \in F$. Equivalentemente:

  $$
  F^{-1}(b) = \{a \in A \mid F(a) = b\} \neq \emptyset
  $$

  dove $F^{-1}(b)$ è l'insieme delle **controimmagini** di $b$.

- Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **biettiva** se è simultaneamente iniettiva e surgettiva.

> **Figura (disegno senza immagine disponibile):**
>
> Due ovali ($A$ a sinistra, $B$ a destra) con cinque punti ciascuno, collegati da cinque frecce blu parallele, una per ogni punto: ogni elemento di $B$ è raggiunto esattamente una volta.

> **N.B.** Le biezioni producono un abbinamento perfetto tra gli elementi del dominio e quelli del codominio.

## Prodotti cartesiani di più di due insiemi

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

Vedi anche: [[#Funzioni|Funzione]], [[#Iniettività e surgettività delle funzioni|Funzione Iniettiva]], [[#Iniettività e surgettività delle funzioni|Funzione Surgettiva]], [[#Iniettività e surgettività delle funzioni|Funzione Biettiva]], [[#Relazione d'ordine|Relazione d'Ordine]], [[#Proprietà antisimmetrica|Proprietà Antisimmetrica]].
