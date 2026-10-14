---
created: 2026-10-07
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/eliminazione_di_gauss
aliases: []
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# Pivot e Matrice a Scala

Consideriamo una matrice $U \in M_{\mathbb{K}}(m,n)$ e siano $U_1, U_2, \dots, U_m$ le sue righe ($U_i \in M_{\mathbb{K}}(1,n)$).

- Il **pivot** della riga $U_i$ è il primo elemento non nullo sulla $i$-esima riga.
- La matrice $U$ si dice **a scala** se:
  - date due righe consecutive non nulle $U_i, U_{i+1}$, il pivot di $U_i$ si trova su una colonna che precede la colonna contenente il pivot di $U_{i+1}$;
  - se $U_i$ è una riga nulla, allora sono nulle tutte le righe seguenti.

![[2026-10-07-matrice-a-scala-pivot.png]]

> **N.B.** L'output del MEG è una matrice a scala.

---
Precedente: [[Metodo di Eliminazione di Gauss]] · Successivo: [[Reversibilità del MEG]]
