---
created: 2026-10-08
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/eliminazione_di_gauss
aliases: []
origine: UpdateVault
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# Esistenza della Matrice Inversa

Mettiamo insieme:
- MEG reversibile ([[Reversibilità del MEG]])
- MEG si può codificare con il prodotto matriciale (a sinistra) ([[Codifica del MEG con il Prodotto]])

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
>ABBIAMO DIMOSTRATO CHE LE MATRICI INVERSE / INVERTIBILI ESISTONO. (Definizione: [[Matrice Invertibile]]; unicità: [[Matrice Invertibile]].)

---
Precedente: [[Codifica del MEG con il Prodotto]] · Successivo: [[MEG e Rango]]
