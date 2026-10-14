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

# Prodotto Esterno e Determinanti

> **Definizione (prodotto esterno).** Dati $u,v$, il **prodotto esterno** è il vettore $u\wedge v$ tale che:
> - se $u,v$ sono multipli uno dell'altro, $u\wedge v=0$;
> - se non sono collineari, $\|u\wedge v\|=\|u\|\,\|v\|\sin\vartheta$ e $u\wedge v$ giace sulla semiretta uscente da $O$ ortogonale al piano $H$ contenente $O,P,Q$ (con $u=OP$, $v=OQ$), orientata in modo che la rotazione di $u$ verso $v$ lungo $\vartheta$ risulti antioraria.

> Disegno: piano $H$ con $O,P,Q$, angolo $\vartheta$, freccia di rotazione antioraria da $u$ verso $v$ e retta ortogonale al piano con la semiretta $OS$.

Il prodotto esterno si calcola in coordinate con i **determinanti**:

$$
\begin{vmatrix}x_1&x_2\\y_1&y_2\end{vmatrix}=x_1y_2-x_2y_1,
\qquad
\begin{vmatrix}x_1&x_2&x_3\\y_1&y_2&y_3\\z_1&z_2&z_3\end{vmatrix}
= x_1\begin{vmatrix}y_2&y_3\\z_2&z_3\end{vmatrix}
- x_2\begin{vmatrix}y_1&y_3\\z_1&z_3\end{vmatrix}
+ x_3\begin{vmatrix}y_1&y_2\\z_1&z_2\end{vmatrix}.
$$

Il determinante tornerà in forma generale con lo [[2026-10-07 GAL Lezione 6|sviluppo di Laplace]].

---
Precedente: [[Prodotto Interno in Coordinate]]
