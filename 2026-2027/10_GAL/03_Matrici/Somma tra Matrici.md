---
created: 2026-09-30
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Somma tra Matrici

«Se voglio sommare due funzioni, queste devono avere lo stesso dominio.» Ad esempio per $f(x) = \frac{1}{x^2-1}$ e $g(x) = e^x$ il valore $(f+g)(1)$ non è definito.

### Definizione

$$
+ : M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(m,n) \to M_{\mathbb{K}}(m,n), \qquad (A,B) \longmapsto A+B
$$

Con $A = [a_{ij}]$ e $B = [b_{ij}]$:

$$
A + B = [a_{ij} + b_{ij}]
$$

(«somma posizione per posizione», «somma puntuale»).

**Esempio**

$$
\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} -1 & 1 \\ 4 & 7 \end{bmatrix}
= \begin{bmatrix} 1+(-1) & -2+1 \\ 0+4 & 3+7 \end{bmatrix}
= \begin{bmatrix} 0 & -1 \\ 4 & 10 \end{bmatrix}
$$

### Proprietà della somma

«Ereditiamo le proprietà della somma del campo.» $\forall A,B,C \in M_{\mathbb{K}}(m,n)$:

- **Proprietà associativa**: $(A+B)+C = A+(B+C) = A+B+C$.
- **Proprietà commutativa**: $A+B = B+A$.
- **Esistenza dell'elemento neutro**: $\exists N \in M_{\mathbb{K}}(m,n)$ tale che $\forall A \in M_{\mathbb{K}}(m,n)$, $A+N = N+A = A$. *Chi è $N$?* La **matrice nulla**:

  $$N = \begin{bmatrix} 0 & \cdots & 0 \\ \vdots & & \vdots \\ 0 & \cdots & 0 \end{bmatrix}$$

  Ad esempio $\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix} = \begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix}$.
- **Esistenza dell'elemento opposto**: $\forall A \in M_{\mathbb{K}}(m,n)$ $\exists A' \in M_{\mathbb{K}}(m,n)$ tale che $A + A' = A' + A = $ matrice nulla. *Chi è $A'$?* Se $A = [a_{ij}]$, allora $A' = [-a_{ij}]$. Esempio: $\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} -1 & 2 \\ 0 & -3 \end{bmatrix} = \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$.

---
Precedente: [[Uguaglianza tra Matrici]] · Successivo: [[Prodotto di una Matrice per uno Scalare]]
