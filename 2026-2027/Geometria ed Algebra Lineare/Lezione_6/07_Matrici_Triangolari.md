---
tags: [GAL, matrici, triangolari, determinante, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 54-55)"
---

# Matrici triangolari e loro determinante

> [!example] Esempio (II)
> (vedi l'obiettivo e l'esempio (I) in [[06_Determinante_Sviluppo_di_Laplace]])

> [!warning] Def. 6.5 Matrici triangolari
> Una matrice $T \in M_{\mathbb{K}}(n,n)$ si dice
> - **triangolare superiore** se $t_{ij} = 0\ \ \forall\, i > j$
> - **triangolare inferiore** se $t_{ij} = 0\ \ \forall\, i < j$
>
> Triangolare superiore:
> $$\begin{bmatrix} t_{11} & \ast & \cdots & \ast \\ 0 & t_{22} & & \vdots \\ \vdots & & \ddots & \ast \\ 0 & \cdots & 0 & t_{nn} \end{bmatrix}$$
> Triangolare inferiore:
> $$\begin{bmatrix} t_{11} & 0 & \cdots & 0 \\ \ast & \ddots & & \vdots \\ \vdots & & \ddots & 0 \\ \ast & \cdots & \ast & t_{nn} \end{bmatrix}$$

> [!note] Osservazione
> $\{\text{matrici diagonali}\} \subseteq \{\text{matrici triang. sup.}\}$ e $\{\text{matrici diagonali}\} \subseteq \{\text{matrici triang. inf.}\}$ (matrici diagonali: [[06_Matrice_Identita_e_Matrici_Diagonali]]).

> [!abstract] Teorema (Determinante di una matrice triangolare superiore)
> Sia $T$ triangolare superiore (con la prima colonna $(t_{11}, 0, \dots, 0)^T$ evidenziata in blu):
> $$T = \begin{bmatrix} t_{11} & t_{12} & \cdots & t_{1n} \\ 0 & t_{22} & \cdots & t_{2n} \\ \vdots & 0 & \ddots & \vdots \\ 0 & 0 & \cdots & t_{nn} \end{bmatrix}$$
> Sviluppo lungo la colonna $j = 1$:
> $$\det(T) \overset{j=1}{=} \sum_{i=1}^{n} (-1)^{i+1}\, t_{i1} \det(\hat{T}_{i1}) = (-1)^{1+1} t_{11} \det(\hat{T}_{11}) + 0 + 0 + \cdots + 0$$
> $$= t_{11} \det\left(\begin{bmatrix} t_{22} & t_{23} & \cdots & t_{2n} \\ 0 & t_{33} & \cdots & \\ \vdots & & \ddots & \\ 0 & \cdots & 0 & t_{nn} \end{bmatrix}\right) = \cdots$$
> (la sottomatrice è ancora triangolare superiore)
> $$= t_{11}\, t_{22} \cdots t_{nn}$$

**!!!** (disegno — L6, p. 11/slide 55: sottomatrice $\hat{T}_{11}$ con riquadro blu sulla prima colonna $(t_{22}, 0, \dots, 0)^T$ e freccia rossa con la scritta «triangolare superiore»)

> [!note] Osservazione
> **Recap degli obiettivi:**
> - (I) calcolare le matrici inverse → [[03_Esistenza_della_Matrice_Inversa]]
> - (II) calcolare il rango → [[04_MEG_e_Rango]]
> - (III) calcolare il determinante usando le matrici triangolari → [[06_Calcolo_del_Determinante_con_il_MEG]]

## Note collegate
- [[06_Determinante_Sviluppo_di_Laplace]]
- [[06_Matrice_Identita_e_Matrici_Diagonali]]
- [[09_Metodo_di_Eliminazione_di_Gauss]]
- [[06_Calcolo_del_Determinante_con_il_MEG]]
- Indice: [[00_Indice_Lezione_6]] · [[00_MOC_GAL]]
