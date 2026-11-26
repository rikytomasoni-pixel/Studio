---
tags: [GAL, autovettori, nucleo, diagonalizzabilita, esempio, polinomi, lezione-25]
data: 2026-11-25
lezione: 25
fonte: "GAL 2026-2027 - 20261125 - LEZIONE 25.pdf (slide 204)"
---

# Esempio 1: gli autovettori di autovalore $0$ e la non diagonalizzabilità

Per $L(p)=tp''-p'$ su $\mathbb{K}[t]_{\le3}$ ([[180_Obiettivo_Concreto_Ricerca_degli_Autovettori_e_Esempio_1]]) l'unico autovalore possibile è $\lambda=0$ ([[181_Autovettori_come_Soluzioni_Non_Nulle_del_Sistema_Omogeneo_A_meno_lambda_Id]]). Fisso $\lambda=0$ e risolvo il sistema
$$\ker(A-0\,\mathrm{Id})=\ker(A)$$

> [!info] Osservazione
> Gli autovettori con autovalore $\lambda=0$ sono (sempre) gli **elementi non nulli del nucleo**.

## Calcolo del nucleo

Dalla matrice $A=\begin{bmatrix}0&-1&0&0\\0&0&0&0\\0&0&0&3\\0&0&0&0\end{bmatrix}$ si eliminano le righe nulle e si riscalano le altre, ottenendo $\begin{bmatrix}0&1&0&0\\0&0&0&1\end{bmatrix}$: le componenti $a_1$ e $a_3$ sono nulle, mentre $a_0$ e $a_2$ sono libere (parametri $s_1,s_2$). Quindi
$$\ker(A)=\mathrm{Span}\left(\begin{bmatrix}1\\0\\0\\0\end{bmatrix},\begin{bmatrix}0\\0\\1\\0\end{bmatrix}\right)$$

Gli autovettori di $L$ sono (con $\mathcal{P}_{\mathcal{B}}$ la mappa di parametrizzazione):
$$\mathcal{P}_{\mathcal{B}}\left(\begin{bmatrix}1\\0\\0\\0\end{bmatrix}\right)=1\ (\underline e_1),\qquad\mathcal{P}_{\mathcal{B}}\left(\begin{bmatrix}0\\0\\1\\0\end{bmatrix}\right)=t^2\ (\underline e_3)$$

> [!info] Osservazione
> Non ci sono altri autovettori di $L$ con $\lambda=0$ linearmente indipendenti da questi.

## Conclusione

Ho trovato **tutti** gli autovettori possibili. Per il [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita|primo criterio]], $L$ sarebbe diagonalizzabile se ci fosse una base di $\mathbb{K}^4$ formata da autovettori di $A$. Ne ho trovati solo **2** linearmente indipendenti:

> [!failure] $A$ **non è diagonalizzabile** (indipendentemente da $\mathbb{K}$, in questo caso)

> [!note] Osservazione (non presente negli appunti)
> In termini di [[186_Definizione_26_2_Molteplicita_Algebrica_Autospazio_Molteplicita_Geometrica|molteplicità]] (L26): qui $a_0=4$ ma $g_0=2<4$, quindi non vale il [[188_Teorema_26_3_Secondo_Criterio_di_Diagonalizzabilita|secondo criterio]].

## Note collegate
- [[180_Obiettivo_Concreto_Ricerca_degli_Autovettori_e_Esempio_1]]
- [[181_Autovettori_come_Soluzioni_Non_Nulle_del_Sistema_Omogeneo_A_meno_lambda_Id]]
- [[151_Nucleo_di_una_Applicazione_Lineare]]
- [[158_Mappa_delle_Coordinate_e_Mappa_di_Parametrizzazione_Definizione_20_6]]
- Indice: [[26_Indice_Lezione_25]] · [[00_MOC_GAL]]

#GAL/autovalori/esempio-non-diagonalizzabile
