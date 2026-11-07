---
tags: [GAL, base, estrazione, completamento, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 126)"
---

# Due problemi classici: estrazione e completamento

> [!abstract] I due problemi
> - **(I) Estrazione:** trovare una base a partire da un insieme di generatori.
> - **(II) Completamento:** costruire una base a partire da un insieme di vettori linearmente indipendenti.

Entrambi si risolvono con il [[68_Metodo_di_Eliminazione_di_Gauss|MEG]], leggendo i vettori in due modi diversi:

| Problema | Strategia | Nota |
|---|---|---|
| (I) con **costruzione libera** (i vettori della base possono essere diversi da quelli dati) | MEG sulle **righe** | [[123_Base_per_Costruzione_Libera_con_il_MEG_sulle_Righe]] |
| (I) con **estrazione** (la base è formata da vettori tra quelli dati) | MEG sulle **colonne** (pivot) | [[124_Estrazione_di_una_Base_con_i_Pivot_delle_Colonne]] |
| (II) completamento | estrazione da {indipendenti} $\cup$ {base canonica} | [[125_Completamento_ad_una_Base]] |

## Esempio guida (slide 126)
In $\mathbb{R}^3$ sia
$$V=\operatorname{Span}\left(\begin{bmatrix}1\\-1\\0\end{bmatrix},\begin{bmatrix}0\\1\\2\end{bmatrix},\begin{bmatrix}1\\0\\2\end{bmatrix}\right)$$
La richiesta può essere formulata come:
- «Determina una base di $V$»
- «Estrai una base di $V$»

Lo svolgimento è in [[123_Base_per_Costruzione_Libera_con_il_MEG_sulle_Righe]].

## Note collegate
- [[100_Base_di_uno_Spazio_Vettoriale]]
- [[96_Insieme_di_Generatori]]
- [[121_Basi_Canoniche]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/base/estrazione-completamento
