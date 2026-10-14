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

# Rappresentazioni Matriciali di un Sistema

Temi: **formalizzazione** e **risoluzione** (teorica/pratica).

**Esempio.**

$$
\begin{cases} x - 3y = 2 \\ 4x + 5y = 1 \end{cases}
\qquad \text{(2 incognite } x,y \text{; 2 equazioni)}
$$

Il sistema equivale a un'uguaglianza tra matrici:

$$
\begin{bmatrix} x - 3y \\ 4x + 5y \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

**(I) Uso la somma tra matrici e il prodotto per scalari** — *rappresentazione matriciale del I tipo*:

$$
\begin{bmatrix} x - 3y \\ 4x + 5y \end{bmatrix} = \begin{bmatrix} x \\ 4x \end{bmatrix} + \begin{bmatrix} -3y \\ 5y \end{bmatrix} = x\begin{bmatrix} 1 \\ 4 \end{bmatrix} + y\begin{bmatrix} -3 \\ 5 \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

Un sistema con 2 equazioni e 2 incognite è equivalente a **1 equazione** che coinvolge vettori colonna di altezza 2.

**(II) Uso il prodotto matriciale** — *rappresentazione matriciale del II tipo*:

$$
\begin{bmatrix} x - 3y \\ 4x + 5y \end{bmatrix} = \begin{bmatrix} 1 & -3 \\ 4 & 5 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
$$

> **Oss. 1**: la matrice dei coefficienti (nel II tipo) è la giustapposizione dei vettori colonna dei coefficienti (I tipo).
>
> **Oss. 2**: il nome di $x$ e $y$ è marginale: il sistema $\begin{cases} x - 3y = 2 \\ 4x + 5y = 1 \end{cases}$ e il sistema $\begin{cases} A - 3B = 2 \\ 4A + 5B = 1 \end{cases}$ hanno la stessa risolubilità e le stesse soluzioni.

**(III) Ottimizzazione dell'informazione** — *rappresentazione matriciale del III tipo*:

$$
\begin{bmatrix} 1 & -3 \\ 4 & 5 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}
\ \leadsto\
\left[\begin{array}{cc|c} 1 & -3 & 2 \\ 4 & 5 & 1 \end{array}\right]
$$

(colonne: «$x$», «$y$», «termini noti»).

### Caso generale

Un sistema lineare di $m$ equazioni in $n$ incognite è del tipo

$$
\begin{cases}
a_{11}x_1 + a_{12}x_2 + \cdots + a_{1n}x_n = b_1 \\
a_{21}x_1 + a_{22}x_2 + \cdots + a_{2n}x_n = b_2 \\
\qquad\vdots \\
a_{m1}x_1 + a_{m2}x_2 + \cdots + a_{mn}x_n = b_m
\end{cases}
$$

- **I tipo**:

  $$x_1\begin{bmatrix} a_{11} \\ a_{21} \\ \vdots \\ a_{m1} \end{bmatrix} + x_2\begin{bmatrix} a_{12} \\ a_{22} \\ \vdots \\ a_{m2} \end{bmatrix} + \cdots + x_n\begin{bmatrix} a_{1n} \\ \vdots \\ a_{mn} \end{bmatrix} = \begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_m \end{bmatrix}$$

- **II tipo**:

  $$\underbrace{\begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & & \vdots \\ \vdots & \vdots & & \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix}}_{A}\underbrace{\begin{bmatrix} x_1 \\ \vdots \\ x_n \end{bmatrix}}_{\underline{x}} = \underbrace{\begin{bmatrix} b_1 \\ \vdots \\ b_m \end{bmatrix}}_{\underline{b}} \iff A\underline{x} = \underline{b}$$

- **III tipo**: la **matrice completa** (o aumentata)

  $$[A \mid \underline{b}] = \left[\begin{array}{ccc|c} a_{11} & \cdots & a_{1n} & b_1 \\ \vdots & & \vdots & \vdots \\ a_{m1} & \cdots & a_{mn} & b_m \end{array}\right] \in M_{\mathbb{K}}(m,n+1)$$

  con $A \in M_{\mathbb{K}}(m,n)$ e $\underline{b} \in M_{\mathbb{K}}(m,1) \cong \mathbb{K}^m$.

---
Successivo: [[Risoluzione di un Sistema con il MEG]]
