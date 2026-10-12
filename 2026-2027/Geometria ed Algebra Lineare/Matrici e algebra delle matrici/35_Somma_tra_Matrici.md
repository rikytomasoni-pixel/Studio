---
tags: [GAL, matrici, somma, proprieta, lezione-3]
data: 2026-09-30
lezione: 3
fonte: "GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 30-31)"
---

# Somma tra matrici

«Se voglio sommare due funzioni, queste devono avere lo stesso dominio»
$f(x) = \dfrac{1}{x^2 - 1}$, $\quad g(x) = e^x$, $\quad (f+g)(1)\ ??$

> [!warning] Def. Somma di matrici
> $$+ : M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(m,n) \to M_{\mathbb{K}}(m,n),\qquad (A,B) \mapsto A + B$$
> $A = [a_{ij}]$, $B = [b_{ij}]$, $\quad A + B = [a_{ij} + b_{ij}]$
> «somma posizione per posizione», «somma puntuale».

> [!example] Esempio
> $$\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} -1 & 1 \\ 4 & 7 \end{bmatrix} = \begin{bmatrix} 1+(-1) & -2+1 \\ 0+4 & 3+7 \end{bmatrix} = \begin{bmatrix} 0 & -1 \\ 4 & 10 \end{bmatrix}$$

**!!!** (colorazione: le quattro posizioni $(1,1)$, $(1,2)$, $(2,1)$, $(2,2)$ evidenziate con colori diversi in $A$, $B$ e $A+B$)

> [!abstract] Teorema (Proprietà)
> «ereditiamo le proprietà della somma del campo» ([[24_Proprieta_delle_Operazioni_tra_Vettori]] per l'analogo sui vettori)
> - **Proprietà associativa** $\forall A,B,C \in M_{\mathbb{K}}(m,n)$: $(A+B)+C = A+(B+C) = A+B+C$
> - **Proprietà commutativa** $\forall A,B \in M_{\mathbb{K}}(m,n)$: $A + B = B + A$
> - **Esistenza elemento neutro:** $\exists\, N \in M_{\mathbb{K}}(m,n)$ tale che $\forall A \in M_{\mathbb{K}}(m,n)$: $A + N = N + A = A$
> - **Esistenza dell'elemento opposto:** $\forall A \in M_{\mathbb{K}}(m,n)\ \exists\, A' \in M_{\mathbb{K}}(m,n)$ tale che $A + A' = A' + A = \begin{bmatrix} 0 & \cdots & 0 \\ \vdots & & \vdots \\ 0 & \cdots & 0 \end{bmatrix}$

> [!note] Osservazione (Domanda)
> D. chi è $N$?
> R. $\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix} = \begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix}$, quindi $N = \begin{bmatrix} 0 & \cdots & 0 \\ \vdots & & \vdots \\ 0 & \cdots & 0 \end{bmatrix}$.

> [!note] Osservazione (Domanda)
> D. chi è $A'$?
> R. $\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} -1 & 2 \\ 0 & -3 \end{bmatrix} = \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$; in generale $A = [a_{ij}]$, $A' = [-a_{ij}]$. Notazione definitiva in [[40_Opposto_di_una_Matrice]].

## Note collegate
- [[34_Confronto_e_Uguaglianza_tra_Matrici]]
- [[36_Prodotto_di_una_Matrice_per_uno_Scalare]]
- [[40_Opposto_di_una_Matrice]]
- [[24_Proprieta_delle_Operazioni_tra_Vettori]]
- [[37_Efficienza_Computazionale]]
- Indice: [[04_Indice_Lezione_3]] · [[00_MOC_GAL]]
