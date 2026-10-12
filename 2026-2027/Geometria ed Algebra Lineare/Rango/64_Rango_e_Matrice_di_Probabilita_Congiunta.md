---
tags: [GAL, matrici, rango, probabilita, indipendenza, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 49-50)"
---

# Rango e matrice di probabilità congiunta

> [!example] Esempio
> Matrice di probabilità congiunta di moneta e dado ([[30_Matrici_come_Rappresentazione_di_Funzioni]]), righe $T, C$, colonne $1, \dots, 6$:
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

Definizione di rango: [[63_Rango_di_una_Matrice]].

## Note collegate
- [[63_Rango_di_una_Matrice]]
- [[30_Matrici_come_Rappresentazione_di_Funzioni]]
- [[73_MEG_e_Rango]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]
