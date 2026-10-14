---
created: 2026-09-30
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Il Campo F2

Ora definiamo le matrici in generale.

**Caratteristiche comuni**: abbiamo studiato funzioni con dominio un prodotto cartesiano di insiemi **finiti**; il codominio delle funzioni è sempre stato un insieme di numeri. D'ora in poi prenderemo come codominio un **campo numerico**: $\mathbb{Q}$, $\mathbb{R}$, $\mathbb{C}$, $\mathbb{F}_2$ (campo finito).

**Notazione**: $[m] = \{1,2,\dots,m\}$ e $[n] = \{1,2,\dots,n\}$, quindi

$$
[m] \times [n] = \{(1,1),(1,2),\dots,(1,n),\ (2,1),(2,2),\dots,(2,n),\ \dots,\ (m,1),(m,2),\dots,(m,n)\}
$$

### Il campo $\mathbb{F}_2 = \{0,1\}$

$0$ = falso (interruttore aperto), $1$ = vero (interruttore chiuso).

- **XOR** («o uno o l'altro ma non entrambi»): realizzato con due deviatori in serie; la lampadina è accesa se i due deviatori sono in posizioni diverse. Corrisponde alla **somma** $+$ in $\mathbb{F}_2$.
- **AND** («sia l'uno che l'altro»): realizzato con due interruttori in serie; la lampadina è accesa solo se entrambi sono chiusi. Corrisponde al **prodotto** $\cdot$ in $\mathbb{F}_2$.

> **Figura (disegno senza immagine disponibile):**
>
> Due schemi di circuito (batteria "+ −", due elementi in serie, lampadina). Sopra il circuito XOR con due *deviatori* e sotto il circuito AND con due *interruttori*, ciascuno con la tabella a doppia entrata (0 rosso = interruttore aperto/falso, 1 verde = chiuso/vero) e lampadina accesa/spenta. Per XOR: $0,0 \to 0$; $0,1 \to 1$; $1,0 \to 1$; $1,1 \to 0$. Per AND: acceso solo per $1,1$.

Operazioni in $\mathbb{F}_2$:

| $+$ | 0 | 1 |
|:-:|:-:|:-:|
| **0** | 0 | 1 |
| **1** | 1 | 0 |

| $\cdot$ | 0 | 1 |
|:-:|:-:|:-:|
| **0** | 0 | 0 |
| **1** | 0 | 1 |

---
Precedente: [[Matrici come Rappresentazione di Funzioni]] · Successivo: [[Definizione di Matrice]]
