---
tags: [GAL, applicazioni-lineari, suriettivita, matrice-associata, spazio-colonne, rango, lezione-19]
data: 2026-11-11
lezione: 19
fonte: "GAL 2026-2027 - 20261111 - LEZIONE 19.pdf (slide 163-164)"
---

# Suriettività di $L_A$ e spazio delle colonne

$A\in M_{\mathbb{K}}(m,n)$, $L_A:\mathbb{K}^n\to\mathbb{K}^m$.

## Criterio di suriettività
$$\begin{aligned}
L_A\ \text{suriettiva}&\iff \mathrm{im}(L_A)=\mathbb{K}^m\\
&\iff \forall\,\underline{b}\in\mathbb{K}^m\ \exists\,\underline{v}\in\mathbb{K}^n\ \text{t.c.}\ L_A(\underline{v})=\underline{b}\\
&\iff \forall\,\underline{b}\in\mathbb{K}^m\ \exists\,\underline{v}\in\mathbb{K}^n\ \text{t.c.}\ A\underline{v}=\underline{b}\\
&\iff \forall\,\underline{b}\in\mathbb{K}^m\ \text{il sistema}\ A\underline{x}=\underline{b}\ \text{è risolubile}\\
&\iff A\underline{x}=\underline{b}\ \text{risolubile}\ \forall\,\underline{b}\in\mathbb{K}^m\\
&\iff r(A)=m
\end{aligned}$$
(ultimo passaggio: [[82_Teorema_di_Rouche_Capelli]]).

## $\mathrm{im}(L_A)=\mathrm{col}(A)$
Costruiamo un insieme di generatori per $\mathrm{im}(L_A)$ partendo dalla base canonica di $\mathbb{K}^n$, $\{\underline{e}_1,\dots,\underline{e}_n\}$ ([[121_Basi_Canoniche]]), e usando la [[148_Proposizione_19_1_Immagine_dei_Generatori]]:
$$\mathrm{im}(L_A)=\mathrm{Span}\big(L_A(\underline{e}_1),\dots,L_A(\underline{e}_n)\big)=\mathrm{Span}(A\underline{e}_1,\dots,A\underline{e}_n)=\mathrm{Span}\big(C_1(A),\dots,C_n(A)\big)=\mathrm{col}(A)$$
perché
$$L_A(\underline{e}_1)=A\underline{e}_1=\begin{bmatrix}a_{11}&a_{12}&\cdots\\a_{21}&a_{22}&\cdots\\ \vdots&&\\a_{m1}&\cdots&\end{bmatrix}\begin{bmatrix}1\\0\\ \vdots\\0\end{bmatrix}=\begin{bmatrix}a_{11}\\a_{21}\\ \vdots\\a_{m1}\end{bmatrix}=C_1(A)$$
e analogamente $L_A(\underline{e}_2)=A\underline{e}_2=C_2(A)$, $\dots$, $L_A(\underline{e}_n)=A\underline{e}_n=C_n(A)$.

> [!abstract] Morale
> L'immagine di $L_A$ è lo **spazio delle colonne** di $A$: $\mathrm{im}(L_A)=\mathrm{col}(A)$.

## Note collegate
- [[131_Spazio_delle_Righe_e_delle_Colonne]]
- [[149_Conseguenze_della_Suriettivita_Generatori_e_Dimensione]]
- [[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]]
- [[137_Esempi_di_Applicazioni_Lineari_Matrici_Trasposizione_Traccia]]
- [[63_Rango_di_una_Matrice]]
- [[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]
- Indice: [[20_Indice_Lezione_19]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/suriettivita-L_A
