---
tags: [GAL, matrici, efficienza, complessita, lezione-3]
data: 2026-09-30
lezione: 3
fonte: "GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 33-34)"
---

# Efficienza computazionale e proprietà delle operazioni

> [!note] Osservazione (Domanda)
> D. perché mi impegno di elencare le proprietà delle operazioni?
> R. sono estremamente significative per l'efficienza computazionale!

> [!example] Esempio — distributiva a destra
> $\lambda(A+B) = \lambda A + \lambda B$ ([[36_Prodotto_di_una_Matrice_per_uno_Scalare]])
>
> «La complessità di un calcolo viene spesso stimata calcolando quanti prodotti devo calcolare».

![[efficienzaComputazionaleEsempio.png]]

Prendiamo due matrici $A, B \in M_{\mathbb{R}}(m,n)$:
- quanti prodotti calcolo in $\lambda(A+B)$? $\quad m \cdot n$ (perché $A + B \in M_{\mathbb{K}}(m,n)$)
- quanti prodotti calcolo in $\lambda A + \lambda B$? $\quad 2\, m \cdot n$

**Valutazione empirica**

![[complessitaEmpirica.png]]

Lo stesso confronto per il prodotto matriciale è in [[44_Proprieta_del_Prodotto_Matriciale]].

## Note collegate
- [[36_Prodotto_di_una_Matrice_per_uno_Scalare]]
- [[35_Somma_tra_Matrici]]
- [[44_Proprieta_del_Prodotto_Matriciale]]
- Indice: [[04_Indice_Lezione_3]] · [[00_MOC_GAL]]

#GAL/matrici/efficienza-computazionale
