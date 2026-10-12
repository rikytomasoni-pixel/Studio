---
tags: [GAL, fondamenti, funzioni, lezione-1]
data: 2026-09-17
lezione: 1
fonte: "GAL_2026-2027_-_20260917_-_LEZIONE_1.pdf (slide 13-17)"
---

# Funzioni

> [!warning] Def. 1.1 Funzione
> Una **funzione** è una [[12_Relazione_Binaria]] $F$ tra due insiemi $A$ e $B$ ($F \subseteq A \times B$) tale che per ogni ($\forall$) $a \in A$ esiste uno ed un solo elemento $b \in B$ tale che $(a,b) \in F$.
> Il primo insieme $A$ si dice **dominio**; il secondo insieme $B$ si dice **codominio**.

La funzione è caratterizzata da 3 ingredienti:
- $A$
- $B$
- $F \subseteq A \times B$

Notazione: $F \subseteq A \times B$, $(a,b) \in F$ — oppure — $F : A \to B$, $F(a) = b$.

> [!example] Esempio (funzione)
> $A = \{\text{studenti / studentesse}\}$, $B = \{\text{colori}\}$
> $F = \{(\text{studente/essa},\ \text{colore}) \mid \text{la maglia di \_\_ è di colore \_\_}\}$
> $F$ è una funzione, $F : A \to B$: per studente/studentessa $x$, $F(x) = \text{colore della maglia di } x$.

> [!example] Esempio (non è una funzione)
> $A = \{\text{studenti / studentesse}\}$, $F \subseteq A \times A$
> $F = \{(x,y) \mid \text{il colore della maglia di } x \text{ è lo stesso della maglia di } y\}$
> Questo non è una funzione!
> Prendiamo un colore per cui ci sono almeno 3 individui con la maglia del colore scelto: $x, y, z$.
> $(x,y) \in F$, $(y,z) \in F$, $(x,z) \in F$ — due coppie con $x$ come primo elemento.

**!!!** (disegno: le tre coppie $(x,y),(y,z),(x,z)$ con $x$ cerchiato e frecce rosse sulle due coppie che hanno $x$ come primo elemento)

> [!example] Esempio
> $A = \{\text{arancia, banana, limone, lampone}\}$, $B = \{\text{"a", "b", "l"}\}$
> $F \subseteq A \times B$
> $F = \{(\text{arancia},\text{"a"}),\ (\text{banana},\text{"b"}),\ (\text{limone},\text{"l"}),\ (\text{lampone},\text{"l"})\}$

> [!note] Osservazione
> N.B. (nel caso di insiemi con un numero finito di elementi) il numero di coppie di $F$ (funzione) è uguale al numero di elementi di $A$ (dominio). Notazione: $\# =$ «numero di elementi di».

> [!abstract] Teorema (Proprietà)
> $F \subseteq A \times B$ funzione $\overset{\text{implica}}{\Longrightarrow} \#F = \#A$.
> Equivalentemente: $\#F \neq \#A \Rightarrow F \subseteq A \times B$ **non è una funzione**!

**Obiettivo:** data una relazione, come faccio a dimostrare che non è una funzione? → [[17_Excursus_Logico_Negazione_Implicazione]]

> [!example] Esempio
> $A = \{\text{arancia, banana, lampone, limone}\}$, $B = \{\text{"a", "b", "l"}\}$
> $F$ funzione $\Rightarrow \#F = 4$, $\#A = 4$.

> [!note] Osservazione
> **ATTENZIONE!** Il fatto che il numero di elementi di $F$ e $A$ sia lo stesso non garantisce che io abbia una funzione. Ci sono relazioni $F \subseteq A \times B$ con $\#F = \#A$ che non sono funzioni:
> $\{(\text{arancia},\text{"a"}),\ (\text{banana},\text{"b"}),\ (\text{lampone},\text{"l"}),\ (\text{arancia},\text{"b"})\}$ — **non è una funzione**.

## Note collegate
- [[12_Relazione_Binaria]]
- [[17_Excursus_Logico_Negazione_Implicazione]]
- [[18_Iniettivita_Suriettivita_Biettivita]]
- [[30_Matrici_come_Rappresentazione_di_Funzioni]]
- Indice: [[02_Indice_Lezione_1]] · [[00_MOC_GAL]]
