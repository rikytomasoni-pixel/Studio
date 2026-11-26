---
tags: [GAL, autovettori, autovalori, endomorfismi, definizione, lezione-25]
data: 2026-11-25
lezione: 25
fonte: "GAL 2026-2027 - 20261125 - LEZIONE 25.pdf (slide 198-199)"
---

# Definizione 25.1: autovettore e autovalore

> [!abstract] Definizione 25.1
> Dato uno spazio vettoriale $V$ su un campo $\mathbb{K}$ e un endomorfismo $L:V\to V$, un vettore $\underline v\ne\underline 0\in V$ si dice **autovettore** di $L$ se esiste $\lambda\in\mathbb{K}$, detto **autovalore** di $\underline v$, tale che
> $$L(\underline v)=\lambda\,\underline v$$

Per una matrice $A\in M_{\mathbb{K}}(n,n)$: gli autovettori di $A$ sono quelli di $L_A:\mathbb{K}^n\to\mathbb{K}^n$, cioè $A\underline v=\lambda\underline v$.

## Esempi

- **Simmetria assiale** ([[167_Simmetria_Assiale_Base_Adattata_e_Matrice_Diagonale]]):
  - $\vec v$ è un autovettore con autovalore $1$;
  - $\vec w$ è un autovettore con autovalore $-1$.
- **$L:V\to V$ non iniettivo** $\Rightarrow\ker(L)\ne\{\underline 0_V\}$ ([[152_Teorema_20_1_Criterio_di_Iniettivita]]). Per ogni $\underline v\ne\underline 0$ in $\ker(L)$: $L(\underline v)=\underline 0=0\cdot\underline v$, quindi $\underline v$ è un autovettore con **autovalore $0$**.
- **Base che diagonalizza**: se $\mathcal{B}=\{\underline v_1,\dots,\underline v_n\}$ è tale che $M_{\mathcal{B}}^{\mathcal{B}}(L)=D=\begin{bmatrix}d_{11}&&0\\&\ddots&\\0&&d_{nn}\end{bmatrix}$, allora per ogni $i=1,\dots,n$ il vettore $\underline v_i$ è un autovettore con autovalore $d_{ii}$ ([[176_Obiettivo_1_Azione_di_L_sulla_Base_Diagonalizzante]]).

## Note collegate
- [[176_Obiettivo_1_Azione_di_L_sulla_Base_Diagonalizzante]]
- [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita]]
- [[151_Nucleo_di_una_Applicazione_Lineare]]
- [[171_Endomorfismi_e_Matrici_Rappresentative]]
- Indice: [[26_Indice_Lezione_25]] · [[00_MOC_GAL]]

#GAL/autovalori/autovettore
