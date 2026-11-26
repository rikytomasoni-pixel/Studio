---
tags: [GAL, diagonalizzabilita, autovettori, dimostrazione, lezione-25]
data: 2026-11-25
lezione: 25
fonte: "GAL 2026-2027 - 20261125 - LEZIONE 25.pdf (slide 199-200)"
---

# Dimostrazione del primo criterio di diagonalizzabilità

Teorema: [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita]]. Qui $\mathcal{E}=\{\underline e_1,\dots,\underline e_n\}$ è la base canonica di $\mathbb{K}^n$.

## (I) $\Rightarrow$ (II)

**Ipotesi:** $A$ diagonalizzabile. Esiste un cambio di base $P$ tale che $P^{-1}AP=D$ diagonale.

$$\begin{array}{ccc}\mathbb{K}^n&\xrightarrow{\;A\;}&\mathbb{K}^n\\P\uparrow&&\uparrow P\\\mathbb{K}^n&\xrightarrow{\;D\;}&\mathbb{K}^n\end{array}$$

Sia $\mathcal{B}=\{\underline v_1,\dots,\underline v_n\}$ la base data da $P$, con $P=M_{\mathcal{B}}^{\mathcal{E}}(\mathrm{id})$ ([[168_Matrice_del_Cambio_di_Base_Definizione_23_1]]). Calcolo $A\underline v_i$:
$$A\underline v_i=L_A(\underline v_i)=M_{\mathcal{B}}^{\mathcal{B}}(L_A)\,\mathcal{X}_{\mathcal{B}}(\underline v_i)=D\begin{bmatrix}0\\\vdots\\1\\\vdots\\0\end{bmatrix}=d_{ii}\,\underline v_i$$
perché $\underline v_i=0\underline v_1+\dots+1\underline v_i+\dots+0\underline v_n$, cioè $\mathcal{X}_{\mathcal{B}}(\underline v_i)=\underline e_i$.

Quindi $\{\underline v_1,\dots,\underline v_n\}$ è una **base di autovettori** di $A$ (con autovalori $d_{ii}$).

## (II) $\Rightarrow$ (I)

**Ipotesi:** esiste una base $\mathcal{B}=\{\underline v_1,\dots,\underline v_n\}$ di $\mathbb{K}^n$ formata da autovettori di $A$. Per ogni $i=1,\dots,n$
$$A\underline v_i=L_A(\underline v_i)=\lambda_i\underline v_i\qquad\lambda_i\in\mathbb{K}$$
Allora le colonne di $M_{\mathcal{B}}^{\mathcal{B}}(L_A)$ sono le coordinate di $L_A(\underline v_i)$ rispetto a $\mathcal{B}$:
$$L_A(\underline v_1)=\lambda_1\underline v_1=\lambda_1\underline v_1+0\underline v_2+\dots+0\underline v_n,\quad L_A(\underline v_2)=\lambda_2\underline v_2=0\underline v_1+\lambda_2\underline v_2+\dots+0\underline v_n,\ \dots$$
$$M_{\mathcal{B}}^{\mathcal{B}}(L_A)=\begin{bmatrix}\lambda_1&&0\\&\ddots&\\0&&\lambda_n\end{bmatrix}$$
$L_A$ ha una **rappresentazione diagonale**. $\square$

## Note collegate
- [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita]]
- [[168_Matrice_del_Cambio_di_Base_Definizione_23_1]]
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- [[176_Obiettivo_1_Azione_di_L_sulla_Base_Diagonalizzante]]
- Indice: [[26_Indice_Lezione_25]] · [[00_MOC_GAL]]

#GAL/diagonalizzabilita/dimostrazione-primo-criterio
