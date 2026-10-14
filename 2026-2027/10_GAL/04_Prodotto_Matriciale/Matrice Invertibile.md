---
created: 2026-10-07
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/prodotto_matriciale
aliases: []
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Matrice Invertibile

Abbiamo visto che c'è un elemento neutro per il [[Prodotto Righe per Colonne|Prodotto Matriciale]] (la [[Matrice Identità e Matrici Diagonali|Matrice Identità]]). **Domanda**: ha senso parlare di elemento inverso per il prodotto matriciale?

### Definizione 6.1

Consideriamo una matrice $A \in M_{\mathbb{K}}(n,n)$.

- $A$ è **invertibile a destra** se esiste (almeno) una matrice $B \in M_{\mathbb{K}}(n,n)$ tale che $AB = \mathrm{Id}_n$.
- $A$ è **invertibile a sinistra** se esiste (almeno) una matrice $C \in M_{\mathbb{K}}(n,n)$ tale che $CA = \mathrm{Id}_n$.
- $A$ è **invertibile** se è invertibile sia a destra sia a sinistra.

**Domande aperte**:

- quante sono le matrici inverse?
- che relazione c'è tra le matrici inverse destre e le matrici inverse sinistre?
- esistono le matrici inverse?
- come calcolo le matrici inverse?

### Proposizione 6.2

- **HP**: sia $A \in M_{\mathbb{K}}(n,n)$ una matrice invertibile.
- **TH1**: l'inverso destro è uguale all'inverso sinistro.
- **TH2**: l'inverso è unico.

**Dimostrazione.** Siano $B,C \in M_{\mathbb{K}}(n,n)$.

*(TH1)* Per ipotesi $A$ è invertibile, quindi per definizione esistono $B$ e $C$ tali che

$$
AB = \mathrm{Id}_n \quad (1), \qquad CA = \mathrm{Id}_n \quad (2)
$$

Allora

$$
B \overset{\text{el. neutro}}{=} \mathrm{Id}_n B \overset{(2)}{=} (CA)B \overset{\text{prop. ass.}}{=} C(AB) \overset{(1)}{=} C\,\mathrm{Id}_n \overset{\text{el. neutro}}{=} C
$$

*(TH2)* Supponiamo di avere due matrici inverse $B,C \in M_{\mathbb{K}}(n,n)$; devo dimostrare $B = C$. $B$ e $C$ sono sia inverse destre che sinistre. Interpreto $B$ come inverso destro, $C$ come inverso sinistro e ripeto l'argomento di prima. $\blacksquare$

---
Precedente: [[Matrice Identità e Matrici Diagonali]] · Successivo: [[Non Commutatività del Prodotto]]
