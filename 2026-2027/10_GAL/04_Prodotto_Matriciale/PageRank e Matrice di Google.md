---
created: 2026-10-01
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/prodotto_matriciale
aliases: []
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# PageRank e Matrice di Google

$S = \{\text{insieme delle pagine web (di interesse)}\}$, $S \times S = \{(\text{pagina 1},\text{pagina 2}) \mid \text{pagina 1},\text{pagina 2} \in S\}$ (pagina 1 = pagina di **arrivo**, pagina 2 = pagina di **partenza**).

Consideriamo funzioni $f : S \times S \to \mathbb{R}$ che misurano la probabilità di navigare tra le pagine (secondo criteri assegnati), cioè una matrice $A : S \times S \to \mathbb{R}$ con

$$
a_{ij} = \text{probabilità di passare dalla pagina } j \text{ alla pagina } i
$$

Google considera 2 comportamenti:

- **Tap random surfer**: mi muovo solo con i link ipertestuali.
- **Keyboard random surfer**: mi muovo solo scrivendo l'indirizzo esplicito della pagina.

*Random* significa che ogni possibile trasferimento è equiprobabile.

> **Figura (disegno senza immagine disponibile):**
>
> Due grafi orientati a tre nodi (1, 2, 3). **TAP** (rosso): $1 \to 2$ con prob. $\frac12$, $1 \to 3$ con prob. $\frac12$, $2 \to 1$ con prob. $1$, $3 \to 2$ con prob. $1$. **KEYBOARD** (blu): grafo completo con cappi su ogni nodo, ogni arco (compresi i cappi) con probabilità $\frac13$.

Matrici (righe = pagina di arrivo, colonne = pagina di partenza):

$$
T = \begin{bmatrix} 0 & 1 & 0 \\ \tfrac12 & 0 & 1 \\ \tfrac12 & 0 & 0 \end{bmatrix},
\qquad
K = \begin{bmatrix} \tfrac13 & \tfrac13 & \tfrac13 \\ \tfrac13 & \tfrac13 & \tfrac13 \\ \tfrac13 & \tfrac13 & \tfrac13 \end{bmatrix}
$$

### Matrice di Google

$G$ = matrice di Google = media pesata tra le due matrici. Con $p \in (0,1)$ (*damping number*):

$$
G = p\,T + (1-p)\,K
$$

**Idea di Google**: la significatività di una pagina corrisponde a per quanto tempo / quante volte la visito.

- $G$ descrive le probabilità di navigazione in 1 step;
- $G^2 = G\cdot G$ descrive le probabilità di navigazione in 2 step;
- $G^3 = G\cdot G\cdot G$ in 3 step;
- $\dots$
- $G^k$ descrive le probabilità di navigazione in $k$ step.

### Esempio (Python): evoluzione del PageRank

> **Figura (disegno senza immagine disponibile):**
>
> Tre grafi con 5 nodi (0–4) disposti ad arco, con frecce curve tra i nodi, colorati secondo il PageRank (barra colori giallo=alto, viola scuro=basso). Iterazione 0: tutti i nodi gialli (PageRank uniforme ≈0.20). Iterazione 3: il nodo 0 resta giallo, i nodi 1 e 2 arancio, i nodi 3 e 4 più scuri (rosso/viola). Iterazione 10: la distribuzione si è stabilizzata (nodo 0 massimo, 1 e 2 intermedi, 3 e 4 minimi).

**Domande**:

- È sempre vero che questo processo si stabilizza?
- È importante come allochiamo le masse iniziali?

---
Precedente: [[Prodotto e Composizione di Funzioni]] · Successivo: [[Proprietà del Prodotto Matriciale]]
