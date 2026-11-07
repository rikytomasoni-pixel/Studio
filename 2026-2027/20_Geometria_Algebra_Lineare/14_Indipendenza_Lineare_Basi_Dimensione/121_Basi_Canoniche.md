---
tags: [GAL, base, base-canonica, dimensione, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 125-126)"
---

# Basi canoniche

## $\mathbb{K}^n$
Ogni $\underline{v}\in\mathbb{K}^n$ si scrive
$$\underline{v}=\begin{bmatrix}v_1\\ \vdots\\ v_n\end{bmatrix}=\begin{bmatrix}v_1\\0\\ \vdots\\0\end{bmatrix}+\begin{bmatrix}0\\v_2\\0\\ \vdots\\0\end{bmatrix}+\dots+\begin{bmatrix}0\\ \vdots\\0\\v_n\end{bmatrix}=v_1\begin{bmatrix}1\\0\\ \vdots\\0\end{bmatrix}+v_2\begin{bmatrix}0\\1\\0\\ \vdots\\0\end{bmatrix}+\dots+v_n\begin{bmatrix}0\\ \vdots\\0\\1\end{bmatrix}$$
Quindi $\mathcal{B}=\{\underline{e}_1,\underline{e}_2,\dots,\underline{e}_n\}$ è una **base** di $\mathbb{K}^n$ (base canonica) e
$$\dim\mathbb{K}^n=n.$$

## $M_{\mathbb{K}}(2,2)$ e $M_{\mathbb{K}}(m,n)$
$$A=\begin{bmatrix}a&b\\c&d\end{bmatrix}=a\begin{bmatrix}1&0\\0&0\end{bmatrix}+b\begin{bmatrix}0&1\\0&0\end{bmatrix}+c\begin{bmatrix}0&0\\1&0\end{bmatrix}+d\begin{bmatrix}0&0\\0&1\end{bmatrix}$$
$\{E_{11},E_{12},E_{21},E_{22}\}$ è la base canonica di $M_{\mathbb{K}}(2,2)$.

In generale, con $E_{ij}$ la matrice con $1$ al posto $(i,j)$ e $0$ altrove:
$$M_{\mathbb{K}}(m,n)=\operatorname{Span}\big(E_{ij}\ \big|\ i=1,\dots,m,\ j=1,\dots,n\big)\qquad\dim M_{\mathbb{K}}(m,n)=mn.$$

## $\mathbb{K}[t]_{\le d}$
$$\mathbb{K}[t]_{\le d}=\operatorname{Span}(1,t,\dots,t^d)$$
$\{1,t,\dots,t^d\}$ è la base canonica di $\mathbb{K}[t]_{\le d}$ e
$$\dim\mathbb{K}[t]_{\le d}=d+1.$$

> [!note] Osservazione (non presente negli appunti)
> Le scritture sopra mostrano che gli insiemi canonici sono **generatori**; l'indipendenza lineare segue dall'unicità dei coefficienti (due combinazioni coincidono solo se coincidono tutte le componenti / tutti i coefficienti). Per $\mathbb{K}[t]_{\le d}$ vedi anche [[96_Insieme_di_Generatori]]; per $\mathbb{R}^2$ la base canonica è già in [[102_Dimensione_di_uno_Spazio_Vettoriale]].

## Note collegate
- [[100_Base_di_uno_Spazio_Vettoriale]]
- [[102_Dimensione_di_uno_Spazio_Vettoriale]]
- [[92_Esempi_di_Spazi_Vettoriali]]
- [[32_Definizione_di_Matrice]]
- Successiva: [[122_Estrazione_e_Completamento_Due_Problemi_Classici]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/base/basi-canoniche
