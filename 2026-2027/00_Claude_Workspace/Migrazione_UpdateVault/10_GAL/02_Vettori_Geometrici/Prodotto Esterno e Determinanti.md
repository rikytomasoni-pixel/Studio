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

# Prodotto Esterno e Determinanti

> [!warning] Def. Prodotto esterno
> Dati due vettori $u, v$ il loro **prodotto esterno** è il vettore $u \wedge v$ definito in questo modo:
> - se $u$ e $v$ sono multipli uno dell'altro allora $u \wedge v = 0$;
> - se $u, v$ non sono collineari allora $\|u \wedge v\| = \|u\| \cdot \|v\| \cdot \sin\vartheta$
>
> e $u \wedge v$ si trova sulla semiretta uscente da $O$ ortogonale al piano $H$ che contiene $O$, $P$ e $Q$ che vede la rotazione di $u$ verso $v$ lungo $\vartheta$ in senso antiorario.

**DISEGNO NON RAPPRESENTABILE** (disegno: piano $H$ contenente $O$, $P$, $Q$ con $u = OP$, $v = OQ$, angolo $\vartheta$, freccia di rotazione antioraria da $u$ verso $v$, e retta ortogonale al piano per $O$ con la semiretta $OS$) *(dove cercarlo: GAL_2026-2027_-_20260917_-_LEZIONE_2.pdf (p. 6))*

Il prodotto esterno si calcola in coordinate con i determinanti: [[Prodotto Esterno e Determinanti]].

## Determinanti 2×2 e 3×3

> [!warning] Def. Determinanti 2×2 e 3×3
> $$\begin{vmatrix} x_1 & x_2 \\ y_1 & y_2 \end{vmatrix} = x_1 y_2 - x_2 y_1$$
> $$\begin{vmatrix} x_1 & x_2 & x_3 \\ y_1 & y_2 & y_3 \\ z_1 & z_2 & z_3 \end{vmatrix} = x_1 \begin{vmatrix} y_2 & y_3 \\ z_2 & z_3 \end{vmatrix} - x_2 \begin{vmatrix} y_1 & y_3 \\ z_1 & z_3 \end{vmatrix} + x_3 \begin{vmatrix} y_1 & y_2 \\ z_1 & z_2 \end{vmatrix}$$

---
Precedente: [[Prodotto Interno in Coordinate]]
