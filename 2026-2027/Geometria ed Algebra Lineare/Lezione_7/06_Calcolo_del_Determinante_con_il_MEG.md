---
tags: [GAL, matrici, determinante, MEG, triangolari, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 69)"
---

# Calcolo del determinante con il MEG

> [!note] Osservazione
> $A \in M_{\mathbb{K}}(n,n) \overset{\text{MEG}}{\leadsto} U \in M_{\mathbb{K}}(n,n)$ a scala ([[09_Metodo_di_Eliminazione_di_Gauss]]); $U$ è triangolare superiore ([[07_Matrici_Triangolari]]).
> $$A = ZU = Z \begin{bmatrix} u_{11} & \cdots & u_{1n} \\ 0 & u_{22} & & \ast \\ \vdots & & \ddots & \\ 0 & \cdots & 0 & u_{nn} \end{bmatrix}$$
> $$\det(A) = \det(Z)\det(U) = \det(Z)\, u_{11}u_{22}\cdots u_{nn}$$
> (primo passaggio per il [[05_Teorema_di_Binet]]; $Z$ come in [[03_Esistenza_della_Matrice_Inversa]])

$$\det(A) = 1 \cdot 1 \cdot \big((0 \cdot (-7)) - ((-5) \cdot (-5))\big) = 1 \cdot (0 - 25) = -25$$
## Note collegate
- [[05_Teorema_di_Binet]]
- [[07_Matrici_Triangolari]]
- [[03_Esistenza_della_Matrice_Inversa]]
- [[09_Metodo_di_Eliminazione_di_Gauss]]
- [[06_Determinante_Sviluppo_di_Laplace]]
- Indice: [[00_Indice_Lezione_7]] · [[00_MOC_GAL]]
