---
tags: [GAL, applicazioni-lineari, esempi, matrici, trasposizione, traccia, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 147-148)"
---

# Esempi di applicazioni lineari: $L_A$, trasposizione, traccia

## (I) L'applicazione $L_A$ associata a una matrice
$V=\mathbb{K}^n$, $W=\mathbb{K}^m$, $A\in M_{\mathbb{K}}(m,n)$. Definiamo
$$L_A:\mathbb{K}^n\to\mathbb{K}^m,\qquad L_A(\underline{v})=A\underline{v}$$
$L_A$ è un'applicazione lineare per le proprietà del prodotto matriciale ([[44_Proprieta_del_Prodotto_Matriciale]]):

**Additività.** $\forall\underline{v}_1,\underline{v}_2\in\mathbb{K}^n$
$$L_A(\underline{v}_1+\underline{v}_2)\overset{\text{def}}{=}A(\underline{v}_1+\underline{v}_2)\overset{\text{distr. a dx}}{=}A\underline{v}_1+A\underline{v}_2\overset{\text{def}}{=}L_A(\underline{v}_1)+L_A(\underline{v}_2)$$
**Omogeneità.** $\forall\underline{v}\in\mathbb{K}^n$, $\forall\lambda\in\mathbb{K}$
$$L_A(\lambda\underline{v})\overset{\text{def}}{=}A(\lambda\underline{v})=\lambda(A\underline{v})\overset{\text{def}}{=}\lambda L_A(\underline{v})$$

> [!example] Esempio numerico
> $A=\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix}$, $V=\mathbb{R}^3$, $W=\mathbb{R}^2$:
> $$L_A\left(\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}\right)=\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}=\begin{bmatrix}x_1+2x_2+3x_3\\4x_1+5x_2+6x_3\end{bmatrix}$$

## (II) La trasposizione
$V=M_{\mathbb{K}}(m,n)$, $W=M_{\mathbb{K}}(n,m)$,
$$T:V\to W,\qquad A\mapsto A^T$$
La trasposizione scambia il ruolo di righe e colonne: le righe $R_1(A),\dots,R_m(A)$ di $A$ diventano le colonne di $A^T$.

> [!example] Esempio
> $$\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix}\xrightarrow{\ T\ }\begin{bmatrix}1&4\\2&5\\3&6\end{bmatrix}$$
> (la prima riga $[1\ 2\ 3]$ diventa la prima colonna, la seconda riga $[4\ 5\ 6]$ la seconda colonna; letto per colonne: le colonne $\binom14,\binom25,\binom36$ diventano le righe.)

> [!todo] Per casa
> Verificare che $T$ è un'applicazione lineare.

## (III) La traccia
$V=M_{\mathbb{K}}(n,n)$, $W=\mathbb{K}^1$:
$$\operatorname{tr}:M_{\mathbb{K}}(n,n)\to\mathbb{K},\qquad\operatorname{tr}(A)=\sum_{i=1}^{n}a_{ii}=a_{11}+a_{22}+\dots+a_{nn}$$

> [!example] Esempio
> $$\operatorname{tr}\left(\begin{bmatrix}1&2&4\\0&7&-3\\2&0&1\end{bmatrix}\right)=1+7+1=9$$


> [!todo] Per casa
> Verificare omogeneità e additività.

## Note collegate
- [[150_Suriettivita_di_L_A_e_Spazio_delle_Colonne]] · [[151_Nucleo_di_una_Applicazione_Lineare]]
- [[136_Applicazioni_Lineari_Definizione_17_1]]
- [[138_Derivata_come_Applicazione_Lineare]]
- [[141_Composizione_e_Inversione_di_Applicazioni_Lineari]]
- [[35_Somma_tra_Matrici]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/esempi
