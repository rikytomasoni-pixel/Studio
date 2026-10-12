---
tags: [GAL, vettori, geometria, prodotto-interno, ortogonalita, lezione-2]
data: 2026-09-17
lezione: 2
fonte: "GAL_2026-2027_-_20260917_-_LEZIONE_2.pdf (p. 4-5)"
---

# Prodotto interno e ortogonalità

> [!warning] Def. Prodotto interno
> Supponiamo che $u$ e $v$ siano due vettori in un sistema di riferimento cartesiano ([[23_Sistemi_di_Riferimento_e_Coordinate]]). Il loro **prodotto interno** è il numero reale $u \cdot v$ definito come segue:
> - se $u = 0$ oppure $v = 0$, allora $u \cdot v = 0$;
> - se $u, v \neq 0$ allora
> $$u \cdot v = \|u\| \cdot \|v\| \cdot \cos\vartheta$$
> dove $\|u\|$ e $\|v\|$ sono le lunghezze di $u$ e $v$ rispetto all'unità di misura.

**!!!** (disegno: due vettori $u$ e $v$ uscenti da $O$ con l'angolo $\vartheta$ tra essi)

> [!warning] Def. Vettori ortogonali
> Due vettori $u$ e $v$ sono **ortogonali** se l'angolo $\vartheta$ fra i due vettori è retto.
> Si conviene che il vettore $0$ sia ortogonale a tutti i vettori.

**!!!** (disegno: $u$ orizzontale e $v$ verticale con angolo retto in $O$)

> [!abstract] Teorema (Proposizione)
> Dati due vettori $u$ e $v$,
> $$u \perp v \iff u \cdot v = 0.$$

$\blacksquare$ [simbolo di fine presente nell'originale; dimostrazione non riportata]

> [!abstract] Teorema (Proposizione — Proprietà del prodotto interno)
> 1. $u \cdot v = v \cdot u$
> 2. $u \cdot (v_1 + v_2) = u \cdot v_1 + u \cdot v_2$
> 3. $(u_1 + u_2) \cdot v = u_1 \cdot v + u_2 \cdot v$
> 4. $u \cdot u \geq 0$
> 5. $u \cdot u = 0 \iff u = 0$
> 6. $(tu) \cdot v = t(u \cdot v) = u \cdot (tv)$

## Note collegate
- [[26_Prodotto_Interno_in_Coordinate]]
- [[27_Prodotto_Esterno]]
- [[23_Sistemi_di_Riferimento_e_Coordinate]]
- Indice: [[03_Indice_Lezione_2]] · [[00_MOC_GAL]]
