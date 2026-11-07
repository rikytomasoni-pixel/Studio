---
tags: [GAL, determinante, sintesi, MEG, laplace]
data: 2026-10-09
lezione: esercizi
fonte: "esempideterminante.pdf (pag. 1) — sintesi delle osservazioni sull'Esercizio 5.1"
---

# Confronto tra i metodi di calcolo del determinante

Sintesi dei tre metodi visti sulla stessa matrice $A$ ([[103_Esercizio_5_1_Calcolo_del_Determinante]]).

| Metodo | Come | Cosa tenere d'occhio | Nota |
|---|---|---|---|
| **MEG** | si riduce a $U$ triangolare, $\det(A)=(-1)^s\prod u_{ii}$ | contare gli scambi di righe ($s$) | [[104_Determinante_con_il_MEG_Esempio_con_Scambio_di_Righe]] |
| **Laplace** | $\det(A)=\sum_j a_{ij}C_{ij}$ su una riga/colonna | segni $(-1)^{i+j}$ e minori | [[105_Determinante_Laplace_Esempio_3x3_Riga_3]] |
| **Misto** | un passo di MEG + Laplace sulla colonna ripulita | niente scambi se il pivot è già in alto | [[106_Determinante_Metodo_Misto_MEG_e_Laplace]] |

## Regole da ricordare
- Sostituzione $R_i+\lambda R_k\to R_i$: $\det$ invariato ([[78_Determinante_e_Sostituzione]]).
- Scambio di due righe: $\det$ cambia segno ([[76_Determinante_Normalizzato_e_Alternante]]).
- Matrice triangolare: $\det$ = prodotto degli elementi diagonali ([[66_Matrici_Triangolari]]).
- Riga o colonna di zeri, o due righe uguali: $\det=0$ ([[65_Determinante_Sviluppo_di_Laplace]], [[79_Determinante_con_Righe_Uguali]]).

> [!note] Osservazioni (non presenti negli appunti)
> - Laplace puro su una matrice $n\times n$ senza zeri richiede il calcolo di $n$ determinanti $(n-1)\times(n-1)$, e così via a cascata: il numero di operazioni cresce come $n!$. Il MEG cresce come $n^3$. Per questo l'Esercizio 5.1 chiede la riduzione a triangolare per $B$ ($4\times4$) e $C$ ($5\times5$).
> - Laplace resta comodo per matrici piccole ($3\times3$) o con righe/colonne quasi tutte nulle.
> - Il metodo misto è il compromesso: poche sostituzioni per creare zeri, poi Laplace.
> - Come controllo, conviene calcolare lo stesso determinante con due metodi diversi, come fatto per $A$.

## Note collegate
- [[103_Esercizio_5_1_Calcolo_del_Determinante]]
- [[75_Calcolo_del_Determinante_con_il_MEG]]
- [[74_Teorema_di_Binet]]
- [[00_MOC_GAL]]

#GAL/determinante/confronto-metodi-calcolo-determinante
