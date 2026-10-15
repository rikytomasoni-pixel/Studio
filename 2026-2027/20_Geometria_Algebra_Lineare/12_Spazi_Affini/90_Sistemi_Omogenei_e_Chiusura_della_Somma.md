---
tags: [GAL, sistemi-omogenei, spazi-affini, chiusura, motivazione-spazi-vettoriali, lezione-11]
data: 2026-10-15
lezione: 11
fonte: "GAL_2026-2027_-_20261015_-_LEZIONE_11.pdf (slide 99-101)"
---

# Sistemi omogenei e chiusura rispetto alla somma

Concentriamoci sui sistemi **omogenei**:
$$S=\{\underline{x}\in\mathbb{R}^n\mid A\underline{x}=\underline{0}\}=\{\underline{x}=\underline{0}+t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}\}$$

## Cosa cambia nella geometria?
- **Retta:** $r=\{\underline{x}=\underline{0}+t\underline{v}\}$: la retta passa per l'**origine** del sistema di riferimento.
- **Piano:** $\alpha=\{\underline{x}=\underline{0}+t_1\underline{v}+t_2\underline{w}\}$: $\alpha$ è un piano che passa per l'origine.
- Dal punto di vista dei sistemi: $\underline{x}=\underline{0}$ è soluzione del sistema, $A\underline{0}=\underline{0}$.

## Cosa cambia dal punto di vista algebrico?
$S=\{\underline{x}\in\mathbb{R}^n\mid A\underline{x}=\underline{0}\}$. Siano $\underline{v},\underline{w}\in S$: è vero che $\underline{v}+\underline{w}\in S$?
$$A(\underline{v}+\underline{w})=A\underline{v}+A\underline{w}=\underline{0}+\underline{0}=\underline{0}\ \Rightarrow\ \underline{v}+\underline{w}\in S$$
è ancora una soluzione del sistema.

In generale **non abbiamo questa fortuna**. Ad esempio per
$$T=\{\underline{x}\in\mathbb{R}^n\mid A\underline{x}=\underline{b}\neq\underline{0}\}$$
con $\underline{v},\underline{w}\in T$ e $\underline{x}=\underline{v}+\underline{w}$:
$$A(\underline{v}+\underline{w})=A\underline{v}+A\underline{w}=\underline{b}+\underline{b}=2\underline{b}\neq\underline{b}$$
$\underline{v}+\underline{w}$ **non** è soluzione del sistema.

## Punto di vista geometrico
- $r=\{\underline{x}=\underline{0}+t\underline{v}\}$ (retta per l'origine): la somma $\underline{v}+\underline{w}$ di due suoi vettori sta ancora sulla retta.
- $s=\{\underline{x}=P+t\underline{v}\}$ (retta che non passa per l'origine): la somma $\underline{v}+\underline{w}$ di due suoi vettori **esce** dalla retta.

![[sommaDiVettoriSpostamento.png]]

## "Pronti per il primo vero salto concettuale"

![[Mordor.png]]

I tre esempi (matrici, vettori geometrici, soluzioni di un sistema omogeneo) hanno in comune l'esistenza di una somma e di un prodotto per scalari ben comportati: da qui nasce lo spazio vettoriale.

## Note collegate
- [[89_Interpretazione_Geometrica_dei_Sistemi_Lineari_Spazi_Affini]]
- [[91_Spazio_Vettoriale_Definizione]]
- [[94_Sottospazi_Vettoriali]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[22_Operazioni_tra_Vettori]]
- [[35_Somma_tra_Matrici]]
- Indice: [[12_Indice_Lezione_11]] · [[00_MOC_GAL]]

#GAL/spazi-affini/sistemi-omogenei-e-chiusura
