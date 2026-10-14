---
created: 2026-10-08
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/eliminazione_di_gauss
aliases: []
origine: UpdateVault
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# MEG e Rango

«il rango vuole essere una misura di complessità (quanta informazione c'è) di una matrice»
«MEG concentra l'informazione nella parte alta e a destra della matrice»

> [!example] Esempio
> Matrice di probabilità congiunta ([[Rango e Probabilità Congiunta]]), con $p_1 = \frac{1}{12}$ (primo elemento):
> $$\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}$$
> Applico il MEG: $\mathrm{II} - \dfrac{\frac{1}{12}}{\frac{1}{12}}\,\mathrm{I} \to \mathrm{II}$ (coefficiente $1$)
> $$\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix}$$
> Codifica con il prodotto ([[Codifica del MEG con il Prodotto]]):
> $$\begin{bmatrix} 1 & 0 \\ -1 & 1 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix}$$
> $$\begin{bmatrix} 1 & 0 \\ +1 & 1 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}$$
> $$\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} \qquad \text{rango } 1$$
> $$\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix} \left( \begin{bmatrix} 1 \\ 0 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} \right) = \left( \begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix} \begin{bmatrix} 1 \\ 0 \end{bmatrix} \right) \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \end{bmatrix} \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix} = \begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}$$
> $$\Rightarrow\ r\left(\begin{bmatrix} \frac{1}{12} & \cdots & \frac{1}{12} \\ \frac{1}{12} & \cdots & \frac{1}{12} \end{bmatrix}\right) = 1$$

> [!abstract] Teorema (Proposizione)
> Dato $A \in M_{\mathbb{K}}(m,n)$, sia $U$ una matrice a scala ottenuta con il MEG a partire da $A$ ([[Pivot e Matrice a Scala]]).
> - $r(U)$ = numero di righe non nulle di $U$ = numero di pivot di $U$
> - $r(A) = r(U)$

Il MEG è il modo **EFFICIENTE** per calcolare il rango di una matrice!!

> [!example] Esempio
> Calcolo il rango di
> $$\begin{bmatrix} 1 & 0 & -1 & 2 \\ 2 & 0 & 3 & 1 \\ 1 & 0 & 4 & -1 \end{bmatrix} \xrightarrow[\ \mathrm{III} - \mathrm{I} \to \mathrm{III}\ ]{\ \mathrm{II} - 2\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 5 & -3 \end{bmatrix} \xrightarrow{\ \mathrm{III} - \mathrm{II} \to \mathrm{III}\ } \begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 0 & 0 \end{bmatrix} \Rightarrow r = 2$$

![[2026-10-08-calcolo-rango-con-MEG.png]]

---
Precedente: [[Esistenza della Matrice Inversa]]
