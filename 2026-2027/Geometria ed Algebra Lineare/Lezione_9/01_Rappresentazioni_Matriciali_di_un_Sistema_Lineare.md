---
tags: [GAL, sistemi-lineari, rappresentazione-matriciale, lezione-9]
data: 2026-10-12
lezione: 9
fonte: "GAL 2026-2027 - 20261012 - LEZIONE 9.pdf (slide 74-76)"
---

# Rappresentazioni matriciali di un sistema lineare

**Sistemi lineari.** Due temi: formalizzazione e risoluzione (teorica / pratica).

## Esempio introduttivo

$$\begin{cases} x-3y=2 \\ 4x+5y=1 \end{cases}\qquad \text{2 incognite } x,y;\quad \text{2 equazioni}$$

Per l'uguaglianza tra matrici il sistema equivale a
$$\begin{bmatrix} x-3y \\ 4x+5y \end{bmatrix}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

### (I) Uso la somma tra matrici e il prodotto per scalari

$$\begin{bmatrix} x-3y \\ 4x+5y \end{bmatrix}=\begin{bmatrix} x \\ 4x \end{bmatrix}+\begin{bmatrix} -3y \\ 5y \end{bmatrix}=x\begin{bmatrix} 1 \\ 4 \end{bmatrix}+y\begin{bmatrix} -3 \\ 5 \end{bmatrix}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

> [!note] Rappresentazione matriciale del I tipo
> Un sistema con 2 equazioni e 2 incognite è equivalente a **1 equazione che coinvolge vettori colonna di altezza 2**.

### (II) Uso il prodotto matriciale

$$\begin{bmatrix} x-3y \\ 4x+5y \end{bmatrix}=\begin{bmatrix} 1 & -3 \\ 4 & 5 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

> [!note] Rappresentazione matriciale del II tipo

**Oss.** La matrice dei coefficienti (nel II tipo) è la giustapposizione dei vettori colonna dei coefficienti (I tipo).

**Oss. 2.** Il nome di $x$ e $y$ è marginale:
$$\begin{cases} x-3y=2 \\ 4x+5y=1 \end{cases}\qquad\qquad \begin{cases} A-3B=2 \\ 4A+5B=1 \end{cases}$$
La risolubilità e le soluzioni sono le medesime.

### (III) Ottimizzazione dell'informazione

$$\begin{bmatrix} 1 & -3 \\ 4 & 5 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}\ \leadsto\ \left[\begin{array}{cc|c} 1 & -3 & 2 \\ 4 & 5 & 1 \end{array}\right]$$
(colonne: "$x$", "$y$", "termini noti").

> [!note] Rappresentazione matriciale del III tipo

## Caso generale

Un sistema lineare di $m$ equazioni in $n$ incognite è del tipo
$$\begin{cases} a_{11}x_1+a_{12}x_2+\cdots+a_{1n}x_n=b_1 \\ a_{21}x_1+a_{22}x_2+\cdots+a_{2n}x_n=b_2 \\ \quad\vdots \\ a_{m1}x_1+a_{m2}x_2+\cdots+a_{mn}x_n=b_m \end{cases}$$

> [!abstract] I tipo
> $$x_1\begin{bmatrix} a_{11}\\ a_{21}\\ \vdots\\ a_{m1}\end{bmatrix}+x_2\begin{bmatrix} a_{12}\\ a_{22}\\ \vdots\\ a_{m2}\end{bmatrix}+\cdots+x_n\begin{bmatrix} a_{1n}\\ \vdots\\ a_{mn}\end{bmatrix}=\begin{bmatrix} b_1\\ b_2\\ \vdots\\ b_m\end{bmatrix}$$

> [!abstract] II tipo
> $$\underbrace{\begin{bmatrix} a_{11}&a_{12}&\cdots&a_{1n}\\ a_{21}&a_{22}&\cdots&a_{2n}\\ \vdots&&&\vdots\\ a_{m1}&a_{m2}&\cdots&a_{mn}\end{bmatrix}}_{A}\underbrace{\begin{bmatrix} x_1\\ \vdots\\ x_n\end{bmatrix}}_{\underline{x}}=\underbrace{\begin{bmatrix} b_1\\ \vdots\\ b_m\end{bmatrix}}_{\underline{b}}\iff A\underline{x}=\underline{b}$$

> [!abstract] III tipo
> $$[A\,|\,\underline{b}]=\left[\begin{array}{ccc|c} a_{11}&\cdots&a_{1n}&b_1\\ \vdots&&\vdots&\vdots\\ a_{m1}&\cdots&a_{mn}&b_m\end{array}\right]\in M_{\mathbb{K}}(m,n+1)$$
> con $A\in M_{\mathbb{K}}(m,n)$ e $\underline{b}\in M_{\mathbb{K}}(m,1)\simeq\mathbb{K}^m$.

### Note collegate
- [[00_Indice_Lezione_9]] · [[00_MOC_GAL]]
- [[02_Risoluzione_di_un_Sistema_con_il_MEG]]
- [[02_Prodotto_Matriciale_Righe_per_Colonne]] — prodotto matriciale usato nel II tipo
- [[01_Opposto_di_una_Matrice]] — somma e prodotto per scalari tra matrici (I tipo)
