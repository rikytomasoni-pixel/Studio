---
created: 2026-10-08
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/eliminazione_di_gauss
aliases: []
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# MEG e Rango

> «Il rango vuole essere una misura di complessità (quanta informazione c'è) di una matrice.» «Il MEG concentra l'informazione nella parte alta e a destra della matrice.»

**Esempio.** Matrice $2\times 6$ con tutte le entrate $\frac{1}{12}$ (pivot $p_1 = \frac1{12}$). Applico il MEG: $\mathrm{II} - \frac{1/12}{1/12}\mathrm{I} \to \mathrm{II}$ (moltiplicatore $1$):

$$
\begin{bmatrix} 1 & 0 \\ -1 & 1 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix} = \begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ 0 & \cdots & 0 \end{bmatrix}
$$

Invertendo il passo ($+1$):

$$
\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}
$$

e la matrice $U$ ottenuta si scrive come

$$
\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix} \qquad (\text{rango } 1)
$$

Quindi

$$
\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix}\left(\begin{bmatrix} 1 \\ 0 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}\right) = \left(\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix}\begin{bmatrix} 1 \\ 0 \end{bmatrix}\right)\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}
$$

$$
\Rightarrow\quad r\left(\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}\right) = 1
$$

### Proposizione

Data $A \in M_{\mathbb{K}}(m,n)$, sia $U$ una matrice a scala ottenuta con il MEG a partire da $A$. Allora:

- $r(U) = $ numero di righe non nulle di $U$ $=$ numero di pivot di $U$;
- $r(A) = r(U)$.

> **Il MEG è il modo EFFICIENTE per calcolare il rango di una matrice!!**

**Esempio — calcolo del rango.**

$$
\begin{bmatrix} 1 & 0 & -1 & 2 \\ 2 & 0 & 3 & 1 \\ 1 & 0 & 4 & -1 \end{bmatrix}
\xrightarrow[\ \mathrm{III}-\mathrm{I}\to\mathrm{III}\ ]{\ \mathrm{II}-2\mathrm{I}\to\mathrm{II}\ }
\begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 5 & -3 \end{bmatrix}
\xrightarrow{\ \mathrm{III}-\mathrm{II}\to\mathrm{III}\ }
\begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 0 & 0 \end{bmatrix}
\Rightarrow r = 2
$$

(pivot: $1$ e $5$).

![[2026-10-08-calcolo-rango-con-MEG.png]]

---
Precedente: [[Esistenza della Matrice Inversa]]
