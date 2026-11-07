---
tags: [GAL, matrici, inversa, invertibilita, definizione, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 46)"
---

# Matrice invertibile

Sulle matrici: abbiamo visto che c'è un elemento neutro per il prodotto matriciale ([[45_Matrice_Identita_e_Matrici_Diagonali]]).

> [!note] Osservazione (Domanda)
> D. ha senso parlare di elemento inverso per il prodotto matriciale?

> [!warning] Def. 6.1 Matrice invertibile
> Consideriamo una matrice $A \in M_{\mathbb{K}}(m,n)$.
> - $A$ è **invertibile a destra** se esiste (almeno) una matrice $B \in M_{\mathbb{K}}(n,m)$ tale che $AB = \mathrm{Id}_m$.
> - $A$ è **invertibile a sinistra** se esiste (almeno) una matrice $C \in M_{\mathbb{K}}(n,m)$ tale che $CA = \mathrm{Id}_n$.
> - $A$ è **invertibile** se è invertibile sia a destra che a sinistra.

> [!note] Osservazione (Domande)
> D.
> - quante sono le matrici inverse? → [[61_Unicita_e_Bilateralita_dell_Inversa]]
> - che relazione c'è tra le matrici inverse destre e le matrici inverse sinistre? → [[61_Unicita_e_Bilateralita_dell_Inversa]]
> - esistono le matrici inverse? → [[72_Esistenza_della_Matrice_Inversa]]
> - come calcolo le matrici inverse? (obiettivo (I) del recap in [[66_Matrici_Triangolari]])

> [!note] Osservazione (non presente negli appunti): invertibilità destra, sinistra e rango
> Sia $A\in M_{\mathbb{K}}(m,n)$. Il **rango** dice quale inverso può esistere:
> $$A\ \text{invertibile a destra}\iff r(A)=m\qquad\qquad A\ \text{invertibile a sinistra}\iff r(A)=n$$
> (rango massimo "per righe" nel primo caso, "per colonne" nel secondo).
>
> **Perché a destra** ($AB=\mathrm{Id}_m$). Cercare $B$ significa risolvere gli $m$ sistemi $A\underline{x}=\underline{e}_j$ ([[87_Ricerca_della_Matrice_Inversa]]).
> - Se $r(A)=m$: $A$ ha $m$ righe, quindi $r(A|\underline{b})\le m=r(A)$ per ogni $\underline{b}$, cioè $r(A|\underline{b})=r(A)$ e per [[82_Teorema_di_Rouche_Capelli]] ogni sistema ha soluzione.
> - Se $r(A)<m$: la forma a scala $U$ ha una riga nulla, quindi esiste un $\underline{b}$ con $r(A|\underline{b})>r(A)$ (sistema impossibile) e $AB=\mathrm{Id}_m$ non ha soluzione.
>
> **Perché a sinistra** ($CA=\mathrm{Id}_n$). Trasponendo: $A^{T}C^{T}=\mathrm{Id}_n$, cioè $C^{T}$ è un inverso destro di $A^{T}\in M_{\mathbb{K}}(n,m)$, quindi $r(A^{T})=n$. Inoltre $r(A^{T})=r(A)$: trasponendo $A=\sum_{i=1}^{r}C_iR_i$ si ottiene $A^{T}=\sum_{i=1}^{r}R_i^{T}C_i^{T}$, stesso numero di addendi di rango 1 ([[63_Rango_di_una_Matrice]]).
>
> **Conseguenze** (ricordando $r(A)\le\min(m,n)$):
> - $m<n$ (matrice "larga"): $r(A)\le m<n$, quindi **mai** invertibile a sinistra; invertibile a destra $\iff r(A)=m$ (come l'esempio $2\times3$ di [[87_Ricerca_della_Matrice_Inversa]]).
> - $m>n$ (matrice "alta"): **mai** invertibile a destra; invertibile a sinistra $\iff r(A)=n$.
> - $m=n$: le due condizioni coincidono ($r(A)=n$), quindi *invertibile a destra $\iff$ invertibile a sinistra $\iff$ invertibile*. Solo in questo caso ha senso il determinante: $A$ invertibile $\iff\det(A)\neq0$ ([[88_Teorema_sull_Invertibilita_della_Matrice]]).
>
> In particolare una matrice invertibile (da entrambi i lati) è necessariamente **quadrata**, perché richiede $r(A)=m$ e $r(A)=n$. Per le non quadrate l'analogo del determinante è il rango.

## Note collegate
- [[45_Matrice_Identita_e_Matrici_Diagonali]]
- [[61_Unicita_e_Bilateralita_dell_Inversa]]
- [[72_Esistenza_della_Matrice_Inversa]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]] (caso quadrato: $\det\neq0$)
- [[63_Rango_di_una_Matrice]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]

#GAL/matrice-inversa/matrice-invertibile
