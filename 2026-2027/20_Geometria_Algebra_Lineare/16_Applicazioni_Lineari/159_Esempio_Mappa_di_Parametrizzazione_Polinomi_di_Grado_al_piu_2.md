---
tags: [GAL, applicazioni-lineari, isomorfismo, parametrizzazione, polinomi, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 174)"
---

# Esempio: mappa di parametrizzazione di $\mathbb{K}[t]_{\le2}$

$V=\mathbb{K}[t]_{\le2}$, $\dim\mathbb{K}[t]_{\le2}=3$, $\mathcal{B}=\{1,t,t^2\}$ ($\mathbb{K}[t]_{\le2}$ è isomorfo a $\mathbb{K}^3$).

$\mathcal{P}_{\mathcal{B}}:\mathbb{K}^3\to\mathbb{K}[t]_{\le2}$:
$$\mathcal{P}_{\mathcal{B}}(\underline{e}_1)=1,\qquad\mathcal{P}_{\mathcal{B}}(\underline{e}_2)=t,\qquad\mathcal{P}_{\mathcal{B}}(\underline{e}_3)=t^2$$
$$\begin{bmatrix}x\\y\\z\end{bmatrix}=x\,\underline{e}_1+y\,\underline{e}_2+z\,\underline{e}_3\ \xmapsto{\ \mathcal{P}_{\mathcal{B}}\ }\ x\cdot1+y\cdot t+z\cdot t^2=x+yt+zt^2$$

La mappa di parametrizzazione "inserisce" le componenti come coefficienti nella base scelta; la mappa delle coordinate fa il percorso inverso ([[158_Mappa_delle_Coordinate_e_Mappa_di_Parametrizzazione_Definizione_20_6]]).

## Note collegate
- [[160_Paradigma_Rappresentare_una_Applicazione_Lineare_con_una_Matrice]]
- [[143_Esempio_Applicazione_Lineare_da_Polinomi_a_Matrici]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/mappa-parametrizzazione
