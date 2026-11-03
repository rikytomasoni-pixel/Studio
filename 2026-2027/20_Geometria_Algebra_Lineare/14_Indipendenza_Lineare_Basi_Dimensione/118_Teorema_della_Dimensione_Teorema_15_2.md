---
tags: [GAL, dimensione, base, teorema, dimostrazione, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 121-122)"
---

# Teorema della dimensione (Teorema 15.2)

> [!abstract] Teorema 15.2 (teorema della dimensione)
> **Ipotesi:** $(V,+,\cdot)$ spazio vettoriale su un campo $\mathbb{K}$; $T=\{\underline{v}_1,\dots,\underline{v}_m\}$ e $S=\{\underline{w}_1,\dots,\underline{w}_n\}$ sono [[100_Base_di_uno_Spazio_Vettoriale|basi]] di $V$.
>
> **Tesi:** $m=n$.

In parole: **tutte le basi di $V$ hanno lo stesso numero di elementi**.

## Dimostrazione
$$m=n\iff\begin{cases}n\ge m\\ m\ge n\end{cases}$$

Applico il [[117_Lemma_Fondamentale_Teorema_15_1|lemma fondamentale]]: se $T$ è un insieme di generatori e $S$ è qualsiasi, allora
$$\#\text{elementi di }S>\#\text{elementi di }T\ \Rightarrow\ S\text{ linearmente dipendente}$$
cioè, per contrapposizione,
$$\#\text{elementi di }S\le\#\text{elementi di }T\ \Longleftarrow\ S\text{ linearmente indipendente}$$

$T$ ed $S$ nel teorema sono **sia** generatori **sia** linearmente indipendenti (sono basi). Due casi:

| Caso | Ruoli | Conclusione |
|---|---|---|
| **1** | $T$ generatori, $S$ linearmente indipendenti | $n\le m$ |
| **2** | $S$ generatori, $T$ linearmente indipendenti | $m\le n$ |

Quindi $m=n$. $\blacksquare$

> [!note] Osservazione (non presente negli appunti)
> Questo teorema giustifica la [[102_Dimensione_di_uno_Spazio_Vettoriale|Definizione 13.6]]: la dimensione, definita come numero di elementi di una base, **non dipende dalla base scelta**. Chiude quindi il punto aperto lasciato dalla lezione 13.

## Note collegate
- [[117_Lemma_Fondamentale_Teorema_15_1]]
- [[100_Base_di_uno_Spazio_Vettoriale]]
- [[102_Dimensione_di_uno_Spazio_Vettoriale]]
- Successiva: [[119_Significato_della_Dimensione_Massimo_Indipendenti_e_Minimo_Generatori]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/dimensione/teorema-della-dimensione
