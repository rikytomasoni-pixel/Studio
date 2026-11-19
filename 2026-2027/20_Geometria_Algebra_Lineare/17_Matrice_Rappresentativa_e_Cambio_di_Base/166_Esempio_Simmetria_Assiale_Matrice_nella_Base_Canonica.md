---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, simmetria-assiale, esempio, geometria, lezione-22]
data: 2026-11-18
lezione: 22
fonte: "GAL 2026-2027 - 20261118 - LEZIONE 22.pdf (slide 183-184)"
---

# Esempio: simmetria assiale in $\mathbb{R}^2$, matrice nella base canonica

$L:\mathbb{R}^2\to\mathbb{R}^2$ simmetria assiale rispetto a una retta. Voglio interpretare $L$ come **applicazione lineare**: i punti devono essere interpretati come **vettori**, quindi fisso un'origine $O$ del sistema.

> [!warning] N.B.
> Affinché $L$ sia un'applicazione lineare devo prendere l'origine **appartenente alla retta**.

Voglio una matrice rappresentativa: devo scegliere le basi per descrivere i vettori. Parto con la base canonica, cioè il riferimento cartesiano $\{O,\vec{i},\vec{j}\}$:
$$\mathcal{B}=\{\vec{i},\vec{j}\},\qquad A=M_{\mathcal{B}}^{\mathcal{B}}(L)\in M_{\mathbb{R}}(2,2).$$

$$\begin{array}{ccc}
\mathbb{R}^2&\xrightarrow{\ L\ }&\mathbb{R}^2\\
\mathcal{X}_{\mathcal{B}}\downarrow&&\downarrow\mathcal{X}_{\mathcal{B}}\\
\mathbb{R}^2&\xrightarrow{\ L_A\ }&\mathbb{R}^2
\end{array}\qquad v_x\vec{i}+v_y\vec{j}\ \mapsto\ \begin{bmatrix}v_x\\v_y\end{bmatrix}$$

$$A=\Big[\,\mathcal{X}_{\mathcal{B}}(L(\vec{i}))\,\Big|\,\mathcal{X}_{\mathcal{B}}(L(\vec{j}))\,\Big]$$

La retta forma un angolo $\theta$ con l'asse $x$.

**Vettore $\vec{i}$.** $\vec{i}$ forma un angolo $\theta$ con la retta, quindi $L(\vec{i})$ è $\vec{i}$ ruotato di $2\theta$:
$$L(\vec{i})=1\cdot\cos(2\theta)\,\vec{i}+1\cdot\sin(2\theta)\,\vec{j},\qquad\mathcal{X}_{\mathcal{B}}(L(\vec{i}))=\begin{bmatrix}\cos2\theta\\\sin2\theta\end{bmatrix}.$$

**Vettore $\vec{j}$.** Il vettore $\vec{j}$ forma con la retta un angolo $\pi/2-\theta$ e $L(\vec{j})$ si ottiene con una rotazione di $-2(\pi/2-\theta)$ (angoli orientati):
$$\begin{aligned}L(\vec{j})&=\cos\!\Big(\tfrac{\pi}{2}-2\big(\tfrac{\pi}{2}-\theta\big)\Big)\vec{i}+\sin\!\Big(\tfrac{\pi}{2}-2\big(\tfrac{\pi}{2}-\theta\big)\Big)\vec{j}\\&=\cos\!\big(2\theta-\tfrac{\pi}{2}\big)\vec{i}+\sin\!\big(2\theta-\tfrac{\pi}{2}\big)\vec{j}\\&=\sin(2\theta)\,\vec{i}-\cos(2\theta)\,\vec{j}.\end{aligned}$$

$$\boxed{A=\begin{bmatrix}\cos(2\theta)&\sin(2\theta)\\\sin(2\theta)&-\cos(2\theta)\end{bmatrix}}$$

![[vettoriSpostamentoPerSimmetriaAsse.png]]

> [!warning] DISEGNO NON RAPPRESENTABILE (slide 184)
> Cerca nelle slide: due figure con assi cartesiani e retta blu inclinata di $\theta$. Prima figura: $\vec{i}$ (rosso) e $L(\vec{i})$ (verde), con gli angoli $\theta$ indicati in viola. Seconda figura: $\vec{j}$ (rosso) e $L(\vec{j})$ (verde), con la rotazione $-(\pi/2-\theta)$ indicata due volte in viola.

## Note collegate
- [[165_Dipendenza_della_Matrice_Rappresentativa_dalle_Basi]]
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- [[167_Simmetria_Assiale_Base_Adattata_e_Matrice_Diagonale]]
- [[169_Esempio_Cambio_di_Base_per_la_Simmetria_Assiale]]
- [[23_Sistemi_di_Riferimento_e_Coordinate]]
- Indice: [[23_Indice_Lezione_22]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/simmetria-assiale
