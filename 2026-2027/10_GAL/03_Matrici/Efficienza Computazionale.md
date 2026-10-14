---
created: 2026-09-30
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
origine: UpdateVault
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Efficienza Computazionale

> [!note] Osservazione (Domanda)
> D. perché mi impegno di elencare le proprietà delle operazioni?
> R. sono estremamente significative per l'efficienza computazionale!

> [!example] Esempio — distributiva a destra
> $\lambda(A+B) = \lambda A + \lambda B$ ([[Prodotto di una Matrice per uno Scalare]])
>
> «La complessità di un calcolo viene spesso stimata calcolando quanti prodotti devo calcolare».

**DISEGNO NON RAPPRESENTABILE** (disegno: addizione in colonna $1123 + 625 = 1748$ e moltiplicazione in colonna $1123 \times 625$ con i prodotti parziali $5615$, $2246$, $6738$ incolonnati e traslati) *(dove cercarlo: GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 33-34))*

Prendiamo due matrici $A, B \in M_{\mathbb{R}}(m,n)$:
- quanti prodotti calcolo in $\lambda(A+B)$? $\quad m \cdot n$ (perché $A + B \in M_{\mathbb{K}}(m,n)$)
- quanti prodotti calcolo in $\lambda A + \lambda B$? $\quad 2\, m \cdot n$

**Valutazione empirica**

**DISEGNO NON RAPPRESENTABILE** (due grafici Python per matrici di tipo $(1000,1500)$: «Confronto tra le strategie», tempo in secondi contro numero di ripetizioni per $\lambda(A+B)$ (blu) e $\lambda A + \lambda B$ (arancione), crescita lineare con la seconda sopra la prima; «Rapporto tra i tempi di esecuzione», strategia 2 / strategia 1, che si stabilizza intorno a $1.5$) *(dove cercarlo: GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 33-34))*

Lo stesso confronto per il prodotto matriciale è in [[Proprietà del Prodotto Matriciale]].

---
Precedente: [[Prodotto di una Matrice per uno Scalare]]
