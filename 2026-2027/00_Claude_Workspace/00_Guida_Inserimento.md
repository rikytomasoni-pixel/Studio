---
tags: [guida, claude-workspace, revisione]
data: 2026-10-15
---

# Guida all'inserimento — Claude Workspace (15-10-2026)

Note create da: **AM1 L10** (14-10), **GAL L9** (12-10), **GAL L10** (14-10), **GAL L11** (15-10). Tutto è in `00_Claude_Workspace` in attesa di revisione. I MOC esistenti **non sono stati modificati**: le proposte sono in [[00_Proposta_Aggiornamento_MOC_GAL]] e [[00_Proposta_Aggiornamento_MOC_Analisi_1]]. Gli esercizi per casa sono nel [[Kanban_Esercizi_per_Casa]].

## Dove metterei le note, una volta rivisionate

| Cartella nel workspace | Dove la metterei | Note | Motivo |
|---|---|---|---|
| `GAL/11_Sistemi_Lineari` | `20_Geometria_Algebra_Lineare`, **nuova** cartella `11_Sistemi_Lineari` | 80-86 | Argomento distinto da Matrici/Rango/Determinante: l'ultima in ordine è dedicata ai sistemi lineari |
| `GAL/04_Matrice_Inversa` | `20_Geometria_Algebra_Lineare/04_Matrice_Inversa` (già esistente) | 87-88 | Completano il tema dell'inversa (L6-L7) |
| `GAL/12_Spazi_Affini` | `20_Geometria_Algebra_Lineare`, **nuova** cartella `12_Spazi_Affini` | 89-90 | Ponte geometrico tra sistemi e spazi vettoriali |
| `GAL/13_Spazi_Vettoriali` | `20_Geometria_Algebra_Lineare`, **nuova** cartella `13_Spazi_Vettoriali` | 91-94 | Inizio della parte astratta del corso |
| `GAL/10_Indici_Lezioni` | `20_Geometria_Algebra_Lineare/10_Indici_Lezioni` (già esistente) | 10-12 (indici L9-L11) | Proseguono la numerazione degli indici |
| `Analisi_1/05_Successioni_e_Limiti` | `10_Analisi_1/05_Successioni_e_Limiti` (già esistente) | 43-46 | Proseguono i confronti asintotici (L9) |
| `Analisi_1/06_Serie` | `10_Analisi_1`, **nuova** cartella `06_Serie` | 47-55 | Argomento distinto: le serie |
| `Kanban_Esercizi_per_Casa.md` | `00_Claude_Workspace` o una cartella a scelta (es. `99_Tools`) | — | Utile per tutte le materie |

I quattro PDF originali sono già in `90_Lezioni_pdf/A1` e `90_Lezioni_pdf/GAL`, non serve spostarli.

## Cose da controllare in revisione
- [[82_Teorema_di_Rouche_Capelli]]: un `<DUBBIO>` sulla lettera $n$/$m$ in TH2 (slide 78).
- Note con `DISEGNO NON RAPPRESENTABILE` (screenshot da fare, suggerisco `99_Tools/Screenshots/GAL/` o `.../Analisi1/Serie/`): [[81_Risoluzione_di_un_Sistema_con_MEG_Esempio_Parametrico]], [[89_Interpretazione_Geometrica_dei_Sistemi_Lineari_Spazi_Affini]], [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]], [[94_Sottospazi_Vettoriali]], [[47_Serie_Introduzione_e_Somme_Parziali]], [[50_Serie_Geometrica]], [[55_Serie_Armonica]].
- Una nota con un commento mio esplicitamente marcato come aggiunto: [[43_Asintotici_con_Funzioni_Composte]].
- Non esiste una Lezione 8 di GAL (la numerazione delle slide passa da 72 a 73).

## Vista Dataview delle note del workspace

```dataview
TABLE data, destinazione
FROM "00_Claude_Workspace"
WHERE destinazione
SORT destinazione ASC, file.name ASC
```

#guida
