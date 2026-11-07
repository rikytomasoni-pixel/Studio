---
tags: [GAL, base, completamento, MEG, esempio, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 129)"
---

# Completamento ad una base

**Problema (II).** In $\mathbb{R}^n$ sia $\{\underline{v}_1,\dots,\underline{v}_k\}$ un insieme di vettori linearmente indipendenti con $k<n$. Voglio completarlo ad una base di $\mathbb{R}^n$.

**Strategia.** Considero l'insieme $\{\underline{v}_1,\dots,\underline{v}_k\}\cup\{\underline{e}_1,\dots,\underline{e}_n\}$ (con la [[121_Basi_Canoniche|base canonica]]) ed **estraggo** una base ([[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]]):
$$\{\underline{v}_1,\dots,\underline{v}_k\}\cup\{\underline{e}_1,\dots,\underline{e}_n\}\ \overset{\text{estraggo}}{\leadsto}\ \{\underline{v}_1,\dots,\underline{v}_k\}\cup\{\,n-k\text{ vettori della base canonica}\,\}$$

## Esempio in $\mathbb{R}^3$
Siano $\underline{v}_1=\begin{bmatrix}1\\0\\1\end{bmatrix}$, $\underline{v}_2=\begin{bmatrix}0\\1\\1\end{bmatrix}$. Scrivo $\underline{v}_1,\underline{v}_2,\underline{e}_1,\underline{e}_2,\underline{e}_3$ come colonne:
$$\left[\begin{array}{cc|ccc}1&0&1&0&0\\0&1&0&1&0\\1&1&0&0&1\end{array}\right]\xrightarrow{\ \mathrm{III}-\mathrm{I}\to\mathrm{III}\ }\left[\begin{array}{cc|ccc}1&0&1&0&0\\0&1&0&1&0\\0&1&-1&0&1\end{array}\right]\xrightarrow{\ \mathrm{III}-\mathrm{II}\to\mathrm{III}\ }\left[\begin{array}{cc|ccc}1&0&1&0&0\\0&1&0&1&0\\0&0&-1&-1&1\end{array}\right]$$
I pivot sono nelle colonne di $\underline{v}_1$, $\underline{v}_2$ e $\underline{e}_1$ (il terzo pivot è il $-1$ in colonna $\underline{e}_1$). Quindi la base completata è
$$\{\underline{v}_1,\underline{v}_2,\underline{e}_1\}.$$

> [!note] Osservazione (non presente negli appunti)
> I vettori $\underline{v}_1,\dots,\underline{v}_k$ sono indipendenti e messi per primi, quindi hanno sempre un pivot e vengono sempre conservati: l'estrazione scarta solo vettori canonici. Verifica: $\det\begin{bmatrix}1&0&1\\0&1&0\\1&1&0\end{bmatrix}=-1\neq0$.

## Note collegate
- [[135_Formula_di_Grassmann_Teorema_16_3]] (uso del completamento nella dimostrazione, L16)
- [[122_Estrazione_e_Completamento_Due_Problemi_Classici]]
- [[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]]
- [[121_Basi_Canoniche]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- Successiva: [[126_Fac_simile_28_10_Esercizio_su_Sottospazi_Dimensione_e_Basi]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/base/completamento
