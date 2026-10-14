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

# Relazione d'Ordine

Sia $S = \{\text{insieme di tutti gli insiemi}\}$. Definiamo: $A$ è in relazione con $B$ se $A$ è contenuto in $B$:

$$
A \subseteq B \iff \forall a \in A \Rightarrow a \in B
$$

- **Riflessività**: ✓ — $A \subseteq A$ per ogni $A \in S$.
- **Simmetria**: ✗ — se $A \subsetneq B$ questa inclusione non può essere invertita.
- **Transitività**: ✓ — $A \subseteq B$ e $B \subseteq C$ $\Rightarrow$ $A \subseteq C$.
![[transitivitàInsiemi.png]]

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

Dunque l'inclusione $\subseteq$ è una Relazione d'Ordine.

---
Precedente: [[Relazione di Equivalenza]] · Successivo: [[Funzioni]]
