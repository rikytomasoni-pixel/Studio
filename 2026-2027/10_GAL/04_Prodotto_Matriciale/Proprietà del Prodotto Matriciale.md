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

# Proprietà del Prodotto Matriciale

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

---
Precedente: [[PageRank e Matrice di Google]] · Successivo: [[Matrice Identità e Matrici Diagonali]]
