---
created: 2026-09-16
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/0
aliases: []
---
[[00_GAL_Indice|⬅️ Torna all'Indice GAL]]

# Prodotto Cartesiano, Relazioni Binarie e Relazioni di Equivalenza

> Lezione 0 — 16.09.2026. Argomenti: [[#Prodotto Cartesiano|Prodotto Cartesiano]], [[#Relazione Binaria|Relazione Binaria]], [[#Relazione di Equivalenza|Relazione di Equivalenza]].

## Modalità d'esame (introduzione al corso)

L'esame si compone di due parti, ciascuna con voto massimo $32$:

- **Esercizi**: 10 quesiti a risposta chiusa e 2 esercizi a risposta aperta.
- **Teoria**: quesiti vero/falso di carattere teorico (definizioni, teoremi, ...).

Soglie per ciascuna parte: $\ge 18/32$ (verde), tra $16/32$ e $18/32$ (arancione), $< 16/32$ (rosso).

**Voto finale** $= 70\%\ \text{esercizi} + 30\%\ \text{teoria}$: la prova è superata se il voto finale è $> 17$, non superata se $\le 17$.

### Prova in itinere (30 ottobre 2026)

- 5 quesiti e 1 esercizio (nessuna teoria).
- **Obiettivo**: valutazione formativa; non esonera dai contenuti della prima parte del corso.
- **Effetto**: può avere unicamente un effetto premiale sul voto dell'esame finale (valido per il primo appello invernale a cui si partecipa).

Siano $V$ il voto della prova in itinere e $W$ il voto degli esercizi dell'esame completo:

$$
\text{voto esercizi} =
\begin{cases}
W & \text{se } W \ge V \\[4pt]
\dfrac{1}{3}V + \dfrac{2}{3}W & \text{se } W < V
\end{cases}
$$

**Esempi**

1. Prova in itinere $23$, esercizi di gennaio $27$ $\Rightarrow$ $27$.
2. Prova in itinere $23$, esercizi di febbraio $21$ (a gennaio non ha partecipato) $\Rightarrow \frac{1}{3}\cdot 23 + \frac{2}{3}\cdot 21 \approx 21.67$.

### Quiz conoscitivo

In aula è stato proposto un quiz (Wooclap) con tre grafici radar sulle abitudini quotidiane, sulle fonti di informazione e sulla dimestichezza con nozioni matematiche.

> **Figura (disegno senza immagine disponibile):**
>
> Tre diagrammi radar (esagono, pentagono, esagono). (1) Frequenza di situazioni quotidiane: ritardo dei mezzi pubblici, interazione con IA, attività sportiva, ascolto di podcast, interazione sui social network, uso di strumenti basati sull'algebra lineare. (2) Fonti di informazione: famiglia, rete amicale, agenti IA, motori di ricerca, libri; i valori massimi sono per motori di ricerca e agenti IA. (3) Dimestichezza matematica: insiemi e funzioni, numeri reali, ragionamento logico, prodotti cartesiani, vettori nel piano e nello spazio, geometria analitica di rette e piani; scala da 1 a 5.

## Prodotto Cartesiano

### Definizione 0.1

Dati due insiemi $A$ e $B$ qualsiasi, il **prodotto cartesiano** $A \times B$ è l'insieme delle coppie **ordinate** $(a,b)$ con $a \in A$ e $b \in B$:

$$
A \times B = \{ (a,b) \mid a \in A,\ b \in B \}
$$

### Esempio 1 — il piano cartesiano

$\mathbb{R}^2 = \mathbb{R} \times \mathbb{R}$. Gli elementi del piano cartesiano sono **punti**. Fissato un sistema di riferimento (gli assi cartesiani), ogni punto è identificato in modo univoco da una coppia $(x,y)$ con $x \in \mathbb{R}$, $y \in \mathbb{R}$.

> **Figura (disegno senza immagine disponibile):**
>
> Piano cartesiano con asse $x$ orizzontale e asse $y$ verticale. Il punto $P = (x_P, y_P) = (2,4)$ (in rosso) ha coordinate $x_P$ sull'asse $x$ e $y_P$ sull'asse $y$ (indicate con parentesi graffe). Il punto $Q$ (in blu) è $Q = (4,2)$, cioè $P$ con le coordinate scambiate: l'**ordine** conta.

Se scambio l'ordine, $(4,2) \in \mathbb{R} \times \mathbb{R}$ è un punto diverso ($Q$).

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

## Relazione Binaria

> **Domanda**: come può essere utile il prodotto cartesiano?

### Definizione 0.2

Una **relazione (binaria)** tra l'insieme $A$ e l'insieme $B$ è un sottoinsieme del prodotto cartesiano $A \times B$.

### Esempio 4

- $A = \{\text{studenti/studentesse in aula}\}$, $B = \{\text{colori}\}$.
- Relazione: «$a$ ha il colore migliore $b$».
- $A \times B = \{(a,b) \mid a \text{ studente/studentessa},\ b \text{ colore}\}$.
- La relazione è $R \subseteq A \times B$, con $R = \{(a,b) \mid a \text{ studente/studentessa},\ b \text{ colore del suo migliore}\}$.

### Relazioni su un solo insieme

Ci concentriamo sulle relazioni binarie tra elementi dello stesso insieme: $R \subseteq A \times A$.

**Esempio.** $A = \{\text{studenti/studentesse dell'aula}\}$, $R = \{a_1 \text{ è in relazione con } a_2 \text{ se il colore del migliore di } a_1 \text{ è uguale al colore del migliore di } a_2\}$.

## Proprietà delle relazioni

### Proprietà riflessiva

Una relazione soddisfa la **proprietà riflessiva** se ogni elemento è in relazione con se stesso.

$$
R \subseteq A \times A \text{ è riflessiva se } \forall a \in A,\ (a,a) \in R
$$

*Esempio*: la relazione sopra è riflessiva.

### Proprietà simmetrica

Una relazione soddisfa la **proprietà di simmetria** se vale: $a$ in relazione con $b$ $\Rightarrow$ $b$ in relazione con $a$.

$$
R \subseteq A \times A \text{ è simmetrica se } (a,b) \in R \Rightarrow (b,a) \in R
$$

*Esempio*: la relazione sopra è simmetrica.

### Proprietà transitiva

Una relazione soddisfa la **proprietà transitiva** se vale: $a$ in relazione con $b$ e $b$ in relazione con $c$ $\Rightarrow$ $a$ in relazione con $c$.

$$
R \subseteq A \times A \text{ è transitiva se } \left.\begin{array}{l}(a,b) \in R \\ (b,c) \in R\end{array}\right\} \Rightarrow (a,c) \in R
$$

*Esempio*: la relazione sopra è transitiva.

## Relazione di Equivalenza

$$
\left.\begin{array}{l}\text{riflessività} \\ \text{simmetria} \\ \text{transitività}\end{array}\right\} \Longleftrightarrow \text{relazione di equivalenza}
$$

Una relazione è di **equivalenza** se e solo se è riflessiva, simmetrica e transitiva.

Vedi anche: [[#Prodotto Cartesiano|Prodotto Cartesiano]], [[#Relazione Binaria|Relazione Binaria]], [[#Relazione di Equivalenza|Relazione di Equivalenza]], [[#Proprietà riflessiva|Proprietà Riflessiva]], [[#Proprietà simmetrica|Proprietà Simmetrica]], [[#Proprietà transitiva|Proprietà Transitiva]].
