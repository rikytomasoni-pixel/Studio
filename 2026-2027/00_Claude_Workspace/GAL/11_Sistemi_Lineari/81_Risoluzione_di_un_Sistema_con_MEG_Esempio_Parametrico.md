---
tags: [GAL, sistemi-lineari, MEG, esempio, parametri, lezione-9]
data: 2026-10-12
lezione: 9
fonte: "GAL_2026-2027_-_20261012_-_LEZIONE_9.pdf (slide 76-77)"
destinazione: "20_Geometria_Algebra_Lineare/11_Sistemi_Lineari"
---

# Risoluzione di un sistema con il MEG: esempio con parametri

## Esempio
$$\begin{cases} 3x-2y=1 \\ 6x+ay=b \end{cases}\qquad x,y \text{ incognite};\quad a,b\in\mathbb{R}\text{ parametri}$$

Rappresentazione del III tipo ([[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]):
$$\left[\begin{array}{cc|c} 3 & -2 & 1 \\ 6 & a & b \end{array}\right]\in M_{\mathbb{R}}(2,2+1)=M_{\mathbb{R}}(2,3)$$

**Quale metodo risolutivo?** confronto, sostituzione, **riduzione** (scelto, in forma matriciale con il [[68_Metodo_di_Eliminazione_di_Gauss]]).

$\mathrm{II}-2\,\mathrm{I}\to\mathrm{II}$:
$$\begin{cases} 3x-2y=1 \\ (a+4)y=b-2 \end{cases}\ \longleftrightarrow\ \left[\begin{array}{cc|c} 3 & -2 & 1 \\ 0 & a+4 & b-2 \end{array}\right]$$

## Discussione dei casi

**Caso $a+4=0$, cioè $a=-4$:**
$$\left[\begin{array}{cc|c} 3 & -2 & 1 \\ 0 & 0 & b-2 \end{array}\right]$$

- $b-2=0$: $\left[\begin{array}{cc|c} 3 & -2 & 1 \\ 0 & 0 & 0 \end{array}\right]$
  - (1) sì, il sistema è risolubile
  - (2) **infinite soluzioni**: l'equazione $0=0$ si elimina e resta $3x-2y=1$, cioè $2y=3x-1$, $\ y=\tfrac12(3x-1)$
- $b-2\neq0$: dividendo per $b-2$ ($\tfrac{1}{b-2}\mathrm{II}\to\mathrm{II}$) si ottiene $\left[\begin{array}{cc|c} 3 & -2 & 1 \\ 0 & 0 & 1 \end{array}\right]$
  - (1) **no**, il sistema non è risolubile: contiene l'equazione $0=1$ (**impossibile**)

**Caso $a+4\neq0$, cioè $a\neq-4$:** $\ \tfrac{1}{a+4}\mathrm{II}\to\mathrm{II}$
$$\left[\begin{array}{cc|c} 3 & -2 & 1 \\ 0 & 1 & \frac{b-2}{a+4} \end{array}\right]$$
- (1) sì
- (2) **soluzione unica**: $y=\dfrac{b-2}{a+4}$ e, sostituendo, $3x-2\dfrac{b-2}{a+4}=1$

## Riepilogo

| Caso | Forma ridotta | Risolubile? | Soluzioni |
|---|---|---|---|
| pivot solo nelle colonne delle incognite, uno per riga | $\left[\begin{smallmatrix}3&-2&1\\0&1&\frac{b-2}{a+4}\end{smallmatrix}\right]$ | sì | unica |
| riga nulla anche nei termini noti | $\left[\begin{smallmatrix}3&-2&1\\0&0&0\end{smallmatrix}\right]$ | sì | infinite |
| pivot nella colonna dei termini noti | $\left[\begin{smallmatrix}3&-2&1\\0&0&1\end{smallmatrix}\right]$ | no | $\emptyset$ |

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** slide 77, in basso, sezione "RIEPILOGO". **Cosa cercare:** tre matrici a blocchi con la linea rossa "a scala" che segue i pivot e dei pallini azzurri sui pivot. Nel primo caso (sol. unica) i pivot sono nelle due colonne delle incognite; nel secondo (sol. infinite) la linea scende solo di un gradino e la seconda riga è nulla; nel terzo ($\emptyset$) il secondo pivot cade nella colonna dei termini noti. Conviene fare uno screenshot e salvarlo in `99_Tools/Screenshots/GAL/`.

Questa classificazione è generalizzata dal [[82_Teorema_di_Rouche_Capelli]].

## Note collegate
- [[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[67_Operazioni_Elementari_sulle_Righe]]
- [[69_Pivot_e_Matrice_a_Scala]]
- Indice: [[10_Indice_Lezione_9]] · [[00_MOC_GAL]]

#GAL/sistemi-lineari/risoluzione-con-meg
