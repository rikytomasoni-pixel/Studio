---
created: 2026-10-12
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/sistemi_lineari
aliases: []
---
[[00_GAL_Sistemi_Lineari|⬅️ Torna a Sistemi Lineari]]

# Dimostrazione di Rouché-Capelli

$A\underline{x} = \underline{b}$ risolubile $\iff r(A) = r([A \mid \underline{b}])$ è equivalente a dimostrare 2 casi:

- $A\underline{x} = \underline{b}$ risolubile $\Rightarrow r(A) = r([A\mid\underline{b}])$; equivalentemente (contronominale) $r(A) \neq r([A\mid\underline{b}]) \Rightarrow A\underline{x} = \underline{b}$ **non** risolubile;
- $r(A) = r([A\mid\underline{b}]) \Rightarrow A\underline{x} = \underline{b}$ risolubile.

Comincio a usare il MEG sulla rappresentazione matriciale del III tipo:

$$
[A \mid \underline{b}] \overset{\text{MEG}}{\leadsto} [U \mid \underline{b}']
$$

Per definizione di rango: $r = r(A) = r(U) = \#\text{pivot di } U$. Considerando l'ultima colonna ci sono 2 possibilità:

1. **$r(A) = r([A\mid\underline{b}])$**: $[U\mid\underline{b}']$ ha i pivot $p_1,\dots,p_r$ tutti nelle colonne di $U$, e le righe dalla $(r+1)$-esima in poi sono completamente nulle (anche nei termini noti).
2. **$r([A\mid\underline{b}]) = r(A) + 1$** (cioè $r(A) \neq r([A\mid\underline{b}])$): esiste un pivot $b'_{r+1} \neq 0$ nella colonna dei termini noti.

> **Figura (disegno senza immagine disponibile):**
>
> Due matrici a scala $[U \mid \underline{b}']$ con linea rossa a gradini. Caso (1): pivot $p_1,\dots,p_r$ nella parte $U$, la linea a gradini termina prima della colonna dei termini noti; righe nulle in fondo anche nella colonna $b'$. Caso (2): oltre ai pivot $p_1,\dots,p_r$ compare un ulteriore pivot $b'_{r+1} \neq 0$ nella colonna dei termini noti, sotto $p_r$.

**Nel caso (2)**, l'equazione sulla riga $r+1$ dice $0 = b'_{r+1} \neq 0$ $\Rightarrow$ $A\underline{x} = \underline{b}$ **non risolubile**.

**Adesso mi occupo del caso (1)** e cerco le soluzioni. Le righe nulle in fondo (barrate in viola) si eliminano. Divido le variabili in due gruppi:

- **variabili dipendenti**: corrispondono alle colonne contenenti i pivot ($r$ variabili);
- **variabili indipendenti**: corrispondono alle colonne non contenenti i pivot ($n - r$ variabili).

Suppongo, per semplicità, che le variabili dipendenti siano le prime $r$ variabili.

> **Figura (disegno senza immagine disponibile):**
>
> Matrice $[U\mid b']$ con $r$ equazioni; sotto, la ripartizione delle colonne: le prime $r$ colonne ($r$ variabili dipendenti, contenenti i pivot $p_1,\dots,p_r$ a scala), le successive $n-r$ colonne (variabili indipendenti, con asterischi) e infine la colonna dei termini noti. Sotto la linea orizzontale sono aggiunte $n-r$ equazioni fittizie la cui parte di coefficienti è una matrice identità sulle variabili indipendenti, con termini noti $t_1,\dots,t_{n-r}$.

Aggiungo $n - r$ equazioni (fittizie):

$$
x_{r+1} = t_1,\ \dots,\ x_n = t_{n-r}, \qquad t_i \in \mathbb{K}
$$

Il sistema diventa un sistema con $n$ equazioni e $n$ incognite, che risolvo per **sostituzione all'indietro**:

- **Step 1**: il termine noto delle prime $r$ equazioni diventa $b'_j + \sum c_i t_i$ (le variabili indipendenti portate a destra);
- **Step 2**: sostituisco a ritroso anche tra le prime $r$ equazioni.

**Dove arrivo?** Si ottiene una forma in cui la parte dei coefficienti è l'identità $n\times n$, con termini noti

$$
x_j = v_{0j} + \sum_{i=1}^{n-r} v_{ij}\,t_i \quad (j = 1,\dots,r), \qquad x_{r+i} = t_i \quad (i = 1,\dots,n-r)
$$

Dunque

$$
\begin{bmatrix} x_1 \\ \vdots \\ x_n \end{bmatrix}
= \underbrace{\begin{bmatrix} v_{01} \\ \vdots \\ v_{0r} \\ 0 \\ \vdots \\ 0 \end{bmatrix}}_{\underline{v}_0\ (\text{parte costante})}
+ t_1\underbrace{\begin{bmatrix} v_{11} \\ \vdots \\ v_{1r} \\ 1 \\ 0 \\ \vdots \\ 0 \end{bmatrix}}_{\underline{v}_1}
+ t_2\underbrace{\begin{bmatrix} v_{21} \\ \vdots \\ v_{2r} \\ 0 \\ 1 \\ \vdots \\ 0 \end{bmatrix}}_{\underline{v}_2}
+ \cdots
+ t_{n-r}\underbrace{\begin{bmatrix} v_{n-r,1} \\ \vdots \\ v_{n-r,r} \\ 0 \\ \vdots \\ 1 \end{bmatrix}}_{\underline{v}_{n-r}}
$$

che è l'espressione cercata. $\blacksquare$

---
Precedente: [[Teorema di Rouché-Capelli]]
