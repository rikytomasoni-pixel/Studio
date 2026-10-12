---
tags: [GAL, matrici, MEG, algoritmo, gauss, lezione-6]
data: 2026-10-07
lezione: 6
fonte: "GAL_2026-2027_-_20261007_-_LEZIONE_6.pdf (slide 56-60)"
---

# Metodo di eliminazione di Gauss (MEG)

> [!warning] Def. Metodo di eliminazione di Gauss (MEG) — input e output
> - **INPUT** $A \in M_{\mathbb{K}}(m,n)$ qualsiasi
> - $?\ \Downarrow\ ?$ (trasformazione da determinare)
> - **OUTPUT** $U \in M_{\mathbb{K}}(m,n)$ «con informazione concentrata nella parte in alto a destra» (se $m = n$, l'output sono matrici triangolari superiori, vedi [[66_Matrici_Triangolari]])
>
> D. per passare da INPUT a OUTPUT posso usare una sequenza di 3 operazioni elementari → [[67_Operazioni_Elementari_sulle_Righe]].

## Algoritmo MEG
**Casi base:**
- $A = \underline{0} \leadsto U = \underline{0}$
- $A \in M_{\mathbb{K}}(1,n) \leadsto U = A$

Possiamo supporre $m > 1$ e $A \neq \underline{0}$.

**STEP 1** — identifico l'indice $j$ della prima colonna non nulla di $A$.
$$A = \begin{bmatrix} 0 & \cdots & 0 & \neq 0 & \ast & \ast \\ \vdots & & \vdots & \vdots & & \\ 0 & \cdots & 0 & \ast & \ast & \ast \end{bmatrix}$$
**STEP 2** — scelgo (arbitrariamente) una riga $i$ tale che $a_{ij} \neq 0$.

![[Step2MEG.png]]

**STEP 3** — scambio la prima riga con la $i$-esima: $R_1(A) \leftrightarrow R_i(A)$.
![[Step3MEG.png]]

**STEP 4** — elimino tutte le entrate non nulle sotto $p_1$ con una sequenza di operazioni del terzo tipo:
$$R_i - \frac{a_{ij}}{p_1} R_1 \to R_i$$

![[Step4MEG.png]]

Al termine dello step 4 la matrice ha la seguente forma:
![[Step4BMEG.png]]

**STEP 5** — estraggo dalla matrice con $m$ righe e $n$ colonne la matrice con $m-1$ righe e $n$ colonne ottenuta tralasciando la prima riga e riparto da capo.

> [!note] Osservazione
> - l'algoritmo termina sempre in un numero finito di passi;
> - nell'algoritmo ci sono due scelte arbitrarie per cui l'output non è univocamente determinato.

> [!example] Esempio
> **Input** $A = \begin{bmatrix} 0 & 0 & 2 & 0 \\ 1 & 0 & 1 & -1 \\ 2 & 0 & 1 & 4 \end{bmatrix}$, $\quad m = 3 > 1$, $A \neq \underline{0}$
>
> - **STEP 1** la prima colonna non nulla è la colonna $1$ (riquadro blu).
> - **STEP 2** scelgo la riga $2$ oppure la riga $3$ (riquadro verde).
> - **STEP 3** sposto la seconda riga in prima posizione:
> $$\begin{bmatrix} 0 & 0 & 2 & 0 \\ 1 & 0 & 1 & -1 \\ 2 & 0 & 1 & 4 \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} 1 & 0 & 1 & -1 \\ 0 & 0 & 2 & 0 \\ 2 & 0 & 1 & 4 \end{bmatrix} \qquad (1 = p_1)$$
> - **STEP 4**
> $$\begin{bmatrix} 1 & 0 & 1 & -1 \\ 0 & 0 & 2 & 0 \\ 2 & 0 & 1 & 4 \end{bmatrix} \xrightarrow{\ \mathrm{III} - \frac{2}{1}\mathrm{I} \to \mathrm{III}\ } \begin{bmatrix} 1 & 0 & 1 & -1 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & -1 & 6 \end{bmatrix}$$
> - **STEP 5** si estrae la sottomatrice $\begin{bmatrix} 0 & 0 & 2 & 0 \\ 0 & 0 & -1 & 6 \end{bmatrix}$ (riquadro viola) e si riparte:
> - **STEP 1** la prima colonna non nulla è la colonna $3$.
> - **STEP 2** scelgo la riga con $2$ oppure quella con $-1$.
> - **STEP 3**
> $$\begin{bmatrix} 1 & 0 & 1 & -1 \\ 0 & 0 & 2 & 0 \\ 0 & 0 & -1 & 6 \end{bmatrix} \xrightarrow{\ \mathrm{II} \leftrightarrow \mathrm{III}\ } \begin{bmatrix} 1 & 0 & 1 & -1 \\ 0 & 0 & -1 & 6 \\ 0 & 0 & 2 & 0 \end{bmatrix} \qquad (1 = p_1,\ -1 = p_2)$$
> - **STEP 4**
> $$\begin{bmatrix} 1 & 0 & 1 & -1 \\ 0 & 0 & -1 & 6 \\ 0 & 0 & 2 & 0 \end{bmatrix} \xrightarrow{\ \mathrm{III} - \frac{2}{-1}\mathrm{II} \to \mathrm{III}\ } \begin{bmatrix} 1 & 0 & 1 & -1 \\ 0 & 0 & -1 & 6 \\ 0 & 0 & 0 & 12 \end{bmatrix}$$

![[MEGEsempio.png]]
L'output è una matrice a scala ([[69_Pivot_e_Matrice_a_Scala]]).

## Note collegate
- [[67_Operazioni_Elementari_sulle_Righe]]
- [[69_Pivot_e_Matrice_a_Scala]]
- [[66_Matrici_Triangolari]]
- [[73_MEG_e_Rango]]
- [[70_Reversibilita_del_MEG]]
- Indice: [[07_Indice_Lezione_6]] · [[00_MOC_GAL]]
