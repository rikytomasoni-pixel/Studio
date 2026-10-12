---
tags: [GAL, matrici, pivot, matrice-a-scala, MEG, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 60-61)"
---

# Pivot e matrice a scala

> [!warning] Def. 6.6 Pivot e matrice a scala
> Consideriamo una matrice $U \in M_{\mathbb{K}}(m,n)$ e siano $U_1, U_2, \dots, U_m$ le sue righe ($U_i \in M_{\mathbb{K}}(1,n)$):
> $$U = \begin{bmatrix} U_1 \\ U_2 \\ \vdots \\ U_m \end{bmatrix}$$
> - Il **pivot** della riga $U_i$ è il primo elemento non nullo sulla $i$-esima riga.
> - La matrice $U$ si dice **a scala** se
>   - date due righe consecutive non nulle $U_i, U_{i+1}$ il pivot di $U_i$ si trova su una colonna che precede la colonna contenente il pivot di $U_{i+1}$;
>   - se $U_i$ è una riga nulla, allora sono nulle tutte le righe seguenti.

$$U = \begin{bmatrix} 0 & \cdots & 0 & p_1 & \ast & \cdots & \cdots & \ast \\ 0 & \cdots & \cdots & 0 & 0 & p_2 & \ast & \ast \\ & & & & & & \ddots & \\ & & & & & & p_r & \ast \\ 0 & \cdots & \cdots & \cdots & 0 & \cdots & \cdots & 0 \\ \vdots & & & & & & & \vdots \\ 0 & \cdots & \cdots & \cdots & 0 & \cdots & \cdots & 0 \end{bmatrix}$$

![[ScalaPivotMEG.png]]

> [!note] Osservazione
> N.B. l'output del MEG ([[68_Metodo_di_Eliminazione_di_Gauss]]) è una matrice a scala.

## Note collegate
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[73_MEG_e_Rango]]
- [[66_Matrici_Triangolari]]
- [[63_Rango_di_una_Matrice]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]
