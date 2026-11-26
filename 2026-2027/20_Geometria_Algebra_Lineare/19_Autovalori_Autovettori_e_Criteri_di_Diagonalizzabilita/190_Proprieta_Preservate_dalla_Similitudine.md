---
tags: [GAL, matrici-simili, similitudine, determinante, rango, traccia, polinomio-caratteristico, lezione-26]
data: 2026-11-26
lezione: 26
fonte: "GAL 2026-2027 - 20261126 - LEZIONE 26.pdf (slide 213-214)"
---

# Proprietà preservate dalla similitudine

> [!question] Domanda
> Perché abbiamo usato il termine "**similitudine**" tra matrici? In cosa si assomigliano le matrici simili ([[172_Matrici_Simili_Definizione_23_2]])?

> [!abstract] Proprietà comuni
> Se $A,B\in M_{\mathbb{K}}(n,n)$ sono **simili**:
> - $\det(A)=\det(B)$ ([[170_Determinante_e_Matrici_Rappresentative_della_Stessa_Applicazione_Lineare]])
> - $r(A)=r(B)$
> - $\chi_A(x)=\chi_B(x)$
> - $\mathrm{tr}(A)=\mathrm{tr}(B)$
> - $A$ e $B$ hanno **gli stessi autovalori con le stesse molteplicità**

## Se $A$ è diagonalizzabile

Sia $A\in M_{\mathbb{K}}(n,n)$ diagonalizzabile su $\mathbb{K}$ e $D=\begin{bmatrix}d_{11}&&0\\&\ddots&\\0&&d_{nn}\end{bmatrix}$ una matrice diagonale simile ad $A$ (le $d_{ii}$ sono gli autovalori $\lambda_i$ di $A$). Allora:

- $r(A)=r(D)=\#\text{autovalori}\ne0$
- $\det(A)=\det(D)=d_{11}d_{22}\cdots d_{nn}=\lambda_1\lambda_2\cdots\lambda_n$
- $\mathrm{tr}(A)=\mathrm{tr}(D)=d_{11}+d_{22}+\dots+d_{nn}=\lambda_1+\dots+\lambda_n$

## Esempio $n=2$

$A=\begin{bmatrix}0&-1\\1&0\end{bmatrix}$:
$$\lambda_1\lambda_2=1,\qquad\lambda_1+\lambda_2=0$$
Gli autovalori sono le radici di $x^2-(\lambda_1+\lambda_2)x+\lambda_1\lambda_2=0$, cioè di
$$x^2+1=0$$
che è proprio $\chi_A(x)=0$ ([[183_Esempio_2_Rotazione_senza_Autovalori_su_Q_e_R]], [[184_Esempio_2_Diagonalizzazione_della_Rotazione_su_C]]).

## Note collegate
- [[172_Matrici_Simili_Definizione_23_2]]
- [[173_La_Similitudine_tra_Matrici_e_una_Relazione_di_Equivalenza]]
- [[185_Definizione_26_1_Polinomio_Caratteristico]]
- [[137_Esempi_di_Applicazioni_Lineari_Matrici_Trasposizione_Traccia]] (traccia)
- Indice: [[27_Indice_Lezione_26]] · [[00_MOC_GAL]]

#GAL/matrici/proprieta-similitudine
