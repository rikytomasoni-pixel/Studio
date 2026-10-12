---
tags: [GAL, fondamenti, funzioni, iniettivita, suriettivita, lezione-1]
data: 2026-09-17
lezione: 1
fonte: "GAL_2026-2027_-_20260917_-_LEZIONE_1.pdf (slide 17-18)"
---

# Iniettività, suriettività e biettività

Siano $F \subseteq A \times B$ funzioni ([[16_Funzioni]]).

**!!!** (disegno: quattro diagrammi a frecce tra $A$ e $B$ — iniettività: $F = $ «l'iniziale di \_\_ è \_\_» con arancia, banana, limone, lampone → "a", "b", "l", NON iniettiva; altro esempio iniettivo con tre frecce parallele; suriettività: «ogni elemento del codominio è raggiunto da almeno una freccia» — esempio NON suriettivo con un punto non raggiunto, esempio suriettivo con l'esempio della frutta)

> [!warning] Def. 1.2 Funzione iniettiva
> Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **iniettiva** se $a_1, a_2 \in A$ e $(a_1,b),(a_2,b) \in F$ [cioè $F(a_1) = b$, $F(a_2) = b$, $F(a_1) = F(a_2)$] allora $a_1 = a_2$.
>
> Equivalentemente, $\forall\, a_1, a_2 \in A$: $F(a_1) = F(a_2) \Rightarrow a_1 = a_2$ ($F$ iniettivo); e $a_1 \neq a_2 \Rightarrow F(a_1) \neq F(a_2)$.

> [!warning] Def. 1.2 Funzione suriettiva
> Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **suriettiva** se $\forall\, b \in B$ esiste ($\exists$) almeno un elemento $a \in A$ tale che $(a,b) \in F$.
> Equivalentemente
> $$F^{-1}(b) = \{\, a \in A \mid F(a) = b \,\} \neq \emptyset$$
> (insieme delle **controimmagini** di $b$).

> [!warning] Def. 1.2 Funzione biettiva
> Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **biettiva** se è simultaneamente iniettiva e suriettiva.

**!!!** (disegno: esempio di biezione, due insiemi con frecce blu che abbinano a uno a uno i punti)

> [!note] Osservazione
> N.B. le biezioni producono un abbinamento perfetto tra gli elementi del dominio e quelli del codominio.

## Note collegate
- [[16_Funzioni]]
- [[19_Prodotto_Cartesiano_di_Piu_Insiemi]]
- [[17_Excursus_Logico_Negazione_Implicazione]]
- [[42_Prodotto_e_Composizione_di_Funzioni]]
- Indice: [[02_Indice_Lezione_1]] · [[00_MOC_GAL]]
