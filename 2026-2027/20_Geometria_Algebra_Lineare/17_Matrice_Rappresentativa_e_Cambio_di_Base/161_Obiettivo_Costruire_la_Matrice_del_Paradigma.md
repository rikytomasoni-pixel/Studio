---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, coordinate, paradigma, lezione-22]
data: 2026-11-18
lezione: 22
fonte: "GAL 2026-2027 - 20261118 - LEZIONE 22.pdf (slide 176-177)"
---

# Obiettivo: costruire la matrice del paradigma

## Riepilogo e idea
- Tutte le applicazioni lineari da $\mathbb{K}^n$ a $\mathbb{K}^m$ sono descrivibili mediante una matrice in $M_{\mathbb{K}}(m,n)$ ([[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]]).
- Tutti gli spazi vettoriali finitamente generati hanno un "gemello" (isomorfismo) con $\mathbb{K}^n$ ([[157_Teorema_20_5_Teorema_di_Isomorfismo_tra_Spazi_Finitamente_Generati]]).

> [!tip] Idea
> Usare le matrici per studiare **tutte** le applicazioni lineari tra spazi vettoriali finitamente generati.

## Paradigma
$V,W$ spazi vettoriali finitamente generati su un campo $\mathbb{K}$, $L:V\to W$ applicazione lineare, $\mathcal{B}=\{\underline{v}_1,\dots,\underline{v}_n\}$ base di $V$ ($\dim V=n$), $\mathcal{C}=\{\underline{w}_1,\dots,\underline{w}_m\}$ base di $W$ ($\dim W=m$).

$$\begin{array}{ccc}
V&\xrightarrow{\ \ L\ \ }&W\\
\mathcal{X}_{\mathcal{B}}\downarrow\uparrow\mathcal{P}_{\mathcal{B}}&&\mathcal{X}_{\mathcal{C}}\downarrow\uparrow\mathcal{P}_{\mathcal{C}}\\
\mathbb{K}^n&\overset{L_A}{\dashrightarrow}&\mathbb{K}^m
\end{array}$$

> [!abstract] Obiettivo
> Determinare una matrice $A\in M_{\mathbb{K}}(m,n)$ tale che
> $$\forall\,\underline{v}\in V\qquad L(\underline{v})=\mathcal{P}_{\mathcal{C}}\big(L_A(\mathcal{X}_{\mathcal{B}}(\underline{v}))\big),\qquad\text{cioè}\qquad L=\mathcal{P}_{\mathcal{C}}\circ L_A\circ\mathcal{X}_{\mathcal{B}}.$$

## Come raggiungiamo l'obiettivo
Ricordo che $\mathcal{P}_{\mathcal{C}}$ è l'applicazione inversa di $\mathcal{X}_{\mathcal{C}}$. Quindi
$$L=\mathcal{P}_{\mathcal{C}}\circ L_A\circ\mathcal{X}_{\mathcal{B}}\iff\mathcal{X}_{\mathcal{C}}\circ L=L_A\circ\mathcal{X}_{\mathcal{B}}.$$

> [!note] Osservazione
> Nelle colonne della matrice $A$ compaiono le immagini dei vettori della base canonica di $\mathbb{K}^n$:
> $$A=\big[\,L_A(\underline{e}_1)\,\big|\,L_A(\underline{e}_2)\,\big|\,\dots\,\big|\,L_A(\underline{e}_n)\,\big].$$

Considero i vettori $\underline{v}_i$ della base $\mathcal{B}$ e impongo $\mathcal{X}_{\mathcal{C}}\circ L(\underline{v}_i)=L_A\circ\mathcal{X}_{\mathcal{B}}(\underline{v}_i)$, con membro sinistro (I) e destro (II).

- (II) $L_A\circ\mathcal{X}_{\mathcal{B}}(\underline{v}_i)=L_A(\mathcal{X}_{\mathcal{B}}(\underline{v}_i))=A\,\mathcal{X}_{\mathcal{B}}(\underline{v}_i)=A\,\underline{e}_i$ = **$i$-esima colonna di $A$** (perché $\mathcal{X}_{\mathcal{B}}(\underline{v}_i)=\underline{e}_i$).
- (I) $\mathcal{X}_{\mathcal{C}}\circ L(\underline{v}_i)=\mathcal{X}_{\mathcal{C}}(L(\underline{v}_i))$.

Sto concludendo:
$$\boxed{A=\big[\,\mathcal{X}_{\mathcal{C}}(L(\underline{v}_1))\,\big|\,\mathcal{X}_{\mathcal{C}}(L(\underline{v}_2))\,\big|\,\dots\,\big|\,\mathcal{X}_{\mathcal{C}}(L(\underline{v}_n))\,\big]}$$

Questa è la costruzione di $A$ che nella [[160_Paradigma_Rappresentare_una_Applicazione_Lineare_con_una_Matrice|lezione 20]] mancava; la definizione ufficiale è in [[162_Matrice_Rappresentativa_Definizione_22_1]].

## Note collegate
- [[160_Paradigma_Rappresentare_una_Applicazione_Lineare_con_una_Matrice]]
- [[158_Mappa_delle_Coordinate_e_Mappa_di_Parametrizzazione_Definizione_20_6]]
- [[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]]
- Indice: [[23_Indice_Lezione_22]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/obiettivo
