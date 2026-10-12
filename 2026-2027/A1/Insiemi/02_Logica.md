---
tags:
  - AM1
  - logica
  - proposizioni
  - predicati
  - quantificatori
data: 2026-09-14
fonte: Lezione 1
---

# Elementi di Logica

> [!warning] Def. Proposizione
> Una **proposizione** è un enunciato non contenente variabili libere a cui si possa attribuire in maniera univoca il valore vero o falso. Si indicano con $P, Q, \dots$

> [!warning] Def. Predicato
> Un **predicato** è un enunciato contenente variabili libere, il cui valore di verità (vero o falso) dipende dal valore delle variabili. Tuttavia, per ogni assegnazione delle variabili, il predicato deve collassare su una proposizione, quindi essere oggettivamente vero o falso. Si indicano con $P(x,y,\dots)$, $Q(x,y,\dots)$, dove $x, y, \dots$ sono le variabili libere.

> [!note] Osservazione
> L'insieme (o gli insiemi) in cui variano le variabili è parte della definizione del predicato.

## Connettivi Logici

| Simbolo           | Significato     | Definizione                                                                                                                                                        |
| ----------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| $\land$           | "e"             | Date $P,Q$ proposizioni, $P \land Q$ è vera se sono vere entrambe, falsa altrimenti                                                                                |
| $\lor$            | "o"             | Date $P,Q$ proposizioni, $P \lor Q$ è vera se almeno una è vera                                                                                                    |
| $\neg$            | "non"           | Data $P$ proposizione, $\neg P$ è vera se $P$ è falsa e viceversa                                                                                                  |
| $\Rightarrow$     | "se ... allora" | Date $P,Q$ proposizioni, $P \Rightarrow Q$ è vera se $P$ è vera e $Q$ è vera, oppure se $P$ è falsa (qualunque sia il valore di verità di $Q$); è falsa altrimenti |
| $\Leftrightarrow$ | "se e solo se"  | Date $P,Q$ proposizioni, $P \Leftrightarrow Q$ è vera se $P$ e $Q$ sono entrambe vere o entrambe false, falsa altrimenti                                           |

## Quantificatori

Per assegnare un valore di verità ad un predicato è necessario "saturare" le variabili libere. In tal modo si ottiene una proposizione con il suo valore di verità, vero o falso. Ciò può essere fatto fissando il valore delle variabili oppure con l'uso di quantificatori:

- $\forall$ "per ogni"
- $\exists$ "esiste"
- $\exists!$ "esiste ed è unico"
- $\nexists$ "non esiste"

> [!warning] Def. Implicazione universale
> Un enunciato che presenta la struttura
> $$\forall x \in A \quad P(x) \Rightarrow Q(x)$$
> con $A$ insieme, $P(x)$ e $Q(x)$ predicati per $x \in A$, prende il nome di **implicazione universale**.

> [!warning] Def. Condizione necessaria e sufficiente
> Date $P, Q$ proposizioni (predicati), se $P \Rightarrow Q$ è vera, diremo che $P$ è condizione **sufficiente** affinché $Q$, e $Q$ è condizione **necessaria** per $P$.
>
> Se $P \Leftrightarrow Q$ è vera, diremo che $P$ è necessaria e sufficiente affinché $Q$, e viceversa.

> [!example] Esempio
> $P$: il triangolo è equilatero
> $Q$: il triangolo è isoscele
>
> $P \Rightarrow Q$ vera $\;\Rightarrow\;$ $P$ è sufficiente per $Q$, e $Q$ è necessaria per $P$

### Note collegate
- [[00_MOC_A1]]
- [[01_Insiemi_Numerici]] — notazione insiemistica
- [[03_Dimostrazioni]] — uso di ipotesi, tesi, implicazioni e controesempi
- [[04_Dimostrazione_per_Assurdo]]
- [[05_Dimostrazione_per_Induzione]]