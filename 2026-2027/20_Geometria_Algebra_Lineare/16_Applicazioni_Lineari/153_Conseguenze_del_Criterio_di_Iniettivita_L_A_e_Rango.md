---
tags: [GAL, applicazioni-lineari, iniettivita, matrice-associata, rango, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 167-168)"
---

# Conseguenze del criterio di iniettività: $L_A$ e rango

$L_A:\mathbb{K}^n\to\mathbb{K}^m$, $A\in M_{\mathbb{K}}(m,n)$:
$$\begin{aligned}
L_A\ \text{iniettivo}&\iff\ker(L_A)=\{\underline{0}\}\iff\ker(A)=\{\underline{0}\}\\
&\iff A\underline{x}=\underline{0}\ \text{ha un'unica soluzione}\\
&\overset{\text{TEO R.C.}}{\iff}\#\text{parametri liberi}=n-r(A)=0\\
&\iff r(A)=n
\end{aligned}$$

## Vincolo sulle dimensioni
$r(A)\le\min(m,n)$ e $r(A)=n$ $\Rightarrow$ $n\le m$. Quindi
$$L_A:\mathbb{K}^n\to\mathbb{K}^m\ \text{iniettivo}\ \Rightarrow\ n\le m$$
e, per contrapposizione,
$$\begin{aligned}
L_A\ \text{NON iniettiva}&\Leftarrow n>m\\
L_A\ \text{NON invertibile}&\Leftarrow n>m\\
A\ \text{NON invertibile}&\Leftarrow n>m
\end{aligned}$$

> [!abstract] Riepilogo con la suriettività
> - $L_A$ suriettivo $\iff r(A)=m$ ([[150_Suriettivita_di_L_A_e_Spazio_delle_Colonne]]); $m>n\Rightarrow$ non suriettivo.
> - $L_A$ iniettivo $\iff r(A)=n$; $n>m\Rightarrow$ non iniettivo.

## Note collegate
- [[152_Teorema_20_1_Criterio_di_Iniettivita]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[63_Rango_di_una_Matrice]]
- [[149_Conseguenze_della_Suriettivita_Generatori_e_Dimensione]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/iniettivita-L_A
