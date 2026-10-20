---
tags: [GAL, indipendenza-lineare, definizione, lezione-13]
data: 2026-10-19
lezione: 13
fonte: "GAL_2026-2027_-_20261019_-_LEZIONE_13.pdf (slide 114)"
---

# Vettori linearmente indipendenti

> [!abstract] Definizione 13.3
> Sia $(V,+,\cdot)$ uno spazio vettoriale su un campo $\mathbb{K}$. Un insieme di vettori $\{\underline{v}_1,\dots,\underline{v}_n\}$ si dice **insieme di vettori linearmente indipendenti** se
> $$\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n=\underline{0}\ \Longrightarrow\ \lambda_1=\dots=\lambda_n=0$$

> [!note] N.B. Perché la definizione ha senso
> $\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$ è un sottospazio vettoriale ([[95_Combinazioni_Lineari_e_Span]]) $\Rightarrow$ $\underline{0}\in\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$.
> - So che $\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n=\underline{0}$ è risolubile;
> - so che $\lambda_1=\dots=\lambda_n=0$ è una soluzione.

"Essere linearmente indipendenti" equivale a: $\lambda_1=\dots=\lambda_n=0$ è l'**unica** soluzione di $\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n=\underline{0}$.

Se la soluzione **non** è unica, si parla di vettori **linearmente dipendenti**.

Per un esempio concreto vedi [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]].

## Note collegate
- [[95_Combinazioni_Lineari_e_Span]]
- [[96_Insieme_di_Generatori]]
- [[94_Sottospazi_Vettoriali]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- Successiva: [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]]
- Indice: [[14_Indice_Lezione_13]] · [[00_MOC_GAL]]

#GAL/indipendenza-lineare/definizione
