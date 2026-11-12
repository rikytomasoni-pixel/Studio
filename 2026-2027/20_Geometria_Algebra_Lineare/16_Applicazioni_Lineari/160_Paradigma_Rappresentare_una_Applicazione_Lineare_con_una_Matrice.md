---
tags: [GAL, applicazioni-lineari, paradigma, matrice-associata, coordinate, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 174)"
---

# Paradigma: rappresentare un'applicazione lineare con una matrice

$V,W$ spazi vettoriali finitamente generati, $L:V\to W$ applicazione lineare.
- $\mathcal{B}=\{\underline{v}_1,\dots,\underline{v}_n\}$ base di $V$, $\dim V=n$
- $\mathcal{C}=\{\underline{w}_1,\dots,\underline{w}_m\}$ base di $W$, $\dim W=m$

$$\begin{array}{ccc}
V&\xrightarrow{\ \ L\ \ }&W\\
\mathcal{X}_{\mathcal{B}}\downarrow\uparrow\mathcal{P}_{\mathcal{B}}&&\mathcal{X}_{\mathcal{C}}\downarrow\uparrow\mathcal{P}_{\mathcal{C}}\\
\mathbb{K}^n&\overset{L_A}{\dashrightarrow}&\mathbb{K}^m
\end{array}$$

> [!tip] Idea
> Devo scegliere $A$ affinché i percorsi $\to\downarrow$ (destro, basso) e $\downarrow\to$ (basso, destro) producano lo stesso effetto!

Cioè $L_A$ è l'applicazione $\mathbb{K}^n\to\mathbb{K}^m$ che "imita" $L$ passando dalle coordinate ([[158_Mappa_delle_Coordinate_e_Mappa_di_Parametrizzazione_Definizione_20_6]]). La costruzione di $A$ non è ancora data in questa lezione.

## Note collegate
- [[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]]
- [[159_Esempio_Mappa_di_Parametrizzazione_Polinomi_di_Grado_al_piu_2]]
- [[157_Teorema_20_5_Teorema_di_Isomorfismo_tra_Spazi_Finitamente_Generati]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/paradigma-matrice-associata
