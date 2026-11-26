---
tags: [GAL, autovettori, diagonalizzabilita, esempio, polinomi, lezione-25]
data: 2026-11-25
lezione: 25
fonte: "GAL 2026-2027 - 20261125 - LEZIONE 25.pdf (slide 201-202)"
---

# Obiettivo concreto: cercare gli autovettori. Esempio 1: matrice di $L(p)=tp''-p'$

> [!abstract] Obiettivo
> Trovare una **rappresentazione diagonale** di un endomorfismo $L:V\to V$.
>
> **Obiettivo concreto:** trovare gli **autovettori** (e gli **autovalori**) di un endomorfismo.

## Esempio 1

$$L:\mathbb{K}[t]_{\le3}\to\mathbb{K}[t]_{\le3},\qquad p(t)\longmapsto t\,p''(t)-p'(t)$$

> [!question] Domanda
> $L$ può essere rappresentato da una matrice diagonale?

### Passo 0: matrice rappresentativa rispetto alla base canonica

$\mathcal{B}=\{1,t,t^2,t^3\}$, $A=M_{\mathcal{B}}^{\mathcal{B}}(L)\in M_{\mathbb{K}}(4,4)$ (le colonne sono le coordinate di $L(1),L(t),L(t^2),L(t^3)$):

- $L(1)=t\cdot0-0=0=0\cdot1+0t+0t^2+0t^3$
- $L(t)=t\cdot0-1=-1=(-1)\cdot1+0t+0t^2+0t^3$
- $L(t^2)=t\cdot2-2t=0=0\cdot1+0t+0t^2+0t^3$
- $L(t^3)=t\,(6t)-3t^2=3t^2=0\cdot1+0t+3t^2+0t^3$

$$A=\begin{bmatrix}0&-1&0&0\\0&0&0&0\\0&0&0&3\\0&0&0&0\end{bmatrix}$$

> [!warning] N.B.
> $A$ **non è diagonale**, ma ha tanti zeri. Per capire se esiste una base che la renda diagonale si cercano gli autovettori ([[181_Autovettori_come_Soluzioni_Non_Nulle_del_Sistema_Omogeneo_A_meno_lambda_Id]]).

## Note collegate
- [[177_Definizione_25_1_Autovettore_e_Autovalore]]
- [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita]]
- [[181_Autovettori_come_Soluzioni_Non_Nulle_del_Sistema_Omogeneo_A_meno_lambda_Id]]
- [[182_Esempio_1_Autovettori_di_Autovalore_0_e_Non_Diagonalizzabilita]]
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- Indice: [[26_Indice_Lezione_25]] · [[00_MOC_GAL]]

#GAL/autovalori/ricerca-autovettori
