---
tags: [GAL, matrici, matrici-simili, relazione-di-equivalenza, dimostrazione, lezione-23]
data: 2026-11-19
lezione: 23
fonte: "GAL 2026-2027 - 20261119 - LEZIONE 23.pdf (slide 193)"
---

# La similitudine tra matrici è una relazione di equivalenza

> [!abstract] Proposizione
> La similitudine tra matrici è una **relazione di equivalenza** su $M_{\mathbb{K}}(n,n)$ ([[14_Relazione_di_Equivalenza]]).

## Riflessività
"Ogni matrice è simile a se stessa": con $P=\mathrm{Id}$,
$$A=\mathrm{Id}\,A\,\mathrm{Id}^{-1},\qquad A=\mathrm{Id}^{-1}A\,\mathrm{Id}.$$

## Simmetria
Se $A=PBP^{-1}$ e $B=P^{-1}AP$, con $Q=P^{-1}$:
$$A=Q^{-1}BQ,\qquad B=QAQ^{-1}.$$

## Transitività
$A,B$ simili: $A=PBP^{-1}$, $B=P^{-1}AP$. $B,C$ simili: $B=SCS^{-1}$, $C=S^{-1}BS$. Allora
$$A=PBP^{-1}=P(SCS^{-1})P^{-1}=(PS)\,C\,(S^{-1}P^{-1})=(PS)\,C\,(PS)^{-1},$$
$$C=S^{-1}BS=S^{-1}(P^{-1}AP)S=\dots=(PS)^{-1}A\,(PS)\ \Rightarrow\ A,C\text{ simili.}$$

## Classi di similitudine
Ogni **strato** (classe di equivalenza) contiene matrici simili. Lo strato contenente $A$ è
$$[A]=\{B\in M_{\mathbb{K}}(n,n)\mid A,B\text{ sono simili}\}.$$

![[StratodiMatriciSimili.png]]

## Note collegate
- [[172_Matrici_Simili_Definizione_23_2]]
- [[14_Relazione_di_Equivalenza]]
- [[13_Proprieta_Riflessiva_Simmetrica_Transitiva]]
- [[174_Matrici_Diagonalizzabili_Definizione_23_3]]
- Indice: [[24_Indice_Lezione_23]] · [[00_MOC_GAL]]

#GAL/matrici/similitudine-equivalenza
