---
tags: [GAL, matrici, funzioni, motivazione, lezione-3]
data: 2026-09-30
lezione: 3
fonte: "GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 22-25)"
---

# Matrici come rappresentazione di funzioni

**Obiettivo:** «valutare» / «quantificare» gli elementi di un prodotto cartesiano ([[11_Prodotto_Cartesiano]]).

> [!example] Esempio 1
> $T = \{\text{voti sufficienti della prova teorica}\}$, $E = \{\text{voti sufficienti della prova di esercizi}\}$
> $T \times E = \{(16,16),(16,17),\dots,(16,32),\ (17,16),(17,17),\dots,(17,32),\ \vdots\ (32,16),\dots,(32,32)\}$
> $$V : T \times E \to \mathbb{N},\qquad (t,e) \mapsto \left\lceil \tfrac{30}{100}\, t + \tfrac{70}{100}\, e \right\rceil$$

**Obiettivo:** trovare una rappresentazione alternativa di $V$ (che sia più efficace / comunicativa).

**!!!** (tabella stampata: griglia dei voti, colonne «ESERCIZI 70%» da 16 a 32, righe «TEORIA 30%» da 16 a 32, con i valori da 16 a 30L; celle rosse per le combinazioni insufficienti; annotazioni: «righe corrispondono agli elementi di $T$», «colonne corrispondono agli elementi di $E$»)

> [!example] Esempio 2
> $M = \{\text{esiti lancio di una moneta}\}$, $D = \{\text{esiti lancio di un dado}\}$
> $M \times D = \{\text{coppie (ordinate) di esiti del lancio di una moneta e un dado}\} = \{(T,1),(T,2),\dots\}$
> $$P : M \times D \to [0,1] \subseteq \mathbb{R},\qquad P((m,d)) = \frac{\#\text{esiti favorevoli}}{\#\text{totale di esiti possibili}} = \frac{1}{12}$$
> Come prima, posso rappresentare la funzione mediante una tabella:
>
> | | 1 | 2 | 3 | 4 | 5 | 6 |
> |---|---|---|---|---|---|---|
> | T | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 |
> | C | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 |
>
> Questa tabella si chiama **matrice di probabilità congiunta** di $M$ e $D$.

> [!example] Esempio 3 — grafico di una funzione
> $f : \mathbb{R} \to \mathbb{R}$, $\Gamma(f) = \{(x,y) \mid y = f(x)\} \subseteq \mathbb{R} \times \mathbb{R}$
> $$v : \mathbb{R} \times \mathbb{R} \to \{0,1\},\qquad v(x,y) = \begin{cases} 1 & \text{se } (x,y) \in \Gamma(f) \\ 0 & \text{se } (x,y) \notin \Gamma(f) \end{cases}$$
> $f(x) = x^2$

**!!!** (disegno: piano $xy$ azzurro con la curva rossa $y = f(x)$ e, sopra di essa, la funzione $v(x,y)$ in blu con segmenti verticali)

> [!example] Esempio 4
> $A = \{\text{arancia, limone, lampone}\}$, $B = \{\text{"a", "b", "l"}\}$
> $f : A \to B$ «… ha come iniziale …» ($\in A$, $\in B$):
> $f(\text{arancia}) = \text{"a"}$, $f(\text{limone}) = \text{"l"}$, $f(\text{lampone}) = \text{"l"}$
> $\Gamma(f) \subseteq A \times B$, $\Gamma(f) = \{(\text{arancia},\text{"a"}),\ (\text{limone},\text{"l"}),\ (\text{lampone},\text{"l"})\}$
> $$v : A \times B \to \{0,1\},\qquad v(\text{frutto},\text{lettera}) = \begin{cases} 1 & (\text{frutto},\text{lettera}) \in \Gamma(f) \\ 0 & (\text{frutto},\text{lettera}) \notin \Gamma(f) \end{cases}$$
> Utilizziamo una tabella:
>
> | | arancia | lampone | limone |
> |---|---|---|---|
> | "a" | 1 | 0 | 0 |
> | "b" | 0 | 0 | 0 |
> | "l" | 0 | 1 | 1 |

Ora definiamo le matrici in generale → [[32_Definizione_di_Matrice]].

## Note collegate
- [[11_Prodotto_Cartesiano]]
- [[16_Funzioni]]
- [[32_Definizione_di_Matrice]]
- [[64_Rango_e_Matrice_di_Probabilita_Congiunta]]
- [[10_Organizzazione_del_Corso]]
- Indice: [[04_Indice_Lezione_3]] · [[00_MOC_GAL]]
