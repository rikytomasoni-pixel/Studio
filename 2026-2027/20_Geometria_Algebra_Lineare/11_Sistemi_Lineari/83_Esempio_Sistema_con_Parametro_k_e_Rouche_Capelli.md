---
tags: [GAL, sistemi-lineari, MEG, esempio, rouche-capelli, parametri, lezione-10]
data: 2026-10-14
lezione: 10
fonte: "GAL_2026-2027_-_20261014_-_LEZIONE_10.pdf (slide 83-84)"
---

# Esempio: sistema con parametro $k$ e Rouché-Capelli

**Testo.** Determino le soluzioni, al variare di $k\in\mathbb{R}$, del sistema lineare rappresentato dalla matrice
$$\left[\begin{array}{ccc|c} 5 & 2 & 1 & 1+k\\ 2 & 2 & -2 & k\\ 1 & -2 & 5 & 1+2k\end{array}\right]$$

## Riduzione con il MEG ([[68_Metodo_di_Eliminazione_di_Gauss]])

Scambio $\mathrm{I}\leftrightarrow\mathrm{III}$ per avere pivot uguale a $1$:
$$\left[\begin{array}{ccc|c} 1 & -2 & 5 & 1+2k\\ 2 & 2 & -2 & k\\ 5 & 2 & 1 & 1+k\end{array}\right]$$
$\mathrm{II}-2\mathrm{I}\to\mathrm{II}$, $\ \mathrm{III}-5\mathrm{I}\to\mathrm{III}$:
$$\left[\begin{array}{ccc|c} 1 & -2 & 5 & 1+2k\\ 0 & 6 & -12 & -2-3k\\ 0 & 12 & -24 & -4-9k\end{array}\right]$$
$\mathrm{III}-\tfrac{12}{6}\mathrm{II}=\mathrm{III}-2\,\mathrm{II}\to\mathrm{III}$:
$$\left[\begin{array}{ccc|c} 1 & -2 & 5 & 1+2k\\ 0 & 6 & -12 & -2-3k\\ 0 & 0 & 0 & -3k\end{array}\right]$$

## Ranghi
- $r(A)=2\quad\forall k\in\mathbb{R}$
- $r(A\mid\underline{b})=\begin{cases}2 & k=0\\ 3 & k\neq0\end{cases}$ (per $k\neq0$ compare un pivot nella colonna dei termini noti, $-3k$)

## Conclusione per il [[82_Teorema_di_Rouche_Capelli]]
- **$k\neq0$:** $r(A)<r(A\mid\underline{b})\Rightarrow$ il sistema **non è risolubile**.
- **$k=0$:** $r(A)=r(A\mid\underline{b})\Rightarrow$ il sistema è risolubile e le soluzioni sono del tipo $\underline{v}_0+t_1\underline{v}_1$, con $1=n-r=3-2$.

## Risoluzione per $k=0$
$$\left[\begin{array}{ccc|c} 1 & -2 & 5 & 1\\ 0 & 6 & -12 & -2\\ 0 & 0 & 0 & 0\end{array}\right]$$
L'ultima riga si elimina. Le variabili $x,y$ sono **dipendenti** (colonne con pivot), $z$ è **indipendente**: pongo $z=t_1$.
$$\left[\begin{array}{ccc|c} 1 & -2 & 5 & 1\\ 0 & 6 & -12 & -2\\ 0 & 0 & 1 & t_1\end{array}\right]$$
$\mathrm{I}-5\mathrm{III}\to\mathrm{I}$, $\ \mathrm{II}+12\mathrm{III}\to\mathrm{II}$:
$$\left[\begin{array}{ccc|c} 1 & -2 & 0 & 1-5t_1\\ 0 & 6 & 0 & -2+12t_1\\ 0 & 0 & 1 & t_1\end{array}\right]$$
$\tfrac16\mathrm{II}\to\mathrm{II}$:
$$\left[\begin{array}{ccc|c} 1 & -2 & 0 & 1-5t_1\\ 0 & 1 & 0 & -\frac13+2t_1\\ 0 & 0 & 1 & t_1\end{array}\right]$$
$\mathrm{I}+2\mathrm{II}\to\mathrm{I}$:
$$\left[\begin{array}{ccc|c} 1 & 0 & 0 & \frac13-t_1\\ 0 & 1 & 0 & -\frac13+2t_1\\ 0 & 0 & 1 & t_1\end{array}\right]$$

$$\begin{cases} x=\tfrac13-t_1\\ y=-\tfrac13+2t_1\\ z=t_1\end{cases}\qquad
\begin{bmatrix} x\\ y\\ z\end{bmatrix}=\underbrace{\begin{bmatrix} \frac13\\ -\frac13\\ 0\end{bmatrix}}_{\underline{v}_0}+t_1\underbrace{\begin{bmatrix} -1\\ 2\\ 1\end{bmatrix}}_{\underline{v}_1}$$

## Note collegate
- [[82_Teorema_di_Rouche_Capelli]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[81_Risoluzione_di_un_Sistema_con_MEG_Esempio_Parametrico]]
- [[69_Pivot_e_Matrice_a_Scala]]
- Indice: [[11_Indice_Lezione_10]] · [[00_MOC_GAL]]

#GAL/sistemi-lineari/esempio-rouche-capelli-parametro
