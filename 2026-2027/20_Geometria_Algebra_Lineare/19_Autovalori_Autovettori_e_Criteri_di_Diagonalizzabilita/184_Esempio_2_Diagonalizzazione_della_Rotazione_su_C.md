---
tags: [GAL, autovalori, autovettori, diagonalizzabilita, rotazione, numeri-complessi, esempio, lezione-26]
data: 2026-11-26
lezione: 26
fonte: "GAL 2026-2027 - 20261126 - LEZIONE 26.pdf (slide 207-208)"
---

# Esempio 2: diagonalizzare la rotazione come matrice su $\mathbb{C}$

Proviamo a diagonalizzare $A=\begin{bmatrix}0&-1\\1&0\end{bmatrix}$ come matrice su $\mathbb{C}$. Su $\mathbb{C}$ i due autovalori possibili sono $\lambda_1=i$, $\lambda_2=-i$ ([[183_Esempio_2_Rotazione_senza_Autovalori_su_Q_e_R]]).

## Autovalore $\lambda_1=i$: $(A-i\,\mathrm{Id})\underline x=\underline 0$

$$A-i\mathrm{Id}=\begin{bmatrix}-i&-1\\1&-i\end{bmatrix}$$
N.B.: so a priori che $r(A-i\mathrm{Id})<2$, quindi una riga è ridondante. Resta $x_1-ix_2=0$ con $x_2=t$ libero:
$$\ker(A-i\mathrm{Id})=\mathrm{Span}\left(\begin{bmatrix}i\\1\end{bmatrix}\right)\subseteq\mathbb{C}^2$$

## Autovalore $\lambda_2=-i$: $(A+i\,\mathrm{Id})\underline x=\underline 0$

$$A+i\mathrm{Id}=\begin{bmatrix}i&-1\\1&i\end{bmatrix}$$
Anche qui $r(A+i\mathrm{Id})<2$; resta $x_1+ix_2=0$ con $x_2=t$ libero:
$$\ker(A+i\mathrm{Id})=\mathrm{Span}\left(\begin{bmatrix}-i\\1\end{bmatrix}\right)\subseteq\mathbb{C}^2$$

> [!info] Osservazione
> Ho esaurito la ricerca degli autovettori.

## $A$ è diagonalizzabile su $\mathbb{C}$

Per il [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita|primo criterio]], $A$ è diagonalizzabile su $\mathbb{C}$ se la collezione di autovettori trovata forma una base di $\mathbb{C}^2$:
$$\mathcal{B}=\left\{\begin{bmatrix}i\\1\end{bmatrix}\right\}\cup\left\{\begin{bmatrix}-i\\1\end{bmatrix}\right\}$$
$\mathcal{B}$ è una base perché i due vettori **non sono proporzionali**.

$$\begin{array}{ccc}\mathbb{C}^2&\xrightarrow{\;A\;}&\mathbb{C}^2\\P\uparrow&&\uparrow P\\\mathbb{C}^2&\xrightarrow{\;D\;}&\mathbb{C}^2\end{array}$$

con $\mathcal{E}=\{\underline e_1,\underline e_2\}$ base canonica e $\mathcal{B}$ base di autovettori:
$$D=M_{\mathcal{B}}^{\mathcal{B}}(L_A)=\begin{bmatrix}i&0\\0&-i\end{bmatrix},\qquad P=M_{\mathcal{B}}^{\mathcal{E}}(\mathrm{id})=\begin{bmatrix}i&-i\\1&1\end{bmatrix}$$
(le colonne di $P$ sono i vettori della base di autovettori espressi nella base canonica; le colonne di $D$ sono le coordinate di $L_A$ sui due autovettori.)

Verifica delle colonne di $D$:
$$L_A\left(\begin{bmatrix}i\\1\end{bmatrix}\right)=A\begin{bmatrix}i\\1\end{bmatrix}=(i\mathrm{Id})\begin{bmatrix}i\\1\end{bmatrix}=i\begin{bmatrix}i\\1\end{bmatrix}=i\begin{bmatrix}i\\1\end{bmatrix}+0\begin{bmatrix}-i\\1\end{bmatrix}$$
$$L_A\left(\begin{bmatrix}-i\\1\end{bmatrix}\right)=A\begin{bmatrix}-i\\1\end{bmatrix}=(-i\mathrm{Id})\begin{bmatrix}-i\\1\end{bmatrix}=(-i)\begin{bmatrix}-i\\1\end{bmatrix}=0\begin{bmatrix}i\\1\end{bmatrix}+(-i)\begin{bmatrix}-i\\1\end{bmatrix}$$

Quindi $A$ è diagonalizzabile su $\mathbb{C}$ ma non su $\mathbb{Q}$, $\mathbb{R}$: è la possibilità 3 di [[175_La_Diagonalizzabilita_Dipende_dal_Campo]].

## Note collegate
- [[183_Esempio_2_Rotazione_senza_Autovalori_su_Q_e_R]]
- [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita]]
- [[168_Matrice_del_Cambio_di_Base_Definizione_23_1]]
- [[13_Numeri_Complessi]] (in `AM1`, unità immaginaria)
- Indice: [[27_Indice_Lezione_26]] · [[00_MOC_GAL]]

#GAL/autovalori/rotazione-su-C
