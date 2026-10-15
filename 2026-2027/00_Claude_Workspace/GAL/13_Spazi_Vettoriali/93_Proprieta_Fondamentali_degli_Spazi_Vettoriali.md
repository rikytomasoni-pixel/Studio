---
tags: [GAL, spazi-vettoriali, proprieta, calcolo, motivazione, lezione-11]
data: 2026-10-15
lezione: 11
fonte: "GAL_2026-2027_-_20261015_-_LEZIONE_11.pdf (slide 104-105)"
destinazione: "20_Geometria_Algebra_Lineare/13_Spazi_Vettoriali"
---

# Perché gli spazi vettoriali: proprietà fondamentali e calcolo

> [!question] Domanda
> Perché gli spazi vettoriali ricoprono un ruolo fondamentale nella matematica e nelle sue applicazioni?

**R1.** Gli spazi vettoriali sono un contesto in cui la nostra **intuizione funziona bene**.

### Fenomeni "noti" (valgono in ogni spazio vettoriale $V$, vedi [[91_Spazio_Vettoriale_Definizione]])
- $\forall\,\underline{v}\in V:\ \ 0\,\underline{v}=\underline{0}$
- L'elemento opposto di $\underline{v}$ è $(-1)\underline{v}=-\underline{v}$:
$$\underline{v}+(-1)\underline{v}=1\,\underline{v}+(-1)\underline{v}=(1+(-1))\underline{v}=0\,\underline{v}=\underline{0}$$
- Vale la **legge di annullamento del prodotto**:
$$\lambda\underline{v}=\underline{0}\ \Rightarrow\ \lambda=0\ \text{ oppure }\ \underline{v}=\underline{0}$$

**R2.** Gli spazi vettoriali sono uno dei pochi contesti in cui riusciamo a fare **calcoli in maniera molto efficace**!

Posso risolvere equazioni lineari che coinvolgono gli elementi di uno spazio vettoriale:
- $\underline{v}\in V$ assegnato, $\lambda\neq0$, $\mu\in\mathbb{K}$
- cerco $\underline{x}\in V$ tale che $\lambda\underline{x}+\mu\underline{v}=\underline{0}$

La soluzione è
$$\underline{x}=-\frac{\mu}{\lambda}\,\underline{v}$$

> [!todo] Per casa
> Scrivere tutti i passaggi che servono per passare da $\lambda\underline{x}+\mu\underline{v}=\underline{0}$ a $\underline{x}=-\frac{\mu}{\lambda}\underline{v}$ e capire quali delle proprietà tra (V1)-(V8) garantiscono che il passaggio sia legittimo.
>
> *(Primo passaggio indicato alla lavagna: sommare $(-\mu\underline{v})$ a entrambi i membri, $\lambda\underline{x}+\mu\underline{v}+(-\mu\underline{v})=\underline{0}+(-\mu\underline{v})$.)*

## Note collegate
- [[91_Spazio_Vettoriale_Definizione]]
- [[92_Esempi_di_Spazi_Vettoriali]]
- [[94_Sottospazi_Vettoriali]]
- [[Kanban_Esercizi_per_Casa]]
- Indice: [[12_Indice_Lezione_11]] · [[00_MOC_GAL]]

#GAL/spazi-vettoriali/proprieta-fondamentali
