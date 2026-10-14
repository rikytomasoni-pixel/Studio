---
created: 2026-09-17
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/1
  - argomento/fondamenti
aliases: []
---
[[00_GAL_Fondamenti|⬅️ Torna a Fondamenti]]

# Iniettività Suriettività Biettività
![[suriettivaIniettiva.png]]
### Definizione 1.2

- Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **iniettiva** se, presi $a_1, a_2 \in A$ e $(a_1,b),(a_2,b) \in F$ (cioè $F(a_1) = b$, $F(a_2) = b$, cioè $F(a_1) = F(a_2)$), allora $a_1 = a_2$.

  Equivalentemente:

  $$
  \forall a_1, a_2 \in A:\ F(a_1) = F(a_2) \Rightarrow a_1 = a_2 \qquad (F \text{ iniettiva})
  $$

  $$
  a_1 \neq a_2 \Rightarrow F(a_1) \neq F(a_2)
  $$

- Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **suriettiva** se $\forall b \in B$ esiste ($\exists$) almeno un elemento $a \in A$ tale che $(a,b) \in F$. Equivalentemente:

  $$
  F^{-1}(b) = \{a \in A \mid F(a) = b\} \neq \emptyset
  $$

  dove $F^{-1}(b)$ è l'insieme delle **controimmagini** di $b$.

- Una funzione $F \subseteq A \times B$ ($F : A \to B$) è **biettiva** se è simultaneamente iniettiva e suriettiva.

![[fBiettiva.png]]

> **N.B.** Le biezioni producono un abbinamento perfetto tra gli elementi del dominio e quelli del codominio.

---
Precedente: [[Excursus Logico, Negazione dell'Implicazione]] · Successivo: [[Prodotto Cartesiano di più Insiemi]]
