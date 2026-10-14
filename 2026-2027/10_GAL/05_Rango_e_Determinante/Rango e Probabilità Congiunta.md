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

# Rango e Probabilità Congiunta

> [!example] Esempio
> Matrice di probabilità congiunta di moneta e dado ([[Matrici come Rappresentazione di Funzioni]]), righe $T, C$, colonne $1, \dots, 6$:
> $$\begin{bmatrix} \frac{1}{12} & \frac{1}{12} & \frac{1}{12} & \frac{1}{12} & \frac{1}{12} & \frac{1}{12} \\ \frac{1}{12} & \frac{1}{12} & \frac{1}{12} & \frac{1}{12} & \frac{1}{12} & \frac{1}{12} \end{bmatrix}$$
> $r \leq \min(2,6)$, quindi $r \leq 2$ ($r > 0$).
>
> D. possiamo trovare una decomposizione con 1 addendo?
> $$\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} \frac12 \\ \frac12 \end{bmatrix} \begin{bmatrix} \frac16 & \frac16 & \frac16 & \frac16 & \frac16 & \frac16 \end{bmatrix} \qquad \boxed{r = 1}$$
> Altre scritture equivalenti: $= \begin{bmatrix} 1 \\ 1 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} \frac{1}{12} \\ \frac{1}{12} \end{bmatrix} \begin{bmatrix} 1 & \cdots & 1 \end{bmatrix}$
>
> $$\begin{bmatrix} \frac12 \\ \frac12 \end{bmatrix} = \begin{bmatrix} P(T) \\ P(C) \end{bmatrix}, \qquad \begin{bmatrix} \frac16 & \cdots & \frac16 \end{bmatrix} = \begin{bmatrix} P(1) & P(2) & \cdots & P(6) \end{bmatrix}$$

> [!warning] Def. (Indipendenza e rango)
> $r(\text{matrice di probabilità congiunta}) = 1 \iff$ i due eventi sono indipendenti.

> [!example] Esempio per casa
> 2 dadi (sei facce equo)
> $A = \{\text{esito } D_1 \text{ pari},\ \text{esito } D_1 \text{ dispari}\}$
> $B = \{\text{esito } D_1+D_2 \text{ pari},\ \text{esito } D_1+D_2 \text{ dispari}\}$
> $P : A \times B \to [0,1]$
> Tabella (da completare): righe «$D_1$ pari», «$D_1$ dispari»; colonne «$D_1+D_2$ pari», «$D_1+D_2$ dispari».

Definizione di rango: [[Rango di una Matrice]].

---
Precedente: [[Rango di una Matrice]] · Successivo: [[Determinante e Sviluppo di Laplace]]
