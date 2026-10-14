---
created: 2026-10-01
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
aliases: []
---
[[00_GAL_Indice|⬅️ Torna all'Indice GAL]]

# Prodotto Matriciale (righe per colonne), PageRank e Matrice Identità

> Lezione 4 — 01.10.2026. Prosegue da [[2026-09-30-Matrici-Somma-e-Prodotto-per-Scalare|Lezione 3 (somma e prodotto per scalare)]]. Argomenti: [[#Prodotto matriciale righe per colonne|Prodotto Matriciale]], [[#Matrice identità|Matrice Identità]], [[#Diagonale principale e matrici diagonali|Matrice Diagonale]].

## Postilla: l'opposto di una matrice

L'esistenza dell'opposto rispetto alla somma, ad esempio:

$$
A = \begin{bmatrix} 1 & -1 \\ 0 & 2 \end{bmatrix}, \qquad
A' = \begin{bmatrix} -1 & 1 \\ 0 & -2 \end{bmatrix}
= \begin{bmatrix} (-1)\cdot 1 & (-1)\cdot(-1) \\ (-1)\cdot 0 & (-1)\cdot 2 \end{bmatrix} = (-1)A
$$

$\Rightarrow$ d'ora in poi l'elemento opposto di una matrice $A$ verrà denotato con $-A$.

## Prodotto matriciale righe per colonne

$$
\cdot : M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(n,p) \to M_{\mathbb{K}}(m,p), \qquad (A,B) \longmapsto AB
$$

Il numero di colonne di $A$ deve coincidere con il numero di righe di $B$. Con $A = [a_{ij}]$ ($i=1,\dots,m$; $j=1,\dots,n$), $B = [b_{ij}]$ ($i=1,\dots,n$; $j=1,\dots,p$) e $C = AB = [c_{ij}]$ ($i=1,\dots,m$; $j=1,\dots,p$):

$$
c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + \dots + a_{in}b_{nj} = \sum_{k=1}^{n} a_{ik}\, b_{kj}
$$

### Esempi

**Riga per colonna.** Se $A \in M_{\mathbb{K}}(1,n)$ e $B \in M_{\mathbb{K}}(n,1)$, allora $AB = C \in M_{\mathbb{K}}(1,1)$, $C = [c_{11}]$:

$$
c_{11} = \sum_{k=1}^{n} a_{1k}\, b_{k1} = a_{11}b_{11} + a_{12}b_{21} + \dots + a_{1n}b_{n1}
$$

**Esempio numerico.** $A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \in M_{\mathbb{K}}(2,2)$, $B = \begin{bmatrix} 0 & 1 & -1 \\ 0 & -1 & 2 \end{bmatrix} \in M_{\mathbb{K}}(2,3)$, quindi $AB = C \in M_{\mathbb{K}}(2,3)$. L'elemento $c_{ij}$ è il prodotto della riga $i$ di $A$ per la colonna $j$ di $B$:

$$
\begin{aligned}
c_{11} &= \begin{bmatrix}1 & 2\end{bmatrix}\begin{bmatrix}0\\0\end{bmatrix} = 1\cdot 0 + 2\cdot 0 = 0 \\
c_{12} &= \begin{bmatrix}1 & 2\end{bmatrix}\begin{bmatrix}1\\-1\end{bmatrix} = 1\cdot 1 + 2\cdot(-1) = -1 \\
c_{13} &= \begin{bmatrix}1 & 2\end{bmatrix}\begin{bmatrix}-1\\2\end{bmatrix} = 1\cdot(-1) + 2\cdot 2 = 3 \\
c_{21} &= \begin{bmatrix}3 & 4\end{bmatrix}\begin{bmatrix}0\\0\end{bmatrix} = 0 \\
c_{22} &= \begin{bmatrix}3 & 4\end{bmatrix}\begin{bmatrix}1\\-1\end{bmatrix} = 3\cdot 1 + 4\cdot(-1) = -1 \\
c_{23} &= \begin{bmatrix}3 & 4\end{bmatrix}\begin{bmatrix}-1\\2\end{bmatrix} = 3\cdot(-1) + 4\cdot 2 = 5
\end{aligned}
$$

$$
AB = \begin{bmatrix} 0 & -1 & 3 \\ 0 & -1 & 5 \end{bmatrix}
$$

> **Figura (disegno senza immagine disponibile):**
>
> Schema colorato: $A$ (2×2) con la prima riga evidenziata in verde e la seconda in blu; $B$ (2×3) con le tre colonne evidenziate in rosso, viola e giallo; la matrice $C = AB$ (2×3) ha ogni cella all'incrocio tra la striscia-riga di $A$ e la striscia-colonna di $B$ corrispondenti.

## Perché tutto questo? Il prodotto codifica la composizione di funzioni

Siano $F = \{\text{anguria, limone, lampone}\}$, $L = \{\text{"a"},\text{"b"},\text{"l"}\}$, $T = \{\text{vocale},\text{consonante}\}$. Siano $A : F \to L$ («$\in F$ ha iniziale $\in L$») e $B : L \to T$ («$\in L$ è una $\in T$»), rappresentate con matrici indicatrici (colonne = elementi del dominio, righe = elementi del codominio):

$$
A = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}
\ \ \begin{matrix}\text{"a"} \\ \text{"b"} \\ \text{"l"}\end{matrix}
\quad (\text{colonne: anguria, limone, lampone}),
\qquad
B = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}
\ \ \begin{matrix}\text{vocale} \\ \text{consonante}\end{matrix}
\quad (\text{colonne: "a", "b", "l"})
$$

Posso moltiplicare $A$ e $B$? In che ordine? $A \cdot B$ **non si può calcolare**, $B \cdot A$ **si può calcolare**:

$$
BA = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}
\begin{bmatrix} 1 & 0 & 0 \\ 0 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}
= \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 1 \end{bmatrix}
$$

con righe (vocale, consonante) e colonne (anguria, limone, lampone): è la funzione composta $F \to T$.

> **Figura (disegno senza immagine disponibile):**
>
> Diagramma con tre ovali: $F$ (anguria, limone, lampone), $L$ ("a", "b", "l"), $T$ (vocale, consonante). Frecce blu $A$: anguria→"a", limone→"l", lampone→"l". Frecce verdi $B$: "a"→vocale, "b"→consonante, "l"→consonante. Frecce rosse (archi sopra e sotto) rappresentano la composizione diretta $F \to T$: anguria→vocale, limone→consonante, lampone→consonante.

> **Morale**: il prodotto matriciale è congeniato per poter codificare la **composizione funzionale**!!!

## Esempio: come funziona Google — parte 1

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

## Proprietà del prodotto matriciale

Per $M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(n,p) \to M_{\mathbb{K}}(m,p)$:

- **Distributiva a destra**: $\forall A \in M_{\mathbb{K}}(m,n)$, $\forall B,C \in M_{\mathbb{K}}(n,p)$: $A(B+C) = AB + AC$ (entrambi in $M_{\mathbb{K}}(m,p)$).

> **Attenzione all'efficienza computazionale**: confrontando le strategie $A(B+C)$ e $AB + AC$ per matrici di tipo $(500,750)$ e $(750,650)$ si osserva sperimentalmente che $A(B+C)$ è nettamente più veloce.

> **Figura (disegno senza immagine disponibile):**
>
> Due grafici. Sinistra «Confronto tra le strategie»: tempo in secondi (0–20) vs numero di ripetizioni (0–500); $A(B+C)$ (blu) cresce fino a circa 10 s, $AB+AC$ (arancione) fino a circa 19,5 s. Destra «Rapporto tra i tempi di esecuzione»: rapporto Strategia 2 / Strategia 1 tra 1.6 e 2.2 circa, con un massimo di ≈2.2 intorno alle 330 ripetizioni.

- **Distributiva a sinistra**: $\forall A,B \in M_{\mathbb{K}}(m,n)$, $\forall C \in M_{\mathbb{K}}(n,p)$: $(A+B)C = AC + BC$.
- **Associativa**: $\forall A \in M_{\mathbb{K}}(m,n)$, $\forall B \in M_{\mathbb{K}}(n,p)$, $\forall C \in M_{\mathbb{K}}(p,q)$: $(AB)C = A(BC) = ABC$, con $AB \in M_{\mathbb{K}}(m,p)$ e $BC \in M_{\mathbb{K}}(n,q)$.
- **Omogeneità**: $\forall \lambda \in \mathbb{K}$, $\forall A \in M_{\mathbb{K}}(m,n)$, $\forall B \in M_{\mathbb{K}}(n,p)$: $\lambda(AB) = (\lambda A)B = A(\lambda B)$.
- **Esistenza dell'elemento neutro** (rispetto al prodotto):
  - **a destra**: $\exists N_D \in M_{\mathbb{K}}(n,n)$ t.c. $\forall A \in M_{\mathbb{K}}(m,n)$, $AN_D = A$;
  - **a sinistra**: $\exists N_S \in M_{\mathbb{K}}(m,m)$ t.c. $\forall A \in M_{\mathbb{K}}(m,n)$, $N_S A = A$.

  *Chi sono $N_D$ e $N_S$?*

## Matrice identità

### Definizione

La **matrice identità** di tipo $(k,k)$ è la matrice

$$
\mathrm{Id}_k = \begin{bmatrix} 1 & 0 & \cdots & 0 \\ 0 & 1 & & \vdots \\ \vdots & & \ddots & 0 \\ 0 & \cdots & 0 & 1 \end{bmatrix} \in M_{\mathbb{K}}(k,k),
\qquad
(\mathrm{Id}_k)_{ij} = \begin{cases} 1 & i = j \\ 0 & i \neq j \end{cases}
$$

$\Rightarrow$ $N_D = \mathrm{Id}_n$ e $N_S = \mathrm{Id}_m$.

## Diagonale principale e matrici diagonali

### Definizione

Gli elementi che occupano le posizioni $(i,i)$ formano la **diagonale principale** di una matrice. Le matrici quadrate in cui tutte le entrate della matrice fuori dalla diagonale principale sono nulle si dicono **matrici diagonali**.

**Esempio**

$$
\begin{bmatrix} * & 0 & \cdots & 0 \\ 0 & * & & \vdots \\ \vdots & & \ddots & 0 \\ 0 & \cdots & 0 & * \end{bmatrix}
$$

dove i simboli $*$ (sulla diagonale principale) sono valori qualsiasi.

- $\mathrm{Id}_n$ è diagonale;
- la matrice nulla quadrata è diagonale;
- $\begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}$ **non è** una matrice diagonale (gli 1 sono sulla diagonale secondaria).

Vedi anche: [[2026-09-25-Proprieta-delle-Funzioni-Composizione-e-Inversa#7. Composizione di funzioni|Composizione di Funzioni]], PageRank, [[#Matrice di Google|Matrice di Google]], [[2026-09-30-Matrici-Somma-e-Prodotto-per-Scalare#Notazione e casi speciali|Matrice Nulla]].
