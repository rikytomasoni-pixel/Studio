---
tags: [GAL, polinomio-caratteristico, autovalori, determinante, definizione, lezione-26]
data: 2026-11-26
lezione: 26
fonte: "GAL 2026-2027 - 20261126 - LEZIONE 26.pdf (slide 209)"
---

# Definizione 26.1: polinomio caratteristico

> [!abstract] Definizione 26.1
> Data una matrice $A\in M_{\mathbb{K}}(n,n)$, il polinomio
> $$\chi_A(x)=\det(A-x\,\mathrm{Id})$$
> si dice **polinomio caratteristico** di $A$. L'equazione $\chi_A(x)=0$ si dice **equazione caratteristica** di $A$.

## Osservazioni

- Gli **autovalori** $\in\mathbb{K}$ di $A$ sono le **radici in $\mathbb{K}$** del polinomio $\chi_A(x)$; gli autovalori sono le **soluzioni in $\mathbb{K}$** dell'equazione $\chi_A(x)=0$ ([[181_Autovettori_come_Soluzioni_Non_Nulle_del_Sistema_Omogeneo_A_meno_lambda_Id]]).
- $\chi_A(x)$ è un polinomio di **grado $n$**:
  $$\chi_A(x)=(-1)^nx^n+\dots+\det(A)$$
  $$\chi_A(0)=\det(A-0\,\mathrm{Id})=\det(A)$$
- $\det(A)=0\iff r(A)<n\iff\ker(A)\ne\{\underline 0\}\ \Rightarrow$ ho degli autovettori con autovalore $0$.
- $\det(A)=0\iff\chi_A(x)=x\,q(x)\ \Rightarrow\ \lambda=0$ è radice di $\chi_A(x)$.

## Esempi già visti
- [[182_Esempio_1_Autovettori_di_Autovalore_0_e_Non_Diagonalizzabilita|Esempio 1]]: $\chi_A(x)=x^4$ (unica radice $0$).
- [[183_Esempio_2_Rotazione_senza_Autovalori_su_Q_e_R|Esempio 2]]: $\chi_A(x)=x^2+1$ (nessuna radice in $\mathbb{Q},\mathbb{R}$; $\pm i$ in $\mathbb{C}$).

## Note collegate
- [[186_Definizione_26_2_Molteplicita_Algebrica_Autospazio_Molteplicita_Geometrica]]
- [[190_Proprieta_Preservate_dalla_Similitudine]]
- [[65_Determinante_Sviluppo_di_Laplace]]
- [[63_Rango_di_una_Matrice]]
- Indice: [[27_Indice_Lezione_26]] · [[00_MOC_GAL]]

#GAL/autovalori/polinomio-caratteristico
