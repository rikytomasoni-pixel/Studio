---
tags: [GAL, matrici, determinante, laplace, definizione, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 51-54)"
---

# Determinante: sviluppo di Laplace

Determinante... (vedi anche i casi $2 \times 2$ e $3 \times 3$ in [[28_Determinanti_2x2_e_3x3]]).

> [!warning] Def. 6.4 Determinante (sviluppo di Laplace del determinante)
> Il determinante è una funzione
> $$\det : M_{\mathbb{K}}(n,n) \to \mathbb{K}$$
> definita come:
> - ($n = 1$) $\quad \det([a_{11}]) = a_{11}$
> - ($n > 1$) $\quad \displaystyle \det(A) = \sum_{j=1}^{n} (-1)^{i+j}\, a_{ij}\, \det(\hat{A}_{ij})$ dove
>   - $i$ è un indice di riga (qualsiasi) fissato
>   - $a_{ij}$ è l'elemento di $A$ sulla $i$-esima riga e $j$-esima colonna
>   - $\hat{A}_{ij} \in M_{\mathbb{K}}(n-1,n-1)$ è ottenuta da $A$ eliminando la $i$-esima riga e la $j$-esima colonna.
>
> In maniera equivalente
> $$\det(A) = \sum_{i=1}^{n} (-1)^{i+j}\, a_{ij}\, \det \hat{A}_{ij}$$
> dove
>   - $j$ è un indice di colonna (qualsiasi) fissato
>   - $a_{ij}$ è l'elemento di $A$ sulla $i$-esima riga e $j$-esima colonna
>   - $\hat{A}_{ij} \in M_{\mathbb{K}}(n-1,n-1)$ è ottenuta da $A$ eliminando la $i$-esima riga e la $j$-esima colonna.
>   - Il **cofattore** $C_{ij}$ relativo all'elemento $a_{ij}$ di una matrice quadrata $A$ è il valore scalare definito da: $$C_{ij} = (-1)^{i+j} \det(\hat{A}_{ij})$$ dove:  **$\hat{A}_{ij} \in M_{\mathbb{K}}(n-1,n-1)$** è la sottomatrice (detta *minore complementare*) ottenuta eliminando da $A$ la $i$-esima riga e la $j$-esima colonna. **$(-1)^{i+j}$** è il segno algebrico associato alla posizione $(i,j)$.

> [!abstract] Teorema (Teorema di Laplace)
> «il risultato non dipende dalla scelta di riga o colonna»

> [!example] Esempio (sviluppo lungo la riga $i=1$)
> $$B = \begin{bmatrix} 9 & 2 & -2 \\ 2 & 2 & 0 \\ -2 & 0 & 2 \end{bmatrix}$$
> $$\det(B) \overset{i=1}{=} \sum_{j=1}^{3} (-1)^{1+j}\, b_{1j} \det \hat{B}_{1j} = (-1)^{1+1} b_{11} \det \hat{B}_{11} + (-1)^{1+2} b_{12} \det \hat{B}_{12} + (-1)^{1+3} b_{13} \det \hat{B}_{13}$$
> $$= +9 \det\left(\begin{bmatrix} 2 & 0 \\ 0 & 2 \end{bmatrix}\right) - 2 \det\left(\begin{bmatrix} 2 & 0 \\ -2 & 2 \end{bmatrix}\right) + (-2) \det\left(\begin{bmatrix} 2 & 2 \\ -2 & 0 \end{bmatrix}\right)$$
> $$= 9(2\cdot2 - 0\cdot0) - 2(2\cdot2 - (-2)\cdot0) - 2(2\cdot0 - (-2)\cdot2) = 9\cdot4 - 2\cdot4 - 2\cdot4 = (9-4)\cdot4 = 20.$$



> [!example] Caso $2 \times 2$ (sviluppo lungo la colonna $j=1$)
> $$\det\left(\begin{bmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{bmatrix}\right) \overset{j=1}{=} \sum_{i=1}^{2} (-1)^{i+1} a_{i1} \det(\hat{A}_{i1}) = (-1)^{1+1} a_{11} \det([a_{22}]) + (-1)^{2+1} a_{21} \det([a_{12}])$$
> $$= a_{11}a_{22} - a_{21}a_{12}$$


> [!note] Osservazione (Idea)
> **IDEA** sfruttare a nostro vantaggio la libertà di scegliere righe / colonne nel calcolo del determinante.

> [!example] Esempio (sviluppo lungo la colonna $j=3$)
> $$\det B \overset{j=3}{=} \sum_{i=1}^{3} (-1)^{i+3}\, b_{i3} \det \hat{B}_{i3} = (-1)^{1+3} b_{13} \det \hat{B}_{13} + (-1)^{2+3} b_{23} \det \hat{B}_{23} + (-1)^{3+3} b_{33} \det \hat{B}_{33}$$
> $$= +(-2) \det \hat{B}_{13} - 0 \cdot \det \hat{B}_{23} + 2 \det \hat{B}_{33}$$
> $$= -2 \det\left(\begin{bmatrix} 2 & 2 \\ -2 & 0 \end{bmatrix}\right) + 2 \det\left(\begin{bmatrix} 9 & 2 \\ 2 & 2 \end{bmatrix}\right) = -2\,(2\cdot0 - (-2)\cdot2) + 2\,(9\cdot2 - 2\cdot2) = -2\cdot4 + 2\cdot14 = 2(-4+14) = 20$$

**Obiettivo:** selezionare una riga / una colonna con più zeri possibile.

> [!example] Esempio (I)
> $A \in M_{\mathbb{K}}(n,n)$ con una riga o una colonna tutta di zeri $\Rightarrow \det(A) = 0$.

Le matrici triangolari (esempio II) sono in [[66_Matrici_Triangolari]].

## Note collegate
- [[28_Determinanti_2x2_e_3x3]]
- [[66_Matrici_Triangolari]]
- [[74_Teorema_di_Binet]]
- [[75_Calcolo_del_Determinante_con_il_MEG]]
- [[76_Determinante_Normalizzato_e_Alternante]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]

#GAL/determinante/determinante-sviluppo-di-laplace
