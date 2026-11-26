---
tags: [GAL, autovalori, autovettori, rotazione, esempio, campo, lezione-26]
data: 2026-11-26
lezione: 26
fonte: "GAL 2026-2027 - 20261126 - LEZIONE 26.pdf (slide 206-207)"
---

# Esempio 2: la rotazione di $\pi/2$ non ha autovalori su $\mathbb{Q}$ e $\mathbb{R}$

$$A=\begin{bmatrix}0&-1\\1&0\end{bmatrix}\in M_{\mathbb{Q}}(2,2)\subseteq M_{\mathbb{R}}(2,2)\subseteq M_{\mathbb{C}}(2,2)$$

> [!question] Cosa fa la matrice $A$?
> In $\mathbb{R}^2$, con $\underline e_1,\underline e_2$ la base canonica: $A\underline e_1=\begin{bmatrix}0\\1\end{bmatrix}=\underline e_2$, $A\underline e_2=\begin{bmatrix}-1\\0\end{bmatrix}=-\underline e_1$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Slide 206.** Piano cartesiano con i vettori $\vec\imath=\underline e_1$ (in rosso, lungo l'asse $x$) e $\vec\jmath=\underline e_2$ (in blu, lungo l'asse $y$); accanto, a destra, i loro trasformati: $A\underline e_1$ (rosso, verso l'alto) e $A\underline e_2$ (blu, verso sinistra). **Da inserire** qui il disegno.

Su $\mathbb{R}$, la matrice $A$ descrive una **rotazione di $\frac\pi2$ in senso antiorario**.

> [!question] Domanda
> Ci sono degli autovettori? Ci sono vettori con un comportamento speciale/semplificato rispetto all'azione di $A$?

$\underline v\ne\underline 0$ è autovettore di $A$ $\iff$ $\underline v\ne\underline 0$ è soluzione di $(A-\lambda\mathrm{Id})\underline x=\underline 0$ per un certo $\lambda$ ([[181_Autovettori_come_Soluzioni_Non_Nulle_del_Sistema_Omogeneo_A_meno_lambda_Id]]), cioè
$$r(A-\lambda\mathrm{Id})<2\iff\det(A-\lambda\mathrm{Id})=0$$
$$\det(A-\lambda\mathrm{Id})=\det\begin{bmatrix}-\lambda&-1\\1&-\lambda\end{bmatrix}=\lambda^2+1$$

- in $\mathbb{Q}$ e $\mathbb{R}$: $\lambda^2+1=0$ **non ha soluzioni** (non ci sono $\lambda$);
- in $\mathbb{C}$: $\lambda=\pm i$ ([[184_Esempio_2_Diagonalizzazione_della_Rotazione_su_C]]).

## Conclusione su $\mathbb{Q}$ e $\mathbb{R}$

Se sono interessato alla diagonalizzabilità su $\mathbb{Q}$ o su $\mathbb{R}$, ho finito la mia ricerca: su $\mathbb{Q}$ o $\mathbb{R}$ **non ci sono autovalori**, quindi **non ci sono autovettori**.

> [!note] Osservazione (non presente negli appunti)
> Per il [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita|primo criterio]], senza autovettori non c'è una base di autovettori: $A$ non è diagonalizzabile né su $\mathbb{Q}$ né su $\mathbb{R}$ (possibilità 3 della tabella in [[175_La_Diagonalizzabilita_Dipende_dal_Campo]]).

## Note collegate
- [[175_La_Diagonalizzabilita_Dipende_dal_Campo]]
- [[184_Esempio_2_Diagonalizzazione_della_Rotazione_su_C]]
- [[185_Definizione_26_1_Polinomio_Caratteristico]]
- Indice: [[27_Indice_Lezione_26]] · [[00_MOC_GAL]]

#GAL/autovalori/rotazione-senza-autovalori
