---
created: 2026-10-08
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/eliminazione_di_gauss
aliases: []
---
[[00_GAL_Eliminazione_di_Gauss|⬅️ Torna a Eliminazione di Gauss]]

# Esistenza della Matrice Inversa

$$
A \overset{T}{\leadsto} U \overset{Z}{\leadsto} A, \qquad A,U \in M_{\mathbb{K}}(m,n),\quad T,Z \in M_{\mathbb{K}}(m,m)
$$

$$
\left.\begin{array}{l} U = TA \\ A = ZU \end{array}\right\} \Rightarrow A = Z(TA) \overset{\text{prop. ass.}}{=} (ZT)A
$$

Poiché $(ZT)A = A$ per ogni $A \in M_{\mathbb{K}}(m,n)$:

$$
ZT = \mathrm{Id}_m \quad\Rightarrow\quad Z \text{ è l'inverso sinistro di } T,\ \ T \text{ è l'inverso destro di } Z
$$

Analogamente, da $U = TA = T(ZU) = (TZ)U$:

$$
TZ = \mathrm{Id}_m \quad\Rightarrow\quad Z \text{ è l'inverso destro di } T,\ \ T \text{ è l'inverso sinistro di } Z
$$

Quindi $T$ è l'inverso di $Z$ e viceversa:

$$
Z = T^{-1}, \qquad T = Z^{-1}
$$

> **Abbiamo dimostrato che le matrici inverse/invertibili esistono.** (Vedi [[Matrice Invertibile|Matrice Invertibile]].)

---
Precedente: [[Codifica del MEG con il Prodotto]] · Successivo: [[MEG e Rango]]
