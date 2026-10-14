---
created: 2026-09-25
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Monotonia

**Definizione.** $f:A\subseteq\mathbb{R}\to\mathbb{R}$ si dice, $\forall x_1,x_2\in A$:

| Tipo | Condizione |
|---|---|
| **crescente** | $x_1<x_2\Rightarrow f(x_1)\le f(x_2)$ |
| **strettamente crescente** | $x_1<x_2\Rightarrow f(x_1)<f(x_2)$ |
| **decrescente** | $x_1<x_2\Rightarrow f(x_1)\ge f(x_2)$ |
| **strettamente decrescente** | $x_1<x_2\Rightarrow f(x_1)>f(x_2)$ |

$f$ si dice **monotona** se soddisfa una di queste 4 proprietà.

![[esempi-monotonia-quattro-grafici.png]]

**Esempio.** $f(x)=\dfrac1x$ su $(-\infty,0)\cup(0,\infty)$: **non** è monotona su $(-\infty,0)\cup(0,\infty)$, ma è strettamente decrescente in $(-\infty,0)$ e in $(0,\infty)$.

![[grafico-iperbole-1-su-x.png]]

**Osservazioni.**
- $f$ crescente **preserva** le disuguaglianze; $f$ decrescente le **inverte**.
- Caratterizzazione con il rapporto incrementale: per $x_1\neq x_2$ in $\mathcal{D}(f)$,
$$f\text{ crescente}\iff\frac{f(x_2)-f(x_1)}{x_2-x_1}\ge0,\qquad f\text{ decrescente}\iff\frac{f(x_2)-f(x_1)}{x_2-x_1}\le0.$$
Il rapporto è il coefficiente angolare $m$ della retta secante. Con «strettamente» si toglie l'uguale.

![[retta-secante-funzione-crescente.png]]

---
Precedente: [[Funzioni Pari e Dispari]] · Successivo: [[Funzioni Periodiche]]
