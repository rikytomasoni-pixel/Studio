---
tags: [GAL, spazi-vettoriali, sottospazi, chiusura, definizione, lezione-11]
data: 2026-10-15
lezione: 11
fonte: "GAL_2026-2027_-_20261015_-_LEZIONE_11.pdf (slide 106-107)"
---

# Sottospazi vettoriali

## Osservazione: spazi contenuti in altri spazi
Tra gli esempi visti ([[92_Esempi_di_Spazi_Vettoriali]]) alcuni spazi vettoriali sono contenuti in altri:
- $\{\text{vettori geometrici di }\mathbb{R}^2\}\subseteq\{\text{vettori geometrici in }\mathbb{R}^3\}$
- $S=\{\underline{x}\in\mathbb{K}^n\mid A\underline{x}=\underline{0}\}\subseteq M_{\mathbb{K}}(n,1)\simeq\mathbb{K}^n$
- $I\subseteq\mathbb{R}$ intervallo aperto: $\mathcal{C}^0(I)=\{f:I\to\mathbb{R}\text{ continua}\}\subseteq V(I)$
- $\mathbb{K}[t]_{\leq d}=\{\text{polinomi in }\mathbb{K}[t]\text{ con grado massimo della variabile }t=d\}=\{a_0+a_1t+a_2t^2+\dots+a_dt^d\}\subseteq\mathbb{K}[t]$

## Definizione

> [!abstract] Definizione 11.3
> Sia $(V,+,\cdot)$ uno spazio vettoriale sul campo $\mathbb{K}$. Un sottoinsieme $H\neq\emptyset$ di $V$ si dice **sottospazio vettoriale** di $V$ se $H$ è uno spazio vettoriale rispetto alle operazioni **ereditate** da $V$.

Esempio: $S=\{\underline{x}\in\mathbb{K}^n\mid A\underline{x}=\underline{0}\}\subseteq\mathbb{K}^n$; per $\underline{v},\underline{w}\in S$ si studia $\underline{v}+\underline{w}$ (vedi [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]).

## Come riconosciamo un sottospazio?
> [!question] Domanda
> Come facciamo a riconoscere un sottospazio?

1. $H$ deve contenere obbligatoriamente $\underline{0}$ (**condizione necessaria**).
2. Le operazioni di $V$ devono essere **chiuse** rispetto ad $H$.

"Chiuse" significa che se parto da elementi di $H$ e uso le operazioni devo produrre nuovi elementi di $H$:
- se $\underline{v},\underline{w}\in H$ allora $\underline{v}+\underline{w}\in H$ (chiusura della somma);
- se $\underline{v}\in H$ e $\lambda\in\mathbb{K}$ allora $\lambda\underline{v}\in H$ (chiusura del prodotto per scalari).

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** slide 107. **Cosa cercare:** quattro diagrammi di Venn (un ovale $V$ che ne contiene uno più piccolo $H$). In alto: a sinistra "CHIUSO", con $\underline{v}$, $\underline{w}$ e $\underline{v}+\underline{w}$ (verde) tutti dentro $H$; a destra "NON CHIUSO", con $\underline{v}+\underline{w}$ (rosso) fuori da $H$ ma dentro $V$. In basso: lo stesso per il prodotto per scalare, $\lambda\underline{v}$ dentro $H$ (verde, chiuso) oppure fuori da $H$ (rosso, non chiuso).

## Note collegate
- [[91_Spazio_Vettoriale_Definizione]]
- [[92_Esempi_di_Spazi_Vettoriali]]
- [[93_Proprieta_Fondamentali_degli_Spazi_Vettoriali]]
- [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- Indice: [[12_Indice_Lezione_11]] · [[00_MOC_GAL]]

#GAL/spazi-vettoriali/sottospazi
