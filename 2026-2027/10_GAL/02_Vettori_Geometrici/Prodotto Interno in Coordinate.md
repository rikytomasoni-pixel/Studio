---
created: 2026-09-17
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/2
  - argomento/vettori_geometrici
aliases: []
---
[[00_GAL_Vettori_Geometrici|⬅️ Torna a Vettori Geometrici]]

# Prodotto Interno in Coordinate

> **Proposizione.** Fissato un riferimento cartesiano, se $u=(x_1,x_2,x_3)^T$ e $v=(y_1,y_2,y_3)^T$ allora
> $$u\cdot v=x_1y_1+x_2y_2+x_3y_3.$$

**Dimostrazione.** Si ha $u=x_1e_1+x_2e_2+x_3e_3$ e $v=y_1e_1+y_2e_2+y_3e_3$, con $e_i\cdot e_j=0$ per $i\ne j$ ed $e_i\cdot e_i=1$. Allora
$$
\begin{aligned}
u\cdot v &= \Big(\sum_{i=1}^{3}x_ie_i\Big)\cdot\Big(\sum_{j=1}^{3}y_je_j\Big)
= \sum_{i,j=1}^{3}x_iy_j\,(e_i\cdot e_j)
= \sum_{i=1}^{3}x_iy_i\,(e_i\cdot e_i)
= \sum_{i=1}^{3}x_iy_i. \qquad\blacksquare
\end{aligned}
$$
(Nell'originale $u=(x_1,x_3,x_3)^T$: svista evidente, corretta.)

> Disegno: parallelepipedo con origine $O$, versori $e_1,e_2,e_3$ e componenti $x_1,x_2,x_3$ del vettore $u$.

---
Precedente: [[Prodotto Interno e Ortogonalità]] · Successivo: [[Prodotto Esterno e Determinanti]]
