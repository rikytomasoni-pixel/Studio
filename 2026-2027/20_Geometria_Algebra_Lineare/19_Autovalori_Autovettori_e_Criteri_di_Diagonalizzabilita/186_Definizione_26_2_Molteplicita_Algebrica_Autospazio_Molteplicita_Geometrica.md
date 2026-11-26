---
tags: [GAL, autovalori, autospazio, molteplicita, definizione, lezione-26]
data: 2026-11-26
lezione: 26
fonte: "GAL 2026-2027 - 20261126 - LEZIONE 26.pdf (slide 210)"
---

# Definizione 26.2: molteplicità algebrica, autospazio, molteplicità geometrica

> [!abstract] Definizione 26.2
> Data una matrice $A\in M_{\mathbb{K}}(n,n)$, sia $\lambda\in\mathbb{K}$ un autovalore.
> - La **molteplicità algebrica** di $\lambda$ è
>   $$a_\lambda=\max\{k\mid(x-\lambda)^k\text{ divide }\chi_A(x)\}$$
> - L'**autospazio** di $A$ associato a $\lambda$ è il sottospazio vettoriale
>   $$V_\lambda=\ker(A-\lambda\mathrm{Id})=\{\underline v\in\mathbb{K}^n\mid A\underline v=\lambda\underline v\}=\{\underline 0\}\cup\{\text{autovettori di }A\text{ con autovalore }\lambda\}$$
>   ($V_\lambda$ è lo spazio vettoriale degli autovettori con autovalore $\lambda$.)
> - La **molteplicità geometrica** di $\lambda$ è
>   $$g_\lambda=\dim V_\lambda=\dim\ker(A-\lambda\mathrm{Id})=n-r(A-\lambda\mathrm{Id})$$

## Osservazioni

- Nell'esempio di $L(p(t))=tp''(t)-p'(t)$ ([[182_Esempio_1_Autovettori_di_Autovalore_0_e_Non_Diagonalizzabilita]]): $\chi_A(x)=x^4$, c'è una sola radice $\lambda=0$ e
  - $a_0=4$
  - $V_0=\mathrm{Span}\left(\begin{bmatrix}1\\0\\0\\0\end{bmatrix},\begin{bmatrix}0\\0\\1\\0\end{bmatrix}\right)$
  - $g_0=2$
- **(Fatto)** $\quad1\le g_\lambda\le a_\lambda$

> [!warning] Differenza rispetto al quaderno
> Nella slide 210 il secondo vettore di $V_0$ è scritto in modo poco leggibile (l'ultima entrata sembra un $3$); l'ho trascritto $\begin{bmatrix}0\\0\\1\\0\end{bmatrix}$ per coerenza con il calcolo del nucleo in [[182_Esempio_1_Autovettori_di_Autovalore_0_e_Non_Diagonalizzabilita]]. Da controllare sulla slide.

## Note collegate
- [[185_Definizione_26_1_Polinomio_Caratteristico]]
- [[187_Autospazi_di_Autovalori_Distinti_e_Somma_Diretta]]
- [[189_Autovalori_Semplici_e_Regolari]]
- [[151_Nucleo_di_una_Applicazione_Lineare]]
- [[164_Teorema_22_2_Teorema_di_Nullita_piu_Rango]]
- Indice: [[27_Indice_Lezione_26]] · [[00_MOC_GAL]]

#GAL/autovalori/molteplicita-autospazio
