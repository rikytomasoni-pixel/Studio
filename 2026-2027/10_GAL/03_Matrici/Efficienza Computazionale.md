---
created: 2026-09-30
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Efficienza Computazionale

Sono estremamente significative per l'**efficienza computazionale**! La complessità di un calcolo viene spesso stimata calcolando quanti prodotti tra numeri devo calcolare.

*(Nell'esempio a mano: la somma $1123 + 625 = 1748$ richiede solo addizioni di cifre, mentre il prodotto $1123 \times 625$ richiede il calcolo di tre righe parziali: $5615$, $2246$ (traslato), $6738$ (traslato di due posizioni), da sommare.)*

**Esempio — distributiva a destra** $\lambda(A+B) = \lambda A + \lambda B$. Prendiamo due matrici $A,B \in M_{\mathbb{R}}(m,n)$:

- Quanti prodotti calcolo in $\lambda(A+B)$? $A+B \in M_{\mathbb{K}}(m,n)$, quindi $m \cdot n$ prodotti.
- Quanti prodotti calcolo in $\lambda A + \lambda B$? $2\, m \cdot n$ prodotti.
---
Precedente: [[Prodotto di una Matrice per uno Scalare]]
