---
tags: [GAL, sistemi-lineari, matrici, rappresentazione-matriciale, lezione-9]
data: 2026-10-12
lezione: 9
fonte: "GAL_2026-2027_-_20261012_-_LEZIONE_9.pdf (slide 74-76)"
destinazione: "20_Geometria_Algebra_Lineare/11_Sistemi_Lineari"
---

# Rappresentazioni matriciali di un sistema lineare

Per i sistemi lineari interessano due aspetti: la **formalizzazione** e la **risoluzione** (teorica / pratica).

## Esempio guida

$$\begin{cases} x-3y=2 \\ 4x+5y=1 \end{cases}$$
2 incognite ($x,y$), 2 equazioni. Per **uguaglianza tra matrici** il sistema equivale a
$$\begin{bmatrix} x-3y \\ 4x+5y \end{bmatrix}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

### Rappresentazione matriciale del I tipo
Uso la somma tra matrici ([[35_Somma_tra_Matrici]]) e il prodotto per scalari ([[36_Prodotto_di_una_Matrice_per_uno_Scalare]]):
$$\begin{bmatrix} x-3y \\ 4x+5y \end{bmatrix}=\begin{bmatrix} x \\ 4x \end{bmatrix}+\begin{bmatrix} -3y \\ 5y \end{bmatrix}= x\begin{bmatrix} 1 \\ 4 \end{bmatrix}+y\begin{bmatrix} -3 \\ 5 \end{bmatrix}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}$$
Un sistema con 2 equazioni e 2 incognite è equivalente a **1 equazione** che coinvolge vettori colonna di altezza 2.

### Rappresentazione matriciale del II tipo
Uso il prodotto matriciale ([[41_Prodotto_Matriciale_Righe_per_Colonne]]):
$$\begin{bmatrix} x-3y \\ 4x+5y \end{bmatrix}=\begin{bmatrix} 1 & -3 \\ 4 & 5 \end{bmatrix}\begin{bmatrix} x \\ y \end{bmatrix}=\begin{bmatrix} 2 \\ 1 \end{bmatrix}$$

> [!note] Osservazione 1
> La matrice dei coefficienti (nel II tipo) è la **giustapposizione dei vettori colonna dei coefficienti** (I tipo).

> [!note] Osservazione 2
> Il nome di $x$ e $y$ è marginale: il sistema $\begin{cases} A-3B=2 \\ 4A+5B=1 \end{cases}$ ha la stessa risolubilità e le stesse soluzioni.

### Rappresentazione matriciale del III tipo (ottimizzazione dell'informazione)
Si scrive solo ciò che serve: i coefficienti delle incognite ("$x$", "$y$") e i termini noti.
$$\left[\begin{array}{cc|c} 1 & -3 & 2 \\ 4 & 5 & 1 \end{array}\right]$$

## Caso generale

Un sistema lineare di $m$ equazioni in $n$ incognite è del tipo
$$\begin{cases} a_{11}x_1+a_{12}x_2+\dots+a_{1n}x_n=b_1 \\ a_{21}x_1+a_{22}x_2+\dots+a_{2n}x_n=b_2 \\ \quad\vdots \\ a_{m1}x_1+a_{m2}x_2+\dots+a_{mn}x_n=b_m \end{cases}$$

**I tipo**
$$x_1\begin{bmatrix} a_{11}\\ a_{21}\\ \vdots\\ a_{m1}\end{bmatrix}+x_2\begin{bmatrix} a_{12}\\ a_{22}\\ \vdots\\ a_{m2}\end{bmatrix}+\dots+x_n\begin{bmatrix} a_{1n}\\ \vdots\\ a_{mn}\end{bmatrix}=\begin{bmatrix} b_1\\ b_2\\ \vdots\\ b_m\end{bmatrix}$$

**II tipo**
$$\underbrace{\begin{bmatrix} a_{11} & a_{12} & \dots & a_{1n}\\ a_{21} & a_{22} & \dots & a_{2n}\\ \vdots & \vdots & & \vdots\\ a_{m1} & a_{m2} & \dots & a_{mn}\end{bmatrix}}_{A}\underbrace{\begin{bmatrix} x_1\\ \vdots\\ x_n\end{bmatrix}}_{\underline{x}}=\underbrace{\begin{bmatrix} b_1\\ \vdots\\ b_m\end{bmatrix}}_{\underline{b}} \iff A\underline{x}=\underline{b}$$

**III tipo**
$$\left[A\mid \underline{b}\right]=\left[\begin{array}{ccc|c} a_{11} & \dots & a_{1n} & b_1\\ \vdots & & \vdots & \vdots\\ a_{m1} & \dots & a_{mn} & b_m\end{array}\right]\in M_{\mathbb{K}}(m,n+1)$$
con $A\in M_{\mathbb{K}}(m,n)$ e $\underline{b}\in M_{\mathbb{K}}(m,1)\simeq\mathbb{K}^m$ (vedi [[32_Definizione_di_Matrice]]).

## Risoluzione: le due domande
1. Il sistema è risolubile?
2. Se la risposta a 1 è sì, **quante** e **quali** sono le soluzioni?

Un esempio con parametri e la risoluzione per riduzione: [[81_Risoluzione_di_un_Sistema_con_MEG_Esempio_Parametrico]].

## Note collegate
- [[81_Risoluzione_di_un_Sistema_con_MEG_Esempio_Parametrico]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- Indice: [[10_Indice_Lezione_9]] · [[00_MOC_GAL]]

#GAL/sistemi-lineari/rappresentazioni-matriciali
