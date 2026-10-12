---
tags: [GAL, fondamenti, insiemi, prodotto-cartesiano, lezione-0]
data: 2026-09-16
lezione: 0
fonte: "GAL_2026-2027_-_20260916_-_LEZIONE_0.pdf (slide 6-8)"
---

# Prodotto cartesiano

> [!warning] Def. 0.1 Prodotto cartesiano
> Dati due insiemi $A$ e $B$ qualsiasi, il **prodotto cartesiano** $A \times B$ è l'insieme delle coppie **ordinate** $(a,b)$ con $a \in A$ e $b \in B$.
> $$A \times B = \{\, (a,b) \mid a \in A,\ b \in B \,\}$$

> [!note] Osservazione (Domanda)
> D. perché *cartesiano*?

> [!example] Esempio 1 — piano cartesiano
> $\mathbb{R}^2 = \mathbb{R} \times \mathbb{R}$
> - gli elementi del piano cartesiano sono punti;
> - se fissiamo un sistema di riferimento, cioè gli assi cartesiani, ogni punto è univocamente identificato da una coppia $(x,y)$, $x \in \mathbb{R}$, $y \in \mathbb{R}$.
>
> $P = (x_P, y_P) = (2,4)$
>
> Se scambio l'ordine: $(4,2) \in \mathbb{R} \times \mathbb{R}$ [annotazione: corrisponde al punto $Q$].

**!!!** (disegno: assi $x$, $y$ con i punti $P$ (rosso) e $Q$ (blu); indicate $x_P$ e $y_P$)

> [!example] Esempio 2 — voti
> $A = \{\text{valutazioni sufficienti per la parte di esercizi}\} = \{16, 17, 18, \dots, 32\}$
> $B = \{\text{valutazioni sufficienti per la parte di teoria}\} = \{16, 17, \dots, 32\}$
>
> $A \times B = \{(a,b) \mid a \in A,\ b \in B\} = \{\text{coppie di valutazioni sufficienti per esercizi e teoria (in quest'ordine)}\}$
>
> - $a = 28,\ b = 22 \leadsto \text{VOTO} = 70\%\, a + 30\%\, b = \frac{7}{10} \cdot 28 + \frac{3}{10}\, 22$
> - $a = 22,\ b = 28 \leadsto \text{VOTO} = \frac{7}{10}\, 22 + \frac{3}{10}\, 28$

> [!example] Esempio 3 — moneta e dado
> Consideriamo: lancio di una moneta (equa); lancio di un dado a sei facce (equo).
> $A = \{\text{esiti del lancio della moneta}\} = \{T, C\}$
> $B = \{\text{esiti del lancio del dado}\} = \{1,2,3,4,5,6\}$
> $$A \times B = \{\text{esiti del lancio simultaneo di una moneta e di un dado}\} = \{(T,1),(T,2),\dots,(T,6),\ (C,1),(C,2),\dots,(C,6)\}$$

> [!note] Osservazione (Domanda)
> D. come può essere utile il prodotto cartesiano? → vedi [[12_Relazione_Binaria]]

## Note collegate
- [[12_Relazione_Binaria]]
- [[16_Funzioni]]
- [[19_Prodotto_Cartesiano_di_Piu_Insiemi]]
- [[30_Matrici_come_Rappresentazione_di_Funzioni]]
- Indice: [[01_Indice_Lezione_0]] · [[00_MOC_GAL]]
