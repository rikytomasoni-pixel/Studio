---
created: 2026-10-07
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/rango_e_determinante
aliases: []
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Rango e Probabilità Congiunta

**Matrice di probabilità congiunta moneta-dado** (con $M \times D$ come nella [[2026-09-30 GAL Lezione 3|Lezione 3]]): la matrice $2 \times 6$ con tutte le entrate $\frac{1}{12}$ ha $r \le \min(2,6) = 2$, e $r > 0$. **Domanda**: possiamo trovare una decomposizione con 1 addendo? Sì:

$$
\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}
= \begin{bmatrix} \tfrac12 \\ \tfrac12 \end{bmatrix}\begin{bmatrix} \tfrac16 & \tfrac16 & \tfrac16 & \tfrac16 & \tfrac16 & \tfrac16 \end{bmatrix}
\quad\Longrightarrow\quad r = 1
$$

Qui $\begin{bmatrix} \frac12 \\ \frac12 \end{bmatrix} = \begin{bmatrix} \mathbb{P}(T) \\ \mathbb{P}(C) \end{bmatrix}$ e $\begin{bmatrix} \frac16 & \cdots & \frac16 \end{bmatrix} = \begin{bmatrix} \mathbb{P}(1) & \mathbb{P}(2) & \cdots & \mathbb{P}(6) \end{bmatrix}$.

### Definizione

$$
r(\text{matrice di probabilità congiunta}) = 1 \iff \text{i due eventi sono indipendenti}
$$

**Esempio per casa**: 2 dadi (sei facce equi). $A = \{\text{esito } D_1 \text{ pari},\ \text{esito } D_1 \text{ dispari}\}$, $B = \{\text{esito } D_1 + D_2 \text{ pari},\ \text{esito } D_1 + D_2 \text{ dispari}\}$, $\mathbb{P} : A \times B \to [0,1]$; da completare la tabella:

| $\mathbb{P}$ | $D_1+D_2$ pari | $D_1+D_2$ dispari |
|---|---|---|
| **$D_1$ pari** | | |
| **$D_1$ dispari** | | |

---
Precedente: [[Rango di una Matrice]] · Successivo: [[Determinante e Sviluppo di Laplace]]
