---
tags: [GAL, matrici, applicazioni, pagerank, google, lezione-4]
data: 2026-10-01
lezione: 4
fonte: "GAL_2026-2027_-_20261001_-_LEZIONE_4.pdf (slide 39-42)"
---

# PageRank e matrice di Google (parte 1)

> [!example] Esempio (come funziona Google — parte 1)
> $S = \{\text{insieme delle pagine web (di interesse)}\}$
> $S \times S = \{(\text{pagina 1},\text{pagina 2}) \mid \text{pagina 1, pagina 2} \in S\}$
> [annotazioni: pagina 1 = pagina di arrivo (rosso); pagina 2 = pagina di partenza (blu)]
>
> Considero delle funzioni $f : S \times S \to \mathbb{R}$ che misurano la probabilità di navigare tra le pagine (secondo criteri assegnati) ([[01_Matrici_come_Rappresentazione_di_Funzioni]]).
> $$A : S \times S \to \mathbb{R}, \qquad a_{ij} = \text{probabilità di passare dalla pagina } j \text{ alla pagina } i.$$

**Google considera 2 comportamenti:** TAP RANDOM SURFER e KEYBOARD RANDOM SURFER.
*Random* significa che ogni possibile trasferimento è equiprobabile.
- **TAP:** mi muovo solo con i link ipertestuali.
- **KEYBOARD:** mi muovo solo scrivendo l'indirizzo esplicito della pagina.



$$T = \begin{bmatrix} 0 & 1 & 0 \\ \tfrac12 & 0 & 1 \\ \tfrac12 & 0 & 0 \end{bmatrix}, \qquad K = \begin{bmatrix} \tfrac13 & \tfrac13 & \tfrac13 \\ \tfrac13 & \tfrac13 & \tfrac13 \\ \tfrac13 & \tfrac13 & \tfrac13 \end{bmatrix}$$
(righe: arrivo pag. 1, 2, 3; colonne: partenza pag. 1, 2, 3).

(slide 40: accanto a ciascuna matrice c'è il grafo orientato sulle 3 pagine. TAP: archi con peso $1$ e $\tfrac12$ secondo i link presenti (dalla pagina 1 due link con peso $\tfrac12$, verso 2 e 3; da 2 verso 1 con peso 1; da 3 verso 2 con peso 1). KEYBOARD: ogni coppia di pagine, cappi compresi, è collegata da archi di peso $\tfrac13$.)

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

(Le potenze sono prodotti righe per colonne: [[02_Prodotto_Matriciale_Righe_per_Colonne]].)

> [!example] Esempio (Python, slide 42)
> Grafo di 5 pagine (nodi 0-4), con la visualizzazione dell'"Evoluzione PageRank" alle iterazioni 0, 3 e 10: il colore dei nodi (scala di colori laterale) indica la massa/probabilità di ciascuna pagina e cambia al procedere delle iterazioni.
>
> **Domande**
> - è sempre vero che questo processo si stabilizza?
> - è importante come allochiamo le masse iniziali?

## Note collegate
- [[03_Prodotto_e_Composizione_di_Funzioni]]
- [[02_Prodotto_Matriciale_Righe_per_Colonne]]
- [[01_Matrici_come_Rappresentazione_di_Funzioni]]
- [[05_Proprieta_del_Prodotto_Matriciale]]
- Indice: [[00_Indice_Lezione_4]] · [[00_MOC_GAL]]
