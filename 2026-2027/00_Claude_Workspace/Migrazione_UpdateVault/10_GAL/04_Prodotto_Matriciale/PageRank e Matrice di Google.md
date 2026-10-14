---
created: 2026-10-01
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/prodotto_matriciale
aliases: []
origine: UpdateVault
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# PageRank e Matrice di Google

> [!example] Esempio (come funziona Google — parte 1)
> $S = \{\text{insieme delle pagine web (di interesse)}\}$
> $S \times S = \{(\text{pagina 1},\text{pagina 2}) \mid \text{pagina 1, pagina 2} \in S\}$
> [annotazioni: pagina 1 = pagina di arrivo (rosso); pagina 2 = pagina di partenza (blu)]
>
> Considero delle funzioni $f : S \times S \to \mathbb{R}$ che misurano la probabilità di navigare tra le pagine (secondo criteri assegnati) ([[Matrici come Rappresentazione di Funzioni]]).
> $$A : S \times S \to \mathbb{R}, \qquad a_{ij} = \text{probabilità di passare dalla pagina } j \text{ alla pagina } i.$$

**Google considera 2 comportamenti:** TAP RANDOM SURFER e KEYBOARD RANDOM SURFER.
*Random* significa che ogni possibile trasferimento è equiprobabile.
- **TAP:** mi muovo solo con i link ipertestuali.
- **KEYBOARD:** mi muovo solo scrivendo l'indirizzo esplicito della pagina.



$$T = \begin{bmatrix} 0 & 1 & 0 \\ \tfrac12 & 0 & 1 \\ \tfrac12 & 0 & 0 \end{bmatrix}, \qquad K = \begin{bmatrix} \tfrac13 & \tfrac13 & \tfrac13 \\ \tfrac13 & \tfrac13 & \tfrac13 \\ \tfrac13 & \tfrac13 & \tfrac13 \end{bmatrix}$$
(righe: arrivo pag. 1, 2, 3; colonne: partenza pag. 1, 2, 3).

> [!warning] Def. Matrice di Google
> $G$ = matrice di Google = media pesata tra le due matrici, con $p \in (0,1)$ (**damping number**):
> $$G = p\,T + (1-p)\,K$$

**Idea di Google:** la significatività corrisponde a per quanto tempo / quante volte visito una pagina.
- $G$ descrive le probabilità di navigazione in 1 step
- $G^2 = G \cdot G$ descrive le probabilità di navigazione in 2 step
- $G^3 = G \cdot G \cdot G$ descrive le probabilità di navigazione in 3 step
- $\vdots$
- $G^k$ descrive le probabilità di navigazione in $k$ step
- $\vdots$

(Le potenze sono prodotti righe per colonne: [[Prodotto Righe per Colonne]].)

> [!example] Esempio (Python)
>
> **Domande**
> - è sempre vero che questo processo si stabilizza?
> - è importante come allochiamo le masse iniziali?

---
Precedente: [[Prodotto e Composizione di Funzioni]] · Successivo: [[Proprietà del Prodotto Matriciale]]
