---
created: 2026-10-08
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/rango_e_determinante
aliases: []
origine: UpdateVault
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Calcolo del Determinante con il MEG

> [!note] Osservazione
> $A \in M_{\mathbb{K}}(n,n) \overset{\text{MEG}}{\leadsto} U \in M_{\mathbb{K}}(n,n)$ a scala ([[Metodo di Eliminazione di Gauss]]); $U$ è triangolare superiore ([[Matrici Triangolari]]).
> $$A = ZU = Z \begin{bmatrix} u_{11} & \cdots & u_{1n} \\ 0 & u_{22} & & \ast \\ \vdots & & \ddots & \\ 0 & \cdots & 0 & u_{nn} \end{bmatrix}$$
> $$\det(A) = \det(Z)\det(U) = \det(Z)\, u_{11}u_{22}\cdots u_{nn}$$
> (primo passaggio per il [[Teorema di Binet]]; $Z$ come in [[Esistenza della Matrice Inversa]])

$$\det(A) = 1 \cdot 1 \cdot \big((0 \cdot (-7)) - ((-5) \cdot (-5))\big) = 1 \cdot (0 - 25) = -25$$

---
Precedente: [[Teorema di Binet]] · Successivo: [[Proprietà del Determinante]]
