---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, simmetria-assiale, matrice-diagonale, esempio, geometria, lezione-23]
data: 2026-11-19
lezione: 23
fonte: "GAL 2026-2027 - 20261119 - LEZIONE 23.pdf (slide 186-188)"
---

# Simmetria assiale: una base adattata e matrice diagonale

$L:\mathbb{R}^2\to\mathbb{R}^2$ simmetria assiale (esempio di [[166_Esempio_Simmetria_Assiale_Matrice_nella_Base_Canonica]]), con origine $O$ sulla retta.

> [!abstract] Obiettivo
> Trovare una base alternativa che **semplifichi la trattazione algebrica**.

**Come?** Trovare una base che si accorge del caso specifico: trovare due vettori (linearmente indipendenti) per cui la simmetria assiale ha un comportamento speciale.

- $\vec{v}$ sulla retta: $L(\vec{v})=\vec{v}$.
- $\vec{w}$ perpendicolare alla retta: $L(\vec{w})=-\vec{w}$.

![[nota167disegno.png]]

## Matrice rispetto alla base $\mathcal{C}=\{\vec{v},\vec{w}\}$
$$B=M_{\mathcal{C}}^{\mathcal{C}}(L)=\begin{bmatrix}1&0\\0&-1\end{bmatrix}\in M_{\mathbb{R}}(2,2)$$
(colonne $L(\vec{v})$, $L(\vec{w})$; righe $\vec{v}$, $\vec{w}$).

- $\vec{v}$: $L(\vec{v})=\vec{v}=\mathbf{1}\vec{v}+\mathbf{0}\vec{w}$, $\ \mathcal{X}_{\mathcal{C}}(L(\vec{v}))=\begin{bmatrix}1\\0\end{bmatrix}$.
- $\vec{w}$: $L(\vec{w})=-\vec{w}=\mathbf{0}\vec{v}+(\mathbf{-1})\vec{w}$, $\ \mathcal{X}_{\mathcal{C}}(L(\vec{w}))=\begin{bmatrix}0\\-1\end{bmatrix}$.

## Confronto tra le due rappresentazioni
$$\mathcal{B}=\{\vec{i},\vec{j}\}:\ A=M_{\mathcal{B}}^{\mathcal{B}}(L)=\begin{bmatrix}\cos2\theta&\sin2\theta\\\sin2\theta&-\cos2\theta\end{bmatrix}\qquad\mathcal{C}=\{\vec{v},\vec{w}\}:\ B=M_{\mathcal{C}}^{\mathcal{C}}(L)=\begin{bmatrix}1&0\\0&-1\end{bmatrix}$$

![[simmetriaConBasi.png]]

> [!note] OSS 1
> La matrice $B$ è **diagonale**, quindi contiene molti zeri $\Rightarrow$ vantaggio in **spazio di memoria**.

> [!note] OSS 2 — facilità di calcolo di $L(\vec{u})$
> - Con $\mathcal{B}$ (per $\mathcal{X}_{\mathcal{B}}(\vec{u})=\begin{bmatrix}2\\2\end{bmatrix}$):
> $$A\,\mathcal{X}_{\mathcal{B}}(\vec{u})=\begin{bmatrix}\cos2\theta&\sin2\theta\\\sin2\theta&-\cos2\theta\end{bmatrix}\begin{bmatrix}2\\2\end{bmatrix}=\begin{bmatrix}2\cos2\theta+2\sin2\theta\\2\sin2\theta-2\cos2\theta\end{bmatrix}$$
> **4 prodotti, 2 somme**.
> - Con $\mathcal{C}$ (per $\mathcal{X}_{\mathcal{C}}(\vec{u})=\begin{bmatrix}2+\varepsilon_1\\1-\varepsilon_2\end{bmatrix}$):
> $$B\,\mathcal{X}_{\mathcal{C}}(\vec{u})=\begin{bmatrix}1&0\\0&-1\end{bmatrix}\begin{bmatrix}2+\varepsilon_1\\1-\varepsilon_2\end{bmatrix}=\begin{bmatrix}1\,(2+\varepsilon_1)\\(-1)(1-\varepsilon_2)\end{bmatrix}=\begin{bmatrix}2+\varepsilon_1\\-(1-\varepsilon_2)\end{bmatrix}$$
> **2 prodotti, 0 somme**.

> [!tip] Morale
> La seconda rappresentazione è **più efficace**. Per ottenerla abbiamo dovuto identificare i vettori migliori per il problema!
> Resta da capire come legare $A$ e $B$: [[168_Matrice_del_Cambio_di_Base_Definizione_23_1]] e [[169_Esempio_Cambio_di_Base_per_la_Simmetria_Assiale]].

## Note collegate
- [[176_Obiettivo_1_Azione_di_L_sulla_Base_Diagonalizzante]]
- [[177_Definizione_25_1_Autovettore_e_Autovalore]]
- [[166_Esempio_Simmetria_Assiale_Matrice_nella_Base_Canonica]]
- [[165_Dipendenza_della_Matrice_Rappresentativa_dalle_Basi]]
- [[174_Matrici_Diagonalizzabili_Definizione_23_3]]
- [[45_Matrice_Identita_e_Matrici_Diagonali]]
- [[37_Efficienza_Computazionale]]
- Indice: [[24_Indice_Lezione_23]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/base-adattata
