---
created: 2026-09-30
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
origine: UpdateVault
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Il Campo F2

> [!note] Osservazione
> Il codominio delle funzioni è sempre stato un insieme di numeri. D'ora in poi prenderemo come codominio un **campo numerico**: $\mathbb{Q}$, $\mathbb{R}$, $\mathbb{C}$, $\mathbb{F}_2$ (campo finito).

> [!warning] Def. Il campo $\mathbb{F}_2$
> $\mathbb{F}_2 = \{0,1\}$, dove $0$ = falso (interruttore aperto, rosso) e $1$ = vero (interruttore chiuso, verde).

**XOR** — «o uno o l'altro ma non entrambi» (somma in $\mathbb{F}_2$): circuito con batteria, due deviatori in serie e lampadina.

**DISEGNO NON RAPPRESENTABILE** (disegno: circuito XOR con due deviatori e lampadina; tabella 2×2 con i quattro casi: $0+0 \to 0$ (spenta), $0+1 \to 1$ (accesa), $1+0 \to 1$ (accesa), $1+1 \to 0$ (spenta)) *(dove cercarlo: GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 25-26))*

**AND** — «sia l'uno che l'altro» [OCR: «né»; lettura di senso corretta] (prodotto in $\mathbb{F}_2$): circuito con batteria, due interruttori in serie e lampadina.

**DISEGNO NON RAPPRESENTABILE** (disegno: circuito AND con due interruttori e lampadina; tabella 2×2 con i quattro casi: $0\cdot 0 \to 0$, $0 \cdot 1 \to 0$, $1 \cdot 0 \to 0$, $1 \cdot 1 \to 1$ (accesa)) *(dove cercarlo: GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 25-26))*

> [!warning] Def. Operazioni in $\mathbb{F}_2$
>
> | $+$ | 0 | 1 |
> |---|---|---|
> | **0** | 0 | 1 |
> | **1** | 1 | 0 |
>
> | $\cdot$ | 0 | 1 |
> |---|---|---|
> | **0** | 0 | 0 |
> | **1** | 0 | 1 |

---
Precedente: [[Matrici come Rappresentazione di Funzioni]] · Successivo: [[Definizione di Matrice]]
