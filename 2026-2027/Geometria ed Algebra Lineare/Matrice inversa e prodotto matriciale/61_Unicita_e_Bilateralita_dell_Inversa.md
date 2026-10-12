---
tags: [GAL, matrici, inversa, dimostrazione, unicita, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 47)"
---

# Unicità e bilateralità dell'inversa

> [!abstract] Teorema (Proposizione 6.2)
> - **HP** Sia $A \in M_{\mathbb{K}}(m,n)$ una matrice invertibile ([[60_Matrice_Invertibile]]).
> - **TH1** L'inverso destro è uguale all'inverso sinistro.
> - **TH2** L'inverso è unico.

**dim:** $B, C \in M_{\mathbb{K}}(n,m)$.

**(TH1)** HP $A$ invertibile $\overset{\text{DEF}}{\iff}$
$$\begin{cases} \exists\, B \text{ t.c. } AB = \mathrm{Id}_m & (1) \\ \exists\, C \text{ t.c. } CA = \mathrm{Id}_n & (2) \end{cases}$$
$$B \overset{\text{EL. NEUTRO}}{=} \mathrm{Id}_n B \overset{(2)}{=} (CA)B \overset{\text{PROP. ASS.}}{=} C(AB) \overset{(1)}{=} C\,\mathrm{Id}_m \overset{\text{EL. NEUTRO}}{=} C$$

**(TH2)** Supponiamo di avere due matrici inverse $B, C \in M_{\mathbb{K}}(n,m)$. Devo dimostrare $B = C$. $B$ e $C$ sono sia inverse destre che sinistre. Interpreto $B$ come inverso destro, $C$ come inverso sinistro e ripeto l'argomento di prima. $\blacksquare$

## Note collegate
- [[60_Matrice_Invertibile]]
- [[72_Esistenza_della_Matrice_Inversa]]
- [[44_Proprieta_del_Prodotto_Matriciale]]
- [[45_Matrice_Identita_e_Matrici_Diagonali]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]
