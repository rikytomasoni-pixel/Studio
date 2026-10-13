---
tags: [GAL, matrici, inversa, MEG, dimostrazione, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 65)"
---

# Esistenza della matrice inversa

Mettiamo insieme:
- MEG reversibile ([[01_Reversibilita_del_MEG]])
- MEG si può codificare con il prodotto matriciale (a sinistra) ([[02_Codifica_del_MEG_con_il_Prodotto_Matriciale]])

$$A \overset{T}{\leadsto} U \overset{Z}{\leadsto} A, \qquad A, U \in M_{\mathbb{K}}(m,n), \qquad T, Z \in M_{\mathbb{K}}(m,m)$$

$$\left.\begin{matrix} U = TA \\ A = ZU \end{matrix}\right\} \quad A = Z(TA) \overset{\text{PROP. ASS.}}{=} (ZT)A$$

$\forall A \in M_{\mathbb{K}}(m,n)$: $(ZT)A = A$
- $\Rightarrow ZT = \mathrm{Id}_m$
- $\Rightarrow Z$ è l'inverso sinistro di $T$; $T$ è l'inverso destro di $Z$

$$\left.\begin{matrix} U = TA \\ A = ZU \end{matrix}\right\} \quad U = TA = T(ZU) = (TZ)U$$
- $\Rightarrow TZ = \mathrm{Id}_m$
- $\Rightarrow Z$ è l'inverso destro di $T$; $T$ è l'inverso sinistro di $Z$

$T$ è l'inverso di $Z$ e viceversa:
$$Z = T^{-1}, \qquad T = Z^{-1}$$

> [!note] Osservazione
>ABBIAMO DIMOSTRATO CHE LE MATRICI INVERSE / INVERTIBILI ESISTONO. (Definizione: [[01_Matrice_Invertibile]]; unicità: [[02_Unicita_e_Bilateralita_dell_Inversa]].)

## Note collegate
- [[01_Matrice_Invertibile]]
- [[02_Unicita_e_Bilateralita_dell_Inversa]]
- [[01_Reversibilita_del_MEG]]
- [[02_Codifica_del_MEG_con_il_Prodotto_Matriciale]]
- [[05_Teorema_di_Binet]]
- Indice: [[00_Indice_Lezione_7]] · [[00_MOC_GAL]]
