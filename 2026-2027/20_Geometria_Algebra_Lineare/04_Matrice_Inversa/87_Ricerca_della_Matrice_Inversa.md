---
tags: [GAL, matrice-inversa, MEG, sistemi-lineari, determinante, lezione-10]
data: 2026-10-14
lezione: 10
fonte: "GAL_2026-2027_-_20261014_-_LEZIONE_10.pdf (slide 87-92)"
---

# Ricerca di una matrice inversa

## Esempio: matrice rettangolare
$$A=\begin{bmatrix} 1 & 2 & 3\\ 4 & 5 & 6\end{bmatrix}\in M(2,3)$$

**Inverso destro.** Cerco $X=\begin{bmatrix} x_{11}&x_{12}\\ x_{21}&x_{22}\\ x_{31}&x_{32}\end{bmatrix}$ tale che $AX=\mathrm{Id}_2$:
$$AX=\begin{bmatrix} x_{11}+2x_{21}+3x_{31} & x_{12}+2x_{22}+3x_{32}\\ 4x_{11}+5x_{21}+6x_{31} & 4x_{12}+5x_{22}+6x_{32}\end{bmatrix}=\begin{bmatrix} 1&0\\0&1\end{bmatrix}$$
$$\iff\begin{cases} x_{11}+2x_{21}+3x_{31}=1\\ x_{12}+2x_{22}+3x_{32}=0\\ 4x_{11}+5x_{21}+6x_{31}=0\\ 4x_{12}+5x_{22}+6x_{32}=1\end{cases}$$
Per calcolare l'inverso destro devo risolvere un sistema lineare con **6 incognite** ($m\cdot n$) e **4 equazioni** ($m\cdot m$).

> [!tip] Domanda e intuizione
> - $\#\text{incognite}=$ gradi di libertà $=$ "capitale di libertà"
> - $\#\text{equazioni}=$ vincoli $=$ "spesa per la libertà"
>
> $\#\text{incognite}\geq\#\text{equazioni}$: sono ottimista sulla ricerca della soluzione. Mi aspetto che $A$ abbia un inverso destro!

**Inverso sinistro.** Cerco $X\in M(3,2)$ tale che $XA=\mathrm{Id}_3$:
$$\begin{bmatrix} x_{11}&x_{12}\\ x_{21}&x_{22}\\ x_{31}&x_{32}\end{bmatrix}\begin{bmatrix} 1&2&3\\4&5&6\end{bmatrix}=\begin{bmatrix} 1&0&0\\0&1&0\\0&0&1\end{bmatrix}$$
La ricerca dell'inverso sinistro equivale alla soluzione di un sistema con **6 incognite** ($n\cdot m$) e **9 equazioni** ($n\cdot n$): $\#\text{incognite}<\#\text{equazioni}$. L'intuizione suggerisce che in questo caso **non** sarò in grado di trovare l'inverso sinistro.

> [!note] Presupposto
> Non sembra plausibile poter calcolare sia l'inverso destro che l'inverso sinistro per matrici **rettangolari**. L'unico caso che lascia uno spiraglio aperto è il caso $m=n$.

## Caso $2\times2$
$$A=\begin{bmatrix} a&b\\c&d\end{bmatrix}\qquad X=\begin{bmatrix} x_{11}&x_{12}\\x_{21}&x_{22}\end{bmatrix}\ ?\qquad AX=\mathrm{Id}_2,\quad XA=\mathrm{Id}_2$$

Cerco l'inverso destro:
$$AX=\mathrm{Id}_2\iff\begin{bmatrix} ax_{11}+bx_{21}&ax_{12}+bx_{22}\\cx_{11}+dx_{21}&cx_{12}+dx_{22}\end{bmatrix}=\begin{bmatrix}1&0\\0&1\end{bmatrix}$$
$$\iff\begin{cases} ax_{11}+bx_{21}=1\\ cx_{11}+dx_{21}=0\end{cases}\ \text{(sistema 1, incognite }x_{11},x_{21})\qquad\begin{cases} ax_{12}+bx_{22}=0\\ cx_{12}+dx_{22}=1\end{cases}\ \text{(sistema 2, incognite }x_{12},x_{22})$$
Non "4 equazioni e 4 incognite", ma **2 sistemi da 2 equazioni e 2 incognite**:
$$\left[A\mid\begin{smallmatrix}1\\0\end{smallmatrix}\right]=\left[\begin{array}{cc|c} a&b&1\\c&d&0\end{array}\right]\qquad\left[A\mid\begin{smallmatrix}0\\1\end{smallmatrix}\right]=\left[\begin{array}{cc|c} a&b&0\\c&d&1\end{array}\right]$$
Indicando con $C_i(\cdot)$ la $i$-esima colonna:
$$AX=\mathrm{Id}_2\iff A\left[C_1(X)\mid C_2(X)\right]=\left[C_1(\mathrm{Id}_2)\mid C_2(\mathrm{Id}_2)\right]\iff AC_1(X)=C_1(\mathrm{Id}_2)\ \text{ e }\ AC_2(X)=C_2(\mathrm{Id}_2)$$

> [!abstract] Morale
> Invertire a destra una matrice $2\times2$ significa risolvere **2 sistemi lineari** con $A$ come matrice dei coefficienti e le 2 colonne di $\mathrm{Id}_2$ come vettori dei termini noti.
> Invertire a destra una matrice $n\times n$ significherà risolvere **$n$ sistemi lineari** con $A$ come matrice dei coefficienti e le $n$ colonne di $\mathrm{Id}_n$ come vettori dei termini noti.

### Obiettivo: svolgere il MEG una volta sola
$$\left[\begin{array}{cc|cc} a&b&1&0\\c&d&0&1\end{array}\right]$$
Suppongo $a\neq0$ (alla fine dovrò occuparmi del caso $a=0$).

$\tfrac1a\mathrm{I}\to\mathrm{I}$:
$$\left[\begin{array}{cc|cc} 1&\frac ba&\frac1a&0\\c&d&0&1\end{array}\right]$$
$\mathrm{II}-c\,\mathrm{I}\to\mathrm{II}$:
$$\left[\begin{array}{cc|cc} 1&\frac ba&\frac1a&0\\0&d-c\frac ba&-\frac ca&1\end{array}\right]$$

**Se $d-c\frac ba=0$:** il secondo sistema ha la seconda equazione $0=1$ $\Rightarrow$ il secondo sistema non è risolubile $\Rightarrow$ la matrice **non è invertibile a destra**.

Devo quindi lavorare sotto l'ipotesi $d-c\frac ba\neq0$:
$$\frac{ad-bc}{a}\neq0\iff ad-bc\neq0\iff\det(A)\neq0$$
(vedi [[28_Determinanti_2x2_e_3x3]]). Allora $d-c\frac ba=\frac{\det(A)}{a}$:
$$\left[\begin{array}{cc|cc} 1&\frac ba&\frac1a&0\\0&\frac{\det(A)}{a}&-\frac ca&1\end{array}\right]\xrightarrow{\ \frac{a}{\det(A)}\mathrm{II}\to\mathrm{II}\ }\left[\begin{array}{cc|cc} 1&\frac ba&\frac1a&0\\0&1&-\frac{c}{\det(A)}&\frac{a}{\det(A)}\end{array}\right]$$
$\mathrm{I}-\tfrac ba\mathrm{II}\to\mathrm{I}$:
$$\left[\begin{array}{cc|cc} 1&0&\frac1a+\frac ba\frac{c}{\det(A)}&-\frac{b}{\det(A)}\\0&1&-\frac{c}{\det(A)}&\frac{a}{\det(A)}\end{array}\right]$$
con
$$\frac1a+\frac ba\frac{c}{\det(A)}=\frac{\det(A)+bc}{a\det(A)}=\frac{ad-bc+bc}{a\det(A)}=\frac{d}{\det(A)}$$
Quindi
$$\left[\begin{array}{cc|cc} 1&0&\frac{d}{\det(A)}&-\frac{b}{\det(A)}\\0&1&-\frac{c}{\det(A)}&\frac{a}{\det(A)}\end{array}\right]$$
e la matrice a destra della barra ($x_{11},x_{12},x_{21},x_{22}$) è
$$A^{-1}=\frac{1}{\det(A)}\begin{bmatrix} d&-b\\-c&a\end{bmatrix}$$
la matrice **inversa a destra**.

> [!todo] Per casa
> Verificare che questa matrice funziona anche a sinistra. *(Lo svolgimento è nella slide 92: $\frac{1}{\det A}\begin{bmatrix}d&-b\\-c&a\end{bmatrix}\begin{bmatrix}a&b\\c&d\end{bmatrix}=\mathrm{Id}_2$ ✓.)*

## Procedimento generale per l'inverso destro
> [!warning] N.B.
> $$[A\mid\text{colonne dei termini noti dei sistemi da risolvere}]=[A\mid\mathrm{Id}]\ \xrightarrow{\ \text{MEG}\ }\ [\mathrm{Id}\mid\text{soluzioni del primo sistema}\ \dots\ \text{soluzioni dell'ultimo sistema}]=[\mathrm{Id}\mid A^{-1}]$$
> Le soluzioni dei sistemi sono le colonne dell'inversa: la prima soluzione è la prima colonna dell'inverso, e così via.

> [!warning] N.B.
> Il verso **sinistro** consiste nel calcolo del prodotto $A^{-1}A=\mathrm{Id}$ (verificato per il caso $2\times2$ nella slide 92).

> [!warning] N.B. — caso $a=0$
> Dovrei studiare il caso $a=0$! Abbiamo anche richiesto $ad-bc\neq0$:
> $$\begin{cases}a=0\\ ad-bc\neq0\end{cases}\iff\begin{cases}a=0\\ bc\neq0\end{cases}\Rightarrow c\neq0$$

> [!question] Domanda aperta
> È stato un caso incontrare il determinante nell'inversione di una matrice $2\times2$? *(La risposta arriva nel [[88_Teorema_sull_Invertibilita_della_Matrice]].)*

## Note collegate
- [[60_Matrice_Invertibile]]
- [[61_Unicita_e_Bilateralita_dell_Inversa]]
- [[72_Esistenza_della_Matrice_Inversa]]
- [[86_Teorema_di_Cramer]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[28_Determinanti_2x2_e_3x3]]
- Indice: [[11_Indice_Lezione_10]] · [[00_MOC_GAL]]

#GAL/matrice-inversa/ricerca-della-matrice-inversa
