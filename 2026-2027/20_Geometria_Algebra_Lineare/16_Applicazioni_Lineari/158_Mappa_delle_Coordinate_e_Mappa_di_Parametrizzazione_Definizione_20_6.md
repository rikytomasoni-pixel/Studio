---
tags: [GAL, applicazioni-lineari, isomorfismo, coordinate, parametrizzazione, basi, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 173)"
---

# Mappa delle coordinate e mappa di parametrizzazione (Definizione 20.6)

> [!abstract] Definizione 20.6
> Sia $V$ uno spazio vettoriale finitamente generato nel campo $\mathbb{K}$ con base $\mathcal{B}=\{\underline{v}_1,\dots,\underline{v}_n\}$ ($V$ è isomorfo a $\mathbb{K}^n$).
>
> - **Mappa delle coordinate** di $V$ rispetto a $\mathcal{B}$: l'isomorfismo $\mathcal{X}_{\mathcal{B}}:V\to\mathbb{K}^n$ definito da
> $$\mathcal{X}_{\mathcal{B}}(\underline{v}_1)=\underline{e}_1,\ \dots,\ \mathcal{X}_{\mathcal{B}}(\underline{v}_n)=\underline{e}_n$$
> - **Mappa di parametrizzazione** di $V$ rispetto a $\mathcal{B}$: l'isomorfismo inverso $\mathcal{P}_{\mathcal{B}}:\mathbb{K}^n\to V$ definito da
> $$\mathcal{P}_{\mathcal{B}}(\underline{e}_1)=\underline{v}_1,\ \dots,\ \mathcal{P}_{\mathcal{B}}(\underline{e}_n)=\underline{v}_n$$

## Esempio: mappa delle coordinate
$V=M_{\mathbb{R}}(2,2)$, $\dim V=4$, $\mathcal{B}=\{E_{11},E_{12},E_{21},E_{22}\}$ ($M_{\mathbb{R}}(2,2)$ è isomorfo a $\mathbb{R}^4$).

$\mathcal{X}_{\mathcal{B}}:M_{\mathbb{R}}(2,2)\to\mathbb{R}^4$:
$$\mathcal{X}_{\mathcal{B}}(E_{11})=\underline{e}_1,\quad\mathcal{X}_{\mathcal{B}}(E_{12})=\underline{e}_2,\quad\mathcal{X}_{\mathcal{B}}(E_{21})=\underline{e}_3,\quad\mathcal{X}_{\mathcal{B}}(E_{22})=\underline{e}_4$$
$$\begin{bmatrix}a_{11}&a_{12}\\a_{21}&a_{22}\end{bmatrix}=a_{11}E_{11}+a_{12}E_{12}+a_{21}E_{21}+a_{22}E_{22}\ \xmapsto{\ \mathcal{X}_{\mathcal{B}}\ }\ \begin{bmatrix}a_{11}\\a_{12}\\a_{21}\\a_{22}\end{bmatrix}=a_{11}\underline{e}_1+a_{12}\underline{e}_2+a_{21}\underline{e}_3+a_{22}\underline{e}_4$$

Questa operazione si chiama **flattening** (la matrice viene "appiattita" in un vettore colonna).

Esempio di mappa di parametrizzazione: [[159_Esempio_Mappa_di_Parametrizzazione_Polinomi_di_Grado_al_piu_2]].

## Note collegate
- [[157_Teorema_20_5_Teorema_di_Isomorfismo_tra_Spazi_Finitamente_Generati]]
- [[101_Teorema_di_Unicita_della_Rappresentazione_rispetto_a_una_Base]]
- [[100_Base_di_uno_Spazio_Vettoriale]]
- [[121_Basi_Canoniche]]
- [[142_Come_Definire_una_Applicazione_Lineare_Proposizione_17_2]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/mappa-coordinate
