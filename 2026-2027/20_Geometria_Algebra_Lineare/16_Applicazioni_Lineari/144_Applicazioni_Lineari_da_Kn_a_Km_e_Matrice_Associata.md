---
tags: [GAL, applicazioni-lineari, matrice-associata, base-canonica, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 154-155)"
---

# Esempio 2: applicazioni lineari $\mathbb{K}^n\to\mathbb{K}^m$ e matrice associata

Caso generale $L:\mathbb{K}^n\to\mathbb{K}^m$.

**D.** Come definisco $L$?
- Scelgo una base del dominio: $\mathcal{B}=\{\underline{e}_1,\dots,\underline{e}_n\}$ ([[121_Basi_Canoniche|base canonica]]).
- Scelgo l'immagine dei vettori di $\mathcal{B}$: $L(\underline{e}_1)=\underline{w}_1,\ L(\underline{e}_2)=\underline{w}_2,\ \dots,\ L(\underline{e}_n)=\underline{w}_n$.

**Qual è l'immagine di un vettore $\underline{v}\in\mathbb{K}^n$ arbitrario?**
$$\underline{v}=\begin{bmatrix}v_1\\\vdots\\v_n\end{bmatrix}=v_1\underline{e}_1+v_2\underline{e}_2+\dots+v_n\underline{e}_n$$
$$L(\underline{v})=L(v_1\underline{e}_1+\dots+v_n\underline{e}_n)=v_1L(\underline{e}_1)+\dots+v_nL(\underline{e}_n)=v_1\underline{w}_1+v_2\underline{w}_2+\dots+v_n\underline{w}_n$$
Questa è una combinazione lineare, "assomiglia" alla rappresentazione del I tipo di un sistema; riscritta come prodotto matrice-vettore "assomiglia" alla rappresentazione del II tipo ([[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]):
$$=\begin{bmatrix}\underline{w}_1\,\Big|\,\dots\,\Big|\,\underline{w}_n\end{bmatrix}\begin{bmatrix}v_1\\\vdots\\v_n\end{bmatrix}=A\underline{v}=L_A(\underline{v}),\qquad A=\begin{bmatrix}\underline{w}_1\,\Big|\,\dots\,\Big|\,\underline{w}_n\end{bmatrix}\in M_{\mathbb{K}}(m,n)$$

> [!abstract] Morale
> **Tutte** le applicazioni lineari da $\mathbb{K}^n$ a $\mathbb{K}^m$ sono codificate come $L_A$, con $A\in M_{\mathbb{K}}(m,n)$: la colonna $j$-esima di $A$ è $L(\underline{e}_j)$.

## Note collegate
- [[142_Come_Definire_una_Applicazione_Lineare_Proposizione_17_2]]
- [[137_Esempi_di_Applicazioni_Lineari_Matrici_Trasposizione_Traccia]] (esempio (I): $L_A$)
- [[141_Composizione_e_Inversione_di_Applicazioni_Lineari]]
- [[121_Basi_Canoniche]]
- [[30_Matrici_come_Rappresentazione_di_Funzioni]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/matrice-associata
