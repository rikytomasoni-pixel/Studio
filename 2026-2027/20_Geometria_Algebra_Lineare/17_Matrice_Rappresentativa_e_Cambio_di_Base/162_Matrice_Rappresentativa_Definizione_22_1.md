---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, definizione, lezione-22]
data: 2026-11-18
lezione: 22
fonte: "GAL 2026-2027 - 20261118 - LEZIONE 22.pdf (slide 178)"
---

# Definizione 22.1 (matrice rappresentativa)

> [!abstract] Definizione 22.1
> Siano $V$ e $W$ due spazi vettoriali su un campo $\mathbb{K}$ con basi $\mathcal{B}=\{\underline{v}_1,\dots,\underline{v}_n\}$ e $\mathcal{C}=\{\underline{w}_1,\dots,\underline{w}_m\}$, e sia $L:V\to W$ un'applicazione lineare.
>
> La **matrice rappresentativa** di $L$ rispetto alle basi $\mathcal{B}$ e $\mathcal{C}$ è l'unica matrice $A\in M_{\mathbb{K}}(m,n)$ tale che
> $$\forall\,\underline{v}\in V\qquad\mathcal{X}_{\mathcal{C}}(L(\underline{v}))=L_A(\mathcal{X}_{\mathcal{B}}(\underline{v}))$$
> ed è definita da
> $$a_{ij}=\text{$i$-esima coordinata rispetto alla base }\mathcal{C}\text{ dell'immagine del $j$-esimo elemento della base }\mathcal{B}.$$

**Notazione:** $A=M_{\mathcal{B}}^{\mathcal{C}}(L)$ (in basso la base del dominio, in alto quella del codominio).

> [!note] Lettura per colonne
> La $j$-esima colonna di $A$ è $\mathcal{X}_{\mathcal{C}}(L(\underline{v}_j))$: è la costruzione ottenuta in [[161_Obiettivo_Costruire_la_Matrice_del_Paradigma]].

## Note collegate
- [[161_Obiettivo_Costruire_la_Matrice_del_Paradigma]]
- [[163_Esempio_Matrice_Rappresentativa_del_Prodotto_a_Sinistra_per_una_Matrice]]
- [[165_Dipendenza_della_Matrice_Rappresentativa_dalle_Basi]]
- [[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]]
- Indice: [[23_Indice_Lezione_22]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/definizione-22-1
