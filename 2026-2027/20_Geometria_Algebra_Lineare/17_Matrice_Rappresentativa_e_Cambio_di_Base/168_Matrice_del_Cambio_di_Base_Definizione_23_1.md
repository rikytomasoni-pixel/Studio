---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, cambio-di-base, definizione, lezione-23]
data: 2026-11-19
lezione: 23
fonte: "GAL 2026-2027 - 20261119 - LEZIONE 23.pdf (slide 188-189)"
---

# Matrice del cambio di base (Definizione 23.1)

## Relazione tra due matrici rappresentative di una applicazione lineare
$L:V\to W$. In $V$ due basi $\mathcal{B}_1$ e $\mathcal{B}_2$; in $W$ due basi $\mathcal{C}_1$ e $\mathcal{C}_2$. Ci sono quattro matrici rappresentative, che corrispondono alle quattro frecce $\mathbb{K}^n\to\mathbb{K}^m$ del diagramma:

$$M_{\mathcal{B}_1}^{\mathcal{C}_1}(L)\qquad M_{\mathcal{B}_2}^{\mathcal{C}_1}(L)\qquad M_{\mathcal{B}_1}^{\mathcal{C}_2}(L)\qquad M_{\mathcal{B}_2}^{\mathcal{C}_2}(L)$$

![[MatriciRappresentativeRelazioni.png]]

## Il lato sinistro del diagramma
Concentriamoci sul lato sinistro: $V$ con le due mappe delle coordinate $\mathcal{X}_{\mathcal{B}_2}$ e $\mathcal{X}_{\mathcal{B}_1}$ verso $\mathbb{K}^n$. Cerco la freccia $\mathbb{K}^n\overset{?}{\dashrightarrow}\mathbb{K}^n$ che trasforma coordinate rispetto a $\mathcal{B}_2$ in coordinate rispetto a $\mathcal{B}_1$. È la matrice rappresentativa della funzione identità:
$$\begin{array}{ccc}
V&\xlongequal{\ \ \mathrm{id}\ \ }&V\\
\mathcal{X}_{\mathcal{B}_2}\downarrow&&\downarrow\mathcal{X}_{\mathcal{B}_1}\\
\mathbb{K}^n&\overset{M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})}{\dashrightarrow}&\mathbb{K}^n
\end{array}$$
![[MatriceCambioBase.png]]
> [!abstract] Definizione 23.1 (matrice del cambio di base)
> Date due basi $\mathcal{B}_1$ e $\mathcal{B}_2$ di uno spazio vettoriale $V$, la matrice $M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})$ che rappresenta la funzione identità rispetto a $\mathcal{B}_2$ (dominio) e $\mathcal{B}_1$ (codominio) si dice **matrice del cambio di base da $\mathcal{B}_2$ a $\mathcal{B}_1$**.
![[relazioniMatriciRappresentativeCambiBase.png]]
## Proprietà
- $\mathcal{B}_1\neq\mathcal{B}_2\ \Rightarrow\ M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})\neq\mathrm{Id}_n$.
- $M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})$ è **invertibile** e $\ M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})^{-1}=M_{\mathcal{B}_1}^{\mathcal{B}_2}(\mathrm{id})$.
- Relazioni tra $M_{\mathcal{B}_1}^{\mathcal{C}_1}(L)$ e $M_{\mathcal{B}_1}^{\mathcal{C}_2}(L)$ (stessa base nel dominio, cambia la base nel codominio):
$$M_{\mathcal{B}_1}^{\mathcal{C}_1}(L)=M_{\mathcal{C}_2}^{\mathcal{C}_1}(\mathrm{id})\,M_{\mathcal{B}_1}^{\mathcal{C}_2}(L)$$
$$M_{\mathcal{B}_1}^{\mathcal{C}_2}(L)=M_{\mathcal{C}_2}^{\mathcal{C}_1}(\mathrm{id})^{-1}\,M_{\mathcal{B}_1}^{\mathcal{C}_1}(L)$$

> [!todo] Per casa
> Scrivere tutte le relazioni tra due matrici rappresentative di $L$ (non svolto).

## Note collegate
- [[179_Dimostrazione_del_Primo_Criterio_di_Diagonalizzabilita]]
- [[165_Dipendenza_della_Matrice_Rappresentativa_dalle_Basi]]
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- [[169_Esempio_Cambio_di_Base_per_la_Simmetria_Assiale]]
- [[171_Endomorfismi_e_Matrici_Rappresentative]]
- [[60_Matrice_Invertibile]]
- [[141_Composizione_e_Inversione_di_Applicazioni_Lineari]]
- Indice: [[24_Indice_Lezione_23]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/cambio-di-base
