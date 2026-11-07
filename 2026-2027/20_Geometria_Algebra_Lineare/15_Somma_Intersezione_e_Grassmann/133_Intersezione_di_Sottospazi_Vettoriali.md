---
tags: [GAL, sottospazi, intersezione, lezione-16]
data: 2026-11-04
lezione: 16
fonte: "GAL 2026-2027 - 20261104 - LEZIONE 16.pdf (slide 139)"
---

# Intersezione di sottospazi vettoriali

**Obiettivo.** Indagare l'analogo per sottospazi vettoriali e dimensione della formula di additività delle aree ([[132_Significato_della_Dimensione_Seconda_Parte]]):
- cosa vuol dire fare l'unione di due sottospazi?
- cosa vuol dire fare l'intersezione di due sottospazi?
- c'è un analogo della formula di addizione delle aree?

## Intersezione
Sia $(V,+,\cdot)$ uno spazio vettoriale e siano $H,K$ sottospazi vettoriali. Considero l'intersezione di $H$ e $K$ come insiemi e verifico che $H\cap K$ è chiuso rispetto alle operazioni.

**Somma.**
$$\underline{v},\underline{w}\in H\cap K\iff\begin{cases}\underline{v},\underline{w}\in H\\ \underline{v},\underline{w}\in K\end{cases}\Rightarrow\begin{cases}\underline{v}+\underline{w}\in H\\ \underline{v}+\underline{w}\in K\end{cases}\iff\underline{v}+\underline{w}\in H\cap K$$
($H,K$ sono chiusi per la somma.)

**Prodotto per scalari.**
$$\underline{v}\in H\cap K,\ \lambda\in\mathbb{K}\iff\begin{cases}\underline{v}\in H,\ \lambda\in\mathbb{K}\\ \underline{v}\in K,\ \lambda\in\mathbb{K}\end{cases}\Rightarrow\begin{cases}\lambda\underline{v}\in H\\ \lambda\underline{v}\in K\end{cases}\iff\lambda\underline{v}\in H\cap K$$

Quindi l'intersezione di due sottospazi è chiusa rispetto a somma e prodotto per scalari ([[94_Sottospazi_Vettoriali]]).

> [!note] Osservazione (non presente negli appunti)
> Per concludere che $H\cap K$ è un **sottospazio** serve anche $\underline{0}\in H\cap K$, che vale perché $\underline{0}\in H$ e $\underline{0}\in K$.

## Note collegate
- [[94_Sottospazi_Vettoriali]]
- [[134_Unione_di_Sottospazi_e_Sottospazio_Somma]]
- [[135_Formula_di_Grassmann_Teorema_16_3]]
- [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]
- Indice: [[17_Indice_Lezione_16]] · [[00_MOC_GAL]]

#GAL/sottospazi/intersezione
