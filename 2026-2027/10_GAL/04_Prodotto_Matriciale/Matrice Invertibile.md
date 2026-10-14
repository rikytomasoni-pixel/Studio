---
created: 2026-10-07
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/prodotto_matriciale
aliases: []
origine: UpdateVault
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Matrice Invertibile

Sulle matrici: abbiamo visto che c'è un elemento neutro per il prodotto matriciale ([[Matrice Identità e Matrici Diagonali]]).

> [!note] Osservazione (Domanda)
> D. ha senso parlare di elemento inverso per il prodotto matriciale?

> [!warning] Def. 6.1 Matrice invertibile
> Consideriamo una matrice $A \in M_{\mathbb{K}}(m,n)$.
> - $A$ è **invertibile a destra** se esiste (almeno) una matrice $B \in M_{\mathbb{K}}(n,m)$ tale che $AB = \mathrm{Id}_m$.
> - $A$ è **invertibile a sinistra** se esiste (almeno) una matrice $C \in M_{\mathbb{K}}(n,m)$ tale che $CA = \mathrm{Id}_n$.
> - $A$ è **invertibile** se è invertibile sia a destra che a sinistra.

> [!note] Osservazione (Domande)
> D.
> - quante sono le matrici inverse? → [[Matrice Invertibile]]
> - che relazione c'è tra le matrici inverse destre e le matrici inverse sinistre? → [[Matrice Invertibile]]
> - esistono le matrici inverse? → [[Esistenza della Matrice Inversa]]
> - come calcolo le matrici inverse? (obiettivo (I) del recap in [[Matrici Triangolari]])

## Unicità e bilateralità dell'inversa

> [!abstract] Teorema (Proposizione 6.2)
> - **HP** Sia $A \in M_{\mathbb{K}}(m,n)$ una matrice invertibile ([[Matrice Invertibile]]).
> - **TH1** L'inverso destro è uguale all'inverso sinistro.
> - **TH2** L'inverso è unico.

**dim:** $B, C \in M_{\mathbb{K}}(n,m)$.

**(TH1)** HP $A$ invertibile $\overset{\text{DEF}}{\iff}$
$$\begin{cases} \exists\, B \text{ t.c. } AB = \mathrm{Id}_m & (1) \\ \exists\, C \text{ t.c. } CA = \mathrm{Id}_n & (2) \end{cases}$$
$$B \overset{\text{EL. NEUTRO}}{=} \mathrm{Id}_n B \overset{(2)}{=} (CA)B \overset{\text{PROP. ASS.}}{=} C(AB) \overset{(1)}{=} C\,\mathrm{Id}_m \overset{\text{EL. NEUTRO}}{=} C$$

**(TH2)** Supponiamo di avere due matrici inverse $B, C \in M_{\mathbb{K}}(n,m)$. Devo dimostrare $B = C$. $B$ e $C$ sono sia inverse destre che sinistre. Interpreto $B$ come inverso destro, $C$ come inverso sinistro e ripeto l'argomento di prima. $\blacksquare$

---
Precedente: [[Matrice Identità e Matrici Diagonali]] · Successivo: [[Non Commutatività del Prodotto]]
