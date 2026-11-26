---
tags: [GAL, diagonalizzabilita, endomorfismi, matrice-diagonale, lezione-25]
data: 2026-11-25
lezione: 25
fonte: "GAL 2026-2027 - 20261125 - LEZIONE 25.pdf (slide 197-198)"
---

# Obiettivo 1: come agisce $L$ sugli elementi di una base che diagonalizza

> [!abstract] Obiettivo 1
> Fornire un'**identikit** di una matrice o di un endomorfismo diagonalizzabile.

Supponiamo di avere un endomorfismo $L:V\to V$ e una base $\mathcal{B}=\{\underline v_1,\dots,\underline v_n\}$ tale che la matrice rappresentativa
$$D=M_{\mathcal{B}}^{\mathcal{B}}(L)$$
sia **diagonale**.

$$\begin{array}{ccc}V&\xrightarrow{\;L\;}&V\\\mathcal{X}_{\mathcal{B}}\downarrow&&\downarrow\mathcal{X}_{\mathcal{B}}\\\mathbb{K}^n&\xrightarrow{\;D\;}&\mathbb{K}^n\end{array}$$

> [!question] Domanda
> Come si comporta $L$ sugli elementi della base $\mathcal{B}$? Per ogni $\underline v_i\in\mathcal{B}$, $L(\underline v_i)=\ ?$

Si usa il diagramma con $\mathcal{X}_{\mathcal{B}}$ in discesa, $D$ in basso e $\mathcal{P}_{\mathcal{B}}$ (mappa di parametrizzazione, inversa di $\mathcal{X}_{\mathcal{B}}$) in risalita:

$$\begin{array}{ccc}\underline v_i\in V&\xrightarrow{\;L\;}&V\\\mathcal{X}_{\mathcal{B}}\downarrow&&\uparrow\mathcal{P}_{\mathcal{B}}\\\mathbb{K}^n&\xrightarrow{\;D\;}&\mathbb{K}^n\end{array}$$

- **Passo 1:** $\mathcal{X}_{\mathcal{B}}(\underline v_i)=\underline e_i=\begin{bmatrix}0\\\vdots\\1\\\vdots\\0\end{bmatrix}$ (1 all'$i$-esima riga).
- **Passo 2:** $D\,\mathcal{X}_{\mathcal{B}}(\underline v_i)=D\underline e_i=\begin{bmatrix}d_{11}&&0\\&\ddots&\\0&&d_{nn}\end{bmatrix}\begin{bmatrix}0\\\vdots\\1\\\vdots\\0\end{bmatrix}=\begin{bmatrix}0\\\vdots\\d_{ii}\\\vdots\\0\end{bmatrix}=d_{ii}\,\underline e_i$
- **Passo 3:** $\mathcal{P}_{\mathcal{B}}\big(D\,\mathcal{X}_{\mathcal{B}}(\underline v_i)\big)=\mathcal{P}_{\mathcal{B}}(d_{ii}\underline e_i)=d_{ii}\,\mathcal{P}_{\mathcal{B}}(\underline e_i)=d_{ii}\,\underline v_i$

> [!success] Risultato
> $$\forall\,\underline v_i\in\mathcal{B}\qquad L(\underline v_i)=d_{ii}\,\underline v_i$$
> **$L$ agisce sugli elementi di $\mathcal{B}$ come un prodotto per uno scalare** (riproporziona i vettori).

## Osservazione: la simmetria assiale

Già nell'esempio della simmetria assiale ([[167_Simmetria_Assiale_Base_Adattata_e_Matrice_Diagonale]]) si osservava questo fenomeno: $L:\mathbb{R}^2\to\mathbb{R}^2$ simmetria, $\mathcal{C}=\{\vec v,\vec w\}$,
$$L(\vec v)=\vec v=1\cdot\vec v\ (d_{11}),\qquad L(\vec w)=-\vec w=(-1)\vec w\ (d_{22}),\qquad M_{\mathcal{C}}^{\mathcal{C}}(L)=\begin{bmatrix}1&0\\0&-1\end{bmatrix}$$

Questa proprietà dà il nome agli [[177_Definizione_25_1_Autovettore_e_Autovalore|autovettori]].

## Note collegate
- [[177_Definizione_25_1_Autovettore_e_Autovalore]]
- [[179_Dimostrazione_del_Primo_Criterio_di_Diagonalizzabilita]]
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- [[158_Mappa_delle_Coordinate_e_Mappa_di_Parametrizzazione_Definizione_20_6]]
- Indice: [[26_Indice_Lezione_25]] · [[00_MOC_GAL]]

#GAL/diagonalizzabilita/azione-sulla-base
