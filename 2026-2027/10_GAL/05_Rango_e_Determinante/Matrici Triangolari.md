---
created: 2026-10-07
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/rango_e_determinante
aliases: []
origine: UpdateVault
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Matrici Triangolari

> [!example] Esempio (II)
> (vedi l'obiettivo e l'esempio (I) in [[Determinante e Sviluppo di Laplace]])

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
> $\{\text{matrici diagonali}\} \subseteq \{\text{matrici triang. sup.}\}$ e $\{\text{matrici diagonali}\} \subseteq \{\text{matrici triang. inf.}\}$ (matrici diagonali: [[Matrice Identità e Matrici Diagonali]]).

> [!abstract] Teorema (Determinante di una matrice triangolare superiore)
> Sia $T$ triangolare superiore, sviluppo lungo la colonna $j = 1$:
> $$\det(T) \overset{j=1}{=} \sum_{i=1}^{n} (-1)^{i+1}\, t_{i1} \det(\hat{T}_{i1}) = (-1)^{1+1} t_{11} \det(\hat{T}_{11}) + 0 + 0 + \cdots + 0$$
> $$= t_{11} \det\left(\begin{bmatrix} t_{22} & t_{23} & \cdots & t_{2n} \\ 0 & t_{33} & \cdots & \\ \vdots & & \ddots & \\ 0 & \cdots & 0 & t_{nn} \end{bmatrix}\right) = \cdots$$
> (la sottomatrice è ancora triangolare superiore)
> $$= t_{11}\, t_{22} \cdots t_{nn}$$

**DISEGNO NON RAPPRESENTABILE** (disegno — L6, p. 11/slide 55: sottomatrice $\hat{T}_{11}$ con riquadro blu sulla prima colonna $(t_{22}, 0, \dots, 0)^T$ e freccia rossa con la scritta «triangolare superiore») *(dove cercarlo: GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 54-55))*

> [!note] Osservazione
> **Recap degli obiettivi:**
> - (I) calcolare le matrici inverse → [[Esistenza della Matrice Inversa]]
> - (II) calcolare il rango → [[MEG e Rango]]
> - (III) calcolare il determinante usando le matrici triangolari → [[Calcolo del Determinante con il MEG]]

---
Precedente: [[Determinante e Sviluppo di Laplace]] · Successivo: [[Teorema di Binet]]
