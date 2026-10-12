---
tags: [GAL, matrici, MEG, rango, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 66-67)"
---

# MEG e rango

«il rango vuole essere una misura di complessità (quanta informazione c'è) di una matrice»
«MEG concentra l'informazione nella parte alta e a destra della matrice»

> [!example] Esempio
> Matrice di probabilità congiunta ([[64_Rango_e_Matrice_di_Probabilita_Congiunta]]), con $p_1 = \frac{1}{12}$ (primo elemento):
> $$\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}$$
> Applico il MEG: $\mathrm{II} - \dfrac{\frac{1}{12}}{\frac{1}{12}}\,\mathrm{I} \to \mathrm{II}$ (coefficiente $1$)
> $$\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix}$$
> Codifica con il prodotto ([[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]):
> $$\begin{bmatrix} 1 & 0 \\ -1 & 1 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix}$$
> $$\begin{bmatrix} 1 & 0 \\ +1 & 1 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}$$
> $$\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} \qquad \text{rango } 1$$
> $$\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix} \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} \right) = \left( \begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix} \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}$$
> $$\Rightarrow\ r\left(\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}\right) = 1$$

> [!abstract] Teorema (Proposizione)
> Dato $A \in M_{\mathbb{K}}(m,n)$, sia $U$ una matrice a scala ottenuta con il MEG a partire da $A$ ([[69_Pivot_e_Matrice_a_Scala]]).
> - $r(U)$ = numero di righe non nulle di $U$ = numero di pivot di $U$
> - $r(A) = r(U)$

Il MEG è il modo **EFFICIENTE** per calcolare il rango di una matrice!!

> [!example] Esempio
> Calcolo il rango di
> $$\begin{bmatrix} 1 & 0 & -1 & 2 \\ 2 & 0 & 3 & 1 \\ 1 & 0 & 4 & -1 \end{bmatrix} \xrightarrow[\ \mathrm{III} - \mathrm{I} \to \mathrm{III}\ ]{\ \mathrm{II} - 2\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 5 & -3 \end{bmatrix} \xrightarrow{\ \mathrm{III} - \mathrm{II} \to \mathrm{III}\ } \begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 0 & 0 \end{bmatrix} \Rightarrow r = 2$$

![[CalcoloRangoMEG.png]]

## Note collegate
- [[63_Rango_di_una_Matrice]]
- [[64_Rango_e_Matrice_di_Probabilita_Congiunta]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[69_Pivot_e_Matrice_a_Scala]]
- [[71_Codifica_del_MEG_con_il_Prodotto_Matriciale]]
- Indice: [[08_Indice_Lezione_7]] · [[00_MOC_GAL]]
