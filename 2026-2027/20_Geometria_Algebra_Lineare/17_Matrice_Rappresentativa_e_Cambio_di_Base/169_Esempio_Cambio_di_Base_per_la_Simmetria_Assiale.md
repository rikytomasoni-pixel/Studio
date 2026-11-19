---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, cambio-di-base, simmetria-assiale, esempio, lezione-23]
data: 2026-11-19
lezione: 23
fonte: "GAL 2026-2027 - 20261119 - LEZIONE 23.pdf (slide 190-191)"
---

# Esempio: cambio di base per la simmetria assiale

Esempio in $\mathbb{R}^2$ (simmetria assiale, vedi [[166_Esempio_Simmetria_Assiale_Matrice_nella_Base_Canonica]] e [[167_Simmetria_Assiale_Base_Adattata_e_Matrice_Diagonale]]):
$$\mathcal{B}=\{\vec{i},\vec{j}\}:\ A=\begin{bmatrix}\cos2\theta&\sin2\theta\\\sin2\theta&-\cos2\theta\end{bmatrix}\qquad\mathcal{C}=\{\vec{v},\vec{w}\}:\ B=\begin{bmatrix}1&0\\0&-1\end{bmatrix}$$

**Domanda:** $M_{\mathcal{C}}^{\mathcal{B}}(\mathrm{id})=\ ?$

> [!warning] N.B.
> È preferibile scrivere le matrici del cambio di base usando le **basi canoniche come basi in arrivo**.

$$M_{\mathcal{C}}^{\mathcal{B}}(\mathrm{id})=\Big[\,\mathrm{id}(\vec{v})\,\Big|\,\mathrm{id}(\vec{w})\,\Big]\in M_{\mathbb{R}}(2,2)\qquad(\text{righe: }\vec{i},\vec{j}).$$

- $\vec{v}$ forma un angolo $\theta$ con l'asse $x$: $\vec{v}=(\cos\theta)\vec{i}+(\sin\theta)\vec{j}$, $\ \mathcal{X}_{\mathcal{B}}(\vec{v})=\begin{bmatrix}\cos\theta\\\sin\theta\end{bmatrix}$.
- $\vec{w}$ è ruotato di $\pi/2$ rispetto a $\vec{v}$: $\vec{w}=\cos(\theta+\tfrac{\pi}{2})\vec{i}+\sin(\theta+\tfrac{\pi}{2})\vec{j}$, $\ \mathcal{X}_{\mathcal{B}}(\vec{w})=\begin{bmatrix}\cos(\theta+\frac{\pi}{2})\\\sin(\theta+\frac{\pi}{2})\end{bmatrix}$.

$$P=M_{\mathcal{C}}^{\mathcal{B}}(\mathrm{id})=\begin{bmatrix}\cos\theta&\cos(\theta+\frac{\pi}{2})\\\sin\theta&\sin(\theta+\frac{\pi}{2})\end{bmatrix}=\begin{bmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{bmatrix}$$

> [!warning] DISEGNO NON RAPPRESENTABILE (slide 190)
> Cerca nelle slide: due figure con assi cartesiani e retta blu inclinata di $\theta$. Prima: $\vec{v}$ (viola) lungo la retta con angolo $\theta$. Seconda: $\vec{w}$ (viola) con l'arco verde che indica la rotazione $\pi/2$ rispetto alla retta e l'angolo $\theta$.

## Diagramma di cambio di base

> [!warning] DISEGNO NON RAPPRESENTABILE (slide 190, in basso; completato in slide 191)
> Cerca nelle slide: diagramma con $\mathbb{R}^2\xrightarrow{L}\mathbb{R}^2$ in alto, $\mathcal{X}_{\mathcal{C}}$ e $\mathcal{X}_{\mathcal{B}}$ che scendono su ciascun lato. Sotto: la freccia orizzontale verde $B$ tra le due copie di $\mathbb{R}^2$ in coordinate $\mathcal{C}$; due frecce blu $P$ (una per lato) che portano da coordinate $\mathcal{C}$ a coordinate $\mathcal{B}$; la freccia viola $A$ in basso tra le due copie in coordinate $\mathcal{B}$.

Dal diagramma (si va da coordinate $\mathcal{B}$ a coordinate $\mathcal{C}$ con $P^{-1}$, si applica $B$, si torna con $P$):
$$\boxed{A=P\,B\,P^{-1}}$$

## Note collegate
- [[168_Matrice_del_Cambio_di_Base_Definizione_23_1]]
- [[170_Determinante_e_Matrici_Rappresentative_della_Stessa_Applicazione_Lineare]]
- [[167_Simmetria_Assiale_Base_Adattata_e_Matrice_Diagonale]]
- [[166_Esempio_Simmetria_Assiale_Matrice_nella_Base_Canonica]]
- [[172_Matrici_Simili_Definizione_23_2]]
- Indice: [[24_Indice_Lezione_23]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/esempio-cambio-di-base
