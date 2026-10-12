---
tags: [GAL, fondamenti, relazioni, ordine, lezione-1]
data: 2026-09-17
lezione: 1
fonte: "GAL_2026-2027_-_20260917_-_LEZIONE_1.pdf (slide 12-13)"
---

# Relazione d'ordine

Dalla lezione di ieri: «non tutte le relazioni sono di equivalenza» (vedi [[14_Relazione_di_Equivalenza]]).

> [!example] Esempio
> $S = \{\text{insieme di tutti gli insiemi}\}$
> $A$ è in relazione con $B$ se $A$ è contenuto in $B$:
> $$A \subseteq B \iff \forall\, a \in A \Rightarrow a \in B$$
>
> - **Riflessività?** ✓ — $A \subseteq A\ \ \forall A \in S$
> - **Simmetria?** ✗ — $A \subsetneq B$ [questa inclusione non può essere invertita]
> - **Transitività?** ✓ — $A \subseteq B,\ B \subseteq C \Rightarrow A \subseteq C$

**!!!** (disegno: diagramma di Venn con $A$ (rosso) dentro $B$ (blu) e un punto in $B$ fuori da $A$)

**!!!** (disegno: tre insiemi annidati $A \subset B \subset C$ a sinistra; $A \subset C$ a destra)

> [!warning] Def. Proprietà di antisimmetria
> Una relazione $R \subseteq S \times S$ si dice **antisimmetrica** se soddisfa la seguente proprietà:
> $A$ è in relazione con $B$ e $B$ è in relazione con $A$ $\Rightarrow A = B$.
> Esempio: $A \subseteq B$ più $B \subseteq A \Rightarrow A = B$.

> [!warning] Def. Relazione d'ordine
> Riflessività, antisimmetria e transitività $\Longleftrightarrow$ **relazione d'ordine**.

## Note collegate
- [[13_Proprieta_Riflessiva_Simmetrica_Transitiva]]
- [[14_Relazione_di_Equivalenza]]
- [[16_Funzioni]]
- Indice: [[02_Indice_Lezione_1]] · [[00_MOC_GAL]]
