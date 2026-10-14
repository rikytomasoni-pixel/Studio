---
created: 2026-09-17
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/2
  - argomento/vettori_geometrici
aliases: []
origine: UpdateVault
---
[[00_GAL_Vettori_Geometrici|⬅️ Torna a Vettori Geometrici]]

# Prodotto Interno in Coordinate

> [!abstract] Teorema (Proposizione — Prodotto interno in coordinate)
> Fissato un riferimento cartesiano ([[Sistemi di Riferimento e Coordinate]]), se
> $$u = \begin{pmatrix} x_1 \\ x_2 \\ x_3 \end{pmatrix}, \qquad v = \begin{pmatrix} y_1 \\ y_2 \\ y_3 \end{pmatrix},$$
> allora
> $$u \cdot v = x_1 y_1 + x_2 y_2 + x_3 y_3.$$

**dim:** Se $u$ ha coordinate $(x_1, x_2, x_3)^T$ [nell'originale: $(x_1,x_3,x_3)^T$, svista evidente] allora $u = x_1 e_1 + x_2 e_2 + x_3 e_3$ e allo stesso modo $v = y_1 e_1 + y_2 e_2 + y_3 e_3$. Allora
$$
\begin{aligned}
u \cdot v &= \Big(\sum_{i=1}^{3} x_i e_i\Big) \cdot \Big(\sum_{j=1}^{3} y_j e_j\Big) \\
&= \sum_{i,j=1}^{3} (x_i e_i) \cdot (y_j e_j) \\
&= \sum_{i,j=1}^{3} x_i y_j \,(e_i \cdot e_j) \qquad (e_i \cdot e_j = 0 \text{ se } i \neq j) \\
&= \sum_{i=1}^{3} x_i y_i \,(e_i \cdot e_i) \qquad (e_i \cdot e_i = 1) \\
&= \sum_{i=1}^{3} x_i y_i. \qquad \blacksquare
\end{aligned}
$$

**DISEGNO NON RAPPRESENTABILE** (disegno: parallelepipedo con $O$ origine, versori $e_1, e_2, e_3$ e componenti $x_1, x_2, x_3$ del vettore $u$) *(dove cercarlo: GAL_2026-2027_-_20260917_-_LEZIONE_2.pdf (p. 5-6))*

---
Precedente: [[Prodotto Interno e Ortogonalità]] · Successivo: [[Prodotto Esterno e Determinanti]]
