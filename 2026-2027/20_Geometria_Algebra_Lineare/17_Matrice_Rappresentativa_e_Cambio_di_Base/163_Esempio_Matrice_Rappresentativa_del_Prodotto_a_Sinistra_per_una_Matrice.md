---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, esempio, matrici-2x2, lezione-22]
data: 2026-11-18
lezione: 22
fonte: "GAL 2026-2027 - 20261118 - LEZIONE 22.pdf (slide 179-180)"
---

# Esempio: matrice rappresentativa di $X\mapsto BX$ su $M_{\mathbb{R}}(2,2)$

$V=W=M_{\mathbb{R}}(2,2)$, $\mathcal{B}=\mathcal{C}=\{E_{11},E_{12},E_{21},E_{22}\}$ (base canonica), e
$$L:M_{\mathbb{R}}(2,2)\to M_{\mathbb{R}}(2,2),\qquad L(X)=B\cdot X,\qquad B=\begin{bmatrix}1&2\\3&6\end{bmatrix}.$$

> [!note] Notazione
> Nel quaderno la matrice variabile è chiamata $A$ ($L(A)=B\cdot A$); qui la chiamo $X$ per non confonderla con la matrice rappresentativa $A\in M_{\mathbb{R}}(4,4)$.

> [!warning] N.B.
> $B$ **non** è la matrice rappresentativa di $L$. Infatti $\mathcal{X}_{\mathcal{B}}$ manda $M_{\mathbb{R}}(2,2)$ in $\mathbb{R}^4$, quindi
> $$A\in M_{\mathbb{R}}(4,4),\qquad\begin{array}{ccc}M_{\mathbb{R}}(2,2)&\xrightarrow{\ L\ }&M_{\mathbb{R}}(2,2)\\\mathcal{X}_{\mathcal{B}}\downarrow&&\downarrow\mathcal{X}_{\mathcal{B}}\\\mathbb{R}^4&\xrightarrow{\ L_A\ }&\mathbb{R}^4\end{array}$$

## Compilazione colonna per colonna
$$A=M_{\mathcal{B}}^{\mathcal{B}}(L)=\Big[\,\mathcal{X}_{\mathcal{B}}(L(E_{11}))\,\Big|\,\mathcal{X}_{\mathcal{B}}(L(E_{12}))\,\Big|\,\mathcal{X}_{\mathcal{B}}(L(E_{21}))\,\Big|\,\mathcal{X}_{\mathcal{B}}(L(E_{22}))\,\Big]$$

- $E_{11}$: $L(E_{11})=BE_{11}=\begin{bmatrix}1&0\\3&0\end{bmatrix}=\mathbf{1}E_{11}+\mathbf{0}E_{12}+\mathbf{3}E_{21}+\mathbf{0}E_{22}$, quindi $\mathcal{X}_{\mathcal{B}}(L(E_{11}))=\begin{bmatrix}1\\0\\3\\0\end{bmatrix}$.
- $E_{12}$: $L(E_{12})=BE_{12}=\begin{bmatrix}0&1\\0&3\end{bmatrix}=0E_{11}+1E_{12}+0E_{21}+3E_{22}$, quindi $\mathcal{X}_{\mathcal{B}}(L(E_{12}))=\begin{bmatrix}0\\1\\0\\3\end{bmatrix}$.
- $E_{21}$: $L(E_{21})=BE_{21}=\begin{bmatrix}2&0\\6&0\end{bmatrix}=2E_{11}+0E_{12}+6E_{21}+0E_{22}$, quindi $\mathcal{X}_{\mathcal{B}}(L(E_{21}))=\begin{bmatrix}2\\0\\6\\0\end{bmatrix}$.
- $E_{22}$: $L(E_{22})=BE_{22}=\begin{bmatrix}0&2\\0&6\end{bmatrix}=0E_{11}+2E_{12}+0E_{21}+6E_{22}$, quindi $\mathcal{X}_{\mathcal{B}}(L(E_{22}))=\begin{bmatrix}0\\2\\0\\6\end{bmatrix}$.

$$\boxed{A=\begin{bmatrix}1&0&2&0\\0&1&0&2\\3&0&6&0\\0&3&0&6\end{bmatrix}}$$

## Note collegate
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- [[161_Obiettivo_Costruire_la_Matrice_del_Paradigma]]
- [[158_Mappa_delle_Coordinate_e_Mappa_di_Parametrizzazione_Definizione_20_6]]
- [[92_Esempi_di_Spazi_Vettoriali]]
- Indice: [[23_Indice_Lezione_22]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/esempio-matrici-2x2
