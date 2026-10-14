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

# Logica e Quantificatori

**Definizione.** Una **proposizione** è un enunciato che non contiene variabili libere a cui si possa attribuire in maniera univoca il valore vero o falso (solo uno dei due, non entrambi).

- «$3 > 4$» è una proposizione ✓ (falsa);
- «la pizza è buona» non lo è ✗;
- «$n$ è pari» non lo è ✗ (contiene la variabile libera $n$).

Le proposizioni si indicano con $P, Q, \dots$

**Definizione.** Si dice **predicato** un enunciato contenente variabili libere il cui valore di verità, vero o falso, dipende dal valore delle variabili. Tuttavia per ogni assegnazione delle variabili il predicato deve essere oggettivamente vero o falso (non entrambi) — cioè deve essere una proposizione. I predicati si indicano con $P(x,y,\dots)$, $Q(x,y,\dots)$, dove $x,y$ sono le variabili libere.

*Esempi*: $P(n)$: «$n$ è pari» ✓; $Q(f)$: «$f$ è derivabile» ✓.

> **Oss.** La dichiarazione dell'insieme in cui variano le variabili $x,y,\dots$ è parte della definizione del predicato.

### Connettivi logici

- $\wedge$ **e**: date $P,Q$ proposizioni, $P \wedge Q$ è la proposizione vera se sono vere entrambe $P$ e $Q$; falsa altrimenti.
- $\vee$ **o**: $P \vee Q$ è vera se è vera $P$, o $Q$, o entrambe (cioè almeno una delle 2); falsa altrimenti.
- $\neg$ **negazione (non)**: $\neg P$ è vera se $P$ è falsa, falsa se $P$ è vera.
- $\Rightarrow$ **implicazione** («se... allora...»): $P \Rightarrow Q$ è vera se $P$ è vera e $Q$ è vera, oppure se $P$ è falsa (qualunque sia il valore di verità di $Q$); è falsa altrimenti.
- $\Leftrightarrow$ **doppia implicazione** («se e solo se»): $P \Leftrightarrow Q$ è vera se $P,Q$ sono entrambe vere oppure entrambe false; falsa altrimenti.

| $P$ | $Q$ | $P \wedge Q$ | $P \vee Q$ | $\neg P$ | $P \Rightarrow Q$ | $P \Leftrightarrow Q$ |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| V | V | V | V | F | V | V |
| V | F | F | V | F | F | F |
| F | V | F | V | V | V | F |
| F | F | F | F | V | V | V |

### Quantificatori

Per assegnare un valore di verità a un predicato è necessario «saturare» le variabili libere: in tal modo si ottiene una proposizione con il suo valore di verità. Ciò può essere fatto fissando le variabili o tramite l'uso di **quantificatori**:

- $\forall$ per ogni;
- $\exists$ esiste;
- $\exists!$ esiste ed è unico;
- $\nexists$ non esiste.

*Esempio* con $P(n)$: «$n$ è pari», $n \in \mathbb{N}$:

| Proposizione | Valore |
|---|---|
| $n = 5$: $n$ è pari | F |
| $\forall n \in \mathbb{N}$: $n$ è pari | F |
| $\exists n \in \mathbb{N}$: $n$ è pari | V |
| $\exists! n \in \mathbb{N}$: $n$ è pari | F |
| $\nexists n \in \mathbb{N}$: $n$ è pari | F |

> **Oss.** Se $P(x)$ è un predicato, $x \in A$: $\forall x\ P(x)$, $\exists x : P(x)$, $\exists! x : P(x)$, $\nexists x : P(x)$, $x = x_0\ P(x)$ (cioè $P(x_0)$) sono proposizioni diverse.

**Definizione.** Un enunciato che presenta la struttura

$$
\forall x \in A \quad P(x) \Rightarrow Q(x)
$$

con $A$ insieme e $P(x), Q(x)$ per $x \in A$ predicati, prende il nome di **implicazione universale**.

---
Precedente: [[Insiemi Numerici]] · Successivo: [[Condizioni Necessarie e Sufficienti]]
