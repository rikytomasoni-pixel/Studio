---
tags: [GAL, matrice-inversa, teorema, invertibilita, determinante, rango, dimostrazione, lezione-10]
data: 2026-10-14
lezione: 10
fonte: "GAL_2026-2027_-_20261014_-_LEZIONE_10.pdf (slide 93-95)"
---

# Teorema sull'invertibilità della matrice

> [!abstract] Teorema 10.3 (Teorema sull'invertibilità della matrice)
> Per una matrice $A\in M_{\mathbb{K}}(n,n)$ le seguenti affermazioni sono **equivalenti**:
> - (I) $A$ invertibile
> - (II) $r(A)=n$
> - (III) $\det(A)\neq0$

## Dimostrazione
Dimostrare l'equivalenza di (I), (II), (III) equivale a dimostrare **3 implicazioni** in ciclo: $\mathrm{I}\Rightarrow\mathrm{III}$, $\ \mathrm{III}\Rightarrow\mathrm{II}$, $\ \mathrm{II}\Rightarrow\mathrm{I}$.

### [I ⇒ III]
**HP:** $A$ invertibile. **TH:** $\det(A)\neq0$.

$A$ invertibile significa che esiste $A^{-1}$ tale che $AA^{-1}=A^{-1}A=\mathrm{Id}_n$. Applico il [[74_Teorema_di_Binet]]:
$$A^{-1}A=\mathrm{Id}_n\ \Rightarrow\ \det(A^{-1}A)=\det(\mathrm{Id}_n)\ \Rightarrow\ \det(A^{-1})\det(A)=1$$
$\Rightarrow\det(A^{-1})$ è l'elemento inverso di $\det(A)$ in $\mathbb{K}$ $\Rightarrow\det(A)$ è un elemento invertibile in un campo $\Rightarrow\det(A)\neq0$. $\blacksquare$

### [III ⇒ II]
**HP:** $\det(A)\neq0$. **TH:** $r(A)=n$.

Proprietà/definizioni già discusse:
- $r(A)=r(U)=\#\text{pivot di }U$ (con $U$ matrice a scala ottenuta da $A$ con il MEG: [[73_MEG_e_Rango]]);
- $\det(A)\neq0\iff\det(U)\neq0$ ([[74_Teorema_di_Binet]]).

Devo dimostrare che $\det(U)\neq0\Rightarrow r(U)=n$ (più facile perché $U$ è a scala).

$U$ a scala $\Rightarrow$ $U$ triangolare superiore $\Rightarrow\det(U)=u_{11}u_{22}\cdots u_{nn}$ ([[66_Matrici_Triangolari]]).
$$\det(U)\neq0\Rightarrow u_{11}u_{22}\cdots u_{nn}\neq0\Rightarrow u_{ii}\neq0\ \ \forall i$$
Gli elementi $u_{ii}$ sono tutti **pivot** della matrice ([[69_Pivot_e_Matrice_a_Scala]]), quindi $r(U)=n\Rightarrow r(A)=n$. $\blacksquare$

### [II ⇒ I]
**HP:** $r(A)=n$. **TH:** $A$ invertibile.

Per invertire $A$ a destra devo risolvere $n$ sistemi lineari
$$A\underline{x}=\begin{bmatrix}1\\0\\ \vdots\\0\end{bmatrix},\quad A\underline{x}=\begin{bmatrix}0\\1\\ \vdots\\0\end{bmatrix},\ \dots,\ A\underline{x}=\begin{bmatrix}0\\ \vdots\\0\\1\end{bmatrix}$$
$r(A)=n$ è l'ipotesi chiave del [[86_Teorema_di_Cramer]]. Per il teorema sono sicuro di poter risolvere ogni sistema con $A$ come matrice dei coefficienti. In particolare posso risolvere gli $n$ sistemi che mi interessano (e la soluzione è unica).

Chiamo $B$ la matrice che inverte $A$ a destra, cioè $AB=\mathrm{Id}_n$. Devo giustificare che $B$ funziona anche a sinistra. Per Binet:
$$\det(AB)=\det(A)\det(B)=\det(\mathrm{Id}_n)=1\ \Rightarrow\ \det(B)\neq0\ \overset{\mathrm{III}\Rightarrow\mathrm{II}}{\Longrightarrow}\ r(B)=n$$
Calcolo l'inverso destro di $B$: per il teorema di Cramer ci riesco. Chiamo $C$ il suo inverso destro, cioè $BC=\mathrm{Id}_n$.
$$\begin{cases}AB=\mathrm{Id}_n\\BC=\mathrm{Id}_n\end{cases}\Rightarrow\ B\text{ ha sia l'inverso destro }(C)\text{ che l'inverso sinistro }(A)\Rightarrow A=C$$
(vedi [[61_Unicita_e_Bilateralita_dell_Inversa]]). Dunque
$$\begin{cases}AB=\mathrm{Id}_n\\BA=\mathrm{Id}_n\end{cases}\Rightarrow B=A^{-1}\qquad\blacksquare$$

> [!note] Risposta alla domanda aperta di [[87_Ricerca_della_Matrice_Inversa]]
> Il determinante non è comparso per caso nell'inversione $2\times2$: $\det(A)\neq0$ è equivalente all'invertibilità.

## Note collegate
- [[87_Ricerca_della_Matrice_Inversa]]
- [[86_Teorema_di_Cramer]]
- [[74_Teorema_di_Binet]]
- [[72_Esistenza_della_Matrice_Inversa]]
- [[60_Matrice_Invertibile]]
- [[63_Rango_di_una_Matrice]]
- [[65_Determinante_Sviluppo_di_Laplace]]
- Indice: [[11_Indice_Lezione_10]] · [[00_MOC_GAL]]

#GAL/matrice-inversa/teorema-invertibilita
