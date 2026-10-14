---
created: 2026-10-07
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/rango_e_determinante
aliases: []
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Matrici Triangolari

**(II) Definizione 6.5** — Una matrice $T \in M_{\mathbb{K}}(n,n)$ si dice

- **triangolare superiore** se $t_{ij} = 0\ \ \forall i > j$;
- **triangolare inferiore** se $t_{ij} = 0\ \ \forall i < j$.

> **Figura (disegno senza immagine disponibile):**
>
> Due matrici $n\times n$. A sinistra «TRIANG. SUP.»: diagonale $t_{11}, t_{22}, \dots, t_{nn}$, asterischi sopra la diagonale e zeri sotto. A destra «TRIANG. INF.»: zeri sopra la diagonale e asterischi sotto. In basso, una matrice triangolare superiore generica con la prima colonna evidenziata in blu (tutti zeri sotto $t_{11}$).

> **Osservazione**: $\{\text{matrici diagonali}\} \subseteq \{\text{matrici triang. sup.}\}$ e $\{\text{matrici diagonali}\} \subseteq \{\text{matrici triang. inf.}\}$.

### Determinante di una matrice triangolare

Sviluppando lungo la prima colonna ($j=1$) di una triangolare superiore $T$:

$$
\det(T) = \sum_{i=1}^{n}(-1)^{i+1}t_{i1}\det(\hat{T}_{i1}) = (-1)^{1+1}t_{11}\det(\hat{T}_{11}) + 0 + 0 + \dots + 0 = t_{11}\det(\hat{T}_{11})
$$

dove $\hat{T}_{11}$ è ancora triangolare superiore. Iterando:

$$
\det(T) = t_{11}\,t_{22}\cdots t_{nn}
$$

Il determinante di una matrice triangolare è il **prodotto degli elementi diagonali**.

**Recap degli obiettivi**:

1. calcolare le matrici inverse;
2. calcolare il rango;
3. calcolare il determinante usando le matrici triangolari.

---
Precedente: [[Determinante e Sviluppo di Laplace]] · Successivo: [[Teorema di Binet]]
