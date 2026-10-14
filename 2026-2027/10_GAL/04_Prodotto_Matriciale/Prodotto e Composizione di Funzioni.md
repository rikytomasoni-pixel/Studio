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

# Prodotto e Composizione di Funzioni

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

---
Precedente: [[Prodotto Righe per Colonne]] · Successivo: [[PageRank e Matrice di Google]]
