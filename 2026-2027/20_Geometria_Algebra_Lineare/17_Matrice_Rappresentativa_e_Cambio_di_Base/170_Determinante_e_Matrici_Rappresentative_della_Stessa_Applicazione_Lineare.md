---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, determinante, binet, cambio-di-base, lezione-23]
data: 2026-11-19
lezione: 23
fonte: "GAL 2026-2027 - 20261119 - LEZIONE 23.pdf (slide 191)"
---

# Determinante e matrici rappresentative della stessa applicazione lineare

Dall'esempio [[169_Esempio_Cambio_di_Base_per_la_Simmetria_Assiale]]: $A=P\,B\,P^{-1}$.

> [!question] Osservazione
> Cosa si può dire di $\det(A)$ e $\det(B)$?

$$\begin{aligned}\det(A)&=\det(PBP^{-1})\overset{\text{TEO Binet}}{=}\det(P)\det(B)\det(P^{-1})\qquad(\text{prodotto in }\mathbb{K})\\&=\det(B)\det(P)\det(P^{-1})\\&\overset{\text{TEO Binet}}{=}\det(B)\det(PP^{-1})=\det(B)\det(\mathrm{Id}_n)\\&=\det(B)\end{aligned}$$

> [!abstract] Conclusione
> - $A,B$ rappresentano entrambe la stessa applicazione lineare (rispetto a basi diverse) $\ \Rightarrow\ \det(A)=\det(B)$.
> - $A,B$ **non** rappresentano la stessa applicazione lineare rispetto a basi diverse $\ \Leftarrow\ \det(A)\neq\det(B)$.

## Note collegate
- [[74_Teorema_di_Binet]]
- [[169_Esempio_Cambio_di_Base_per_la_Simmetria_Assiale]]
- [[168_Matrice_del_Cambio_di_Base_Definizione_23_1]]
- [[172_Matrici_Simili_Definizione_23_2]]
- Indice: [[24_Indice_Lezione_23]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/determinante
