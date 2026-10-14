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

### Valutazione empirica

> **Figura (disegno senza immagine disponibile):**
>
> Due grafici per matrici di tipo $(1000,1500)$. Sinistra «Confronto tra le strategie»: asse $x$ = numero di ripetizioni (0–1000), asse $y$ = tempo in secondi; due rette crescenti, $\lambda(A+B)$ (blu, circa 5 s a 1000 ripetizioni) e $\lambda A + \lambda B$ (arancione, circa 7,5 s). Destra «Rapporto tra i tempi di esecuzione»: rapporto Strategia 2 / Strategia 1 in funzione del numero di ripetizioni; parte da circa 0,6 per 0 ripetizioni, sale rapidamente e si stabilizza intorno a 1,5.

Conclusione empirica: la strategia $\lambda(A+B)$ è circa $1.5$ volte più veloce di $\lambda A + \lambda B$.

---
Precedente: [[Prodotto di una Matrice per uno Scalare]]
