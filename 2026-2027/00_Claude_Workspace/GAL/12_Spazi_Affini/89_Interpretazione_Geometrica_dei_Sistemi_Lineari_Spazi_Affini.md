---
tags: [GAL, sistemi-lineari, spazi-affini, rette, piani, equazioni-cartesiane, equazioni-parametriche, lezione-11]
data: 2026-10-15
lezione: 11
fonte: "GAL_2026-2027_-_20261015_-_LEZIONE_11.pdf (slide 97-99)"
destinazione: "20_Geometria_Algebra_Lineare/12_Spazi_Affini"
---

# Interpretazione geometrica dei sistemi lineari: spazi affini

Lavoro su $\mathbb{K}=\mathbb{R}$.

| Sistema lineare | | Soluzioni |
|---|---|---|
| $A\underline{x}=\underline{b}$, $\ A\in M_{\mathbb{R}}(m,n)$, $\underline{b}\in\mathbb{R}^m$ | $\xrightarrow{\ \text{MEG, teor. R-C}\ }$ | $\underline{x}=\underline{v}_0+t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$ |
| **equazioni cartesiane** (descrizione *implicita*) | | **equazioni parametriche** (descrizione *esplicita*) |

> [!abstract] Definizione 11.1
> Un (sotto)spazio **affine** di $\mathbb{R}^n$ è l'insieme delle soluzioni di un sistema lineare $A\underline{x}=\underline{b}$.
> $$S=\{\underline{x}\in\mathbb{R}^n\mid A\underline{x}=\underline{b}\}\ \ (\text{eq. cartesiane})=\{\underline{x}=\underline{v}_0+t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}\}\ \ (\text{eq. parametriche})=\underline{v}_0+\ker(A)$$

Uso [[82_Teorema_di_Rouche_Capelli]] e [[85_Teorema_di_Struttura_delle_Soluzioni]]. Studio il caso di **rette e piani**.

## Retta
$$r=\{\underline{x}=P+t\underline{v}\mid t\in\mathbb{R}\}$$
scritta così non so dove ritrovo $r$ (con $P,\underline{v}\in\mathbb{R}^2$ in $\mathbb{R}^2$, $P,\underline{v}\in\mathbb{R}^3$ in $\mathbb{R}^3$, ...).

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** slide 97, in basso a destra. **Cosa cercare:** una retta $r$ con un punto $P$ evidenziato e il vettore direzione $\underline{v}$ (freccia viola) applicato in $P$.

Voglio passare alle equazioni cartesiane: $r=\{\underline{x}\in\mathbb{R}^n\mid A\underline{x}=\underline{b}\}$.

> [!question] Domanda
> Quante equazioni devo determinare, cioè quante righe ha $A\in M_{\mathbb{R}}(?,n)$? Più precisamente, quante equazioni **non ridondanti**: $A\in M_{\mathbb{R}}(r,n)$?

**Risposta.** $r=\{\underline{x}=P+t\underline{v}\}$ $\xrightarrow{\text{R-C}}$ ho **1 parametro libero**, inoltre $1=n-r$, cioè $r=n-1$.
- $n=2$, piano euclideo: una retta è descritta da $2-1=1$ equazione cartesiana
- $n=3$, spazio euclideo: una retta è descritta da $3-1=2$ equazioni cartesiane
- in $\mathbb{R}^n$: una retta è descritta da $n-1$ equazioni cartesiane

## Piano
$$\alpha=\{\underline{x}=P+t_1\underline{v}+t_2\underline{w}\}$$
Un piano è caratterizzato da **2 parametri liberi**.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** slide 98, in basso a destra. **Cosa cercare:** un piano (parallelogramma verde in prospettiva) con il punto $P$, i vettori $\underline{v}$ e $\underline{w}$ applicati in $P$ e il vettore somma tratteggiato come diagonale del parallelogramma.

$\alpha=\{\underline{x}\in\mathbb{R}^n\mid A\underline{x}=\underline{b}\}$, con $A\in M_{\mathbb{R}}(?,n)$. Per Rouché-Capelli: $2=n-r\Rightarrow r=n-2$.
- in $\mathbb{R}^2$: $2-2=0$ equazioni (il piano è tutto $\mathbb{R}^2$)
- in $\mathbb{R}^3$: $3-2=1$ equazione cartesiana
- in $\mathbb{R}^n$: un piano è descritto da $n-2$ equazioni cartesiane

## Note collegate
- [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[85_Teorema_di_Struttura_delle_Soluzioni]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[23_Sistemi_di_Riferimento_e_Coordinate]]
- [[22_Operazioni_tra_Vettori]]
- Indice: [[12_Indice_Lezione_11]] · [[00_MOC_GAL]]

#GAL/spazi-affini/interpretazione-geometrica-sistemi
