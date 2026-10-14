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

# Relazione d'Ordine

Dalla lezione di ieri: «non tutte le relazioni sono di equivalenza» (vedi [[Relazione di Equivalenza]]).

> [!example] Esempio
> $S = \{\text{insieme di tutti gli insiemi}\}$
> $A$ è in relazione con $B$ se $A$ è contenuto in $B$:
> $$A \subseteq B \iff \forall\, a \in A \Rightarrow a \in B$$
>
> - **Riflessività?** ✓ — $A \subseteq A\ \ \forall A \in S$
> - **Simmetria?** ✗ — $A \subsetneq B$ [questa inclusione non può essere invertita]
> - **Transitività?** ✓ — $A \subseteq B,\ B \subseteq C \Rightarrow A \subseteq C$

![[simmetriaInsiemi.png]]
%% originale: **!!!** (disegno: diagramma di Venn con $A$ (rosso) dentro $B$ (blu) e un punto in $B$ fuori da $A$) %%

![[transitivitàInsiemi.png]]
%% originale: **!!!** (disegno: tre insiemi annidati $A \subset B \subset C$ a sinistra; $A \subset C$ a destra) %%

> [!warning] Def. Proprietà di antisimmetria
> Una relazione $R \subseteq S \times S$ si dice **antisimmetrica** se soddisfa la seguente proprietà:
> $A$ è in relazione con $B$ e $B$ è in relazione con $A$ $\Rightarrow A = B$.
> Esempio: $A \subseteq B$ più $B \subseteq A \Rightarrow A = B$.

> [!warning] Def. Relazione d'ordine
> Riflessività, antisimmetria e transitività $\Longleftrightarrow$ **relazione d'ordine**.

---
Precedente: [[Relazione di Equivalenza]] · Successivo: [[Funzioni]]
