---
tags: [GAL, base, estrazione, MEG, pivot, nucleo, esempio, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 127-129)"
---

# Estrazione di una base: pivot delle colonne

Per **estrarre** una base conservando i vettori dati, li scrivo come **colonne** di una matrice $A$ e applico il [[68_Metodo_di_Eliminazione_di_Gauss|MEG]] fino a una matrice a scala $U$.

## Proprietà
> [!tip] Colonne e MEG
> Se $A\overset{\text{MEG}}{\leadsto}U$:
> - in generale $\operatorname{Span}(C_1(A),\dots,C_n(A))\neq\operatorname{Span}(C_1(U),\dots,C_n(U))$ (gli span delle colonne **cambiano**);
> - ma $\ker(A)=\ker(U)$, dove
> $$\ker(A)=\{\underline{x}\in\mathbb{R}^n\mid A\underline{x}=\underline{0}\}=\{\underline{x}\in\mathbb{R}^n\mid x_1C_1(A)+x_2C_2(A)+\dots+x_nC_n(A)=\underline{0}\}$$
> $$\ker(U)=\{\underline{x}\in\mathbb{R}^n\mid x_1C_1(U)+x_2C_2(U)+\dots+x_nC_n(U)=\underline{0}\}$$
>
> Le **relazioni di dipendenza lineare** tra le colonne di $A$ e tra le colonne di $U$ sono le stesse ([[84_Nucleo_e_Sistema_Omogeneo_Associato]]).

> [!important] Proprietà (estrazione)
> L'estrazione della base consiste nel **conservare le colonne di $A$ che corrispondono alle colonne di $U$ contenenti i pivot** ([[69_Pivot_e_Matrice_a_Scala]]).

## Esempio
$$W=\operatorname{Span}\left(\begin{bmatrix}0\\2\\1\end{bmatrix},\begin{bmatrix}4\\1\\2\end{bmatrix},\begin{bmatrix}4\\-3\\0\end{bmatrix}\right)$$
Vettori come colonne:
$$A=\begin{bmatrix}0&4&4\\2&1&-3\\1&2&0\end{bmatrix}\xrightarrow{\ \mathrm{I}\leftrightarrow\mathrm{III}\ }\begin{bmatrix}1&2&0\\2&1&-3\\0&4&4\end{bmatrix}\xrightarrow{\ \mathrm{II}-2\mathrm{I}\to\mathrm{II}\ }\begin{bmatrix}1&2&0\\0&-3&-3\\0&4&4\end{bmatrix}$$
$$\xrightarrow[\ \mathrm{III}+\frac43\mathrm{II}\to\mathrm{III}\ ]{\ -\frac13\mathrm{II}\to\mathrm{II}\ }U=\begin{bmatrix}1&2&0\\0&1&1\\0&0&0\end{bmatrix}$$

> [!warning] Da controllare sul quaderno
> Le due operazioni dell'ultimo passaggio sono scritte insieme sulla slide. L'operazione $\mathrm{III}+\frac43\mathrm{II}$ è corretta se applicata alla matrice **prima** di moltiplicare la riga II per $-\tfrac13$ (altrimenti sarebbe $\mathrm{III}-4\,\mathrm{II}$): le ho lette come eseguite in parallelo.

Relazioni tra le colonne di $U$: risolvo il sistema omogeneo aggiungendo la riga $\lambda_3=t$ (come in [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]]):
$$\left[\begin{array}{ccc|c}1&2&0&0\\0&1&1&0\\0&0&1&t\end{array}\right]\leadsto\left[\begin{array}{ccc|c}1&2&0&0\\0&1&0&-t\\0&0&1&t\end{array}\right]\leadsto\left[\begin{array}{ccc|c}1&0&0&2t\\0&1&0&-t\\0&0&1&t\end{array}\right]$$
Con $t=1$:
$$2C_1(U)-C_2(U)+C_3(U)=\underline{0}\ \Rightarrow\ C_3(U)=C_2(U)-2C_1(U)$$
e quindi, per $\ker(A)=\ker(U)$, la stessa relazione vale per $A$:
$$2C_1(A)-C_2(A)+C_3(A)=\underline{0}\ \Rightarrow\ C_3(A)=C_2(A)-2C_1(A)$$

$\Rightarrow$ **scarto la terza colonna e conservo le prime due**: i pivot di $U$ sono nelle colonne 1 e 2. Base estratta:
$$\left\{\begin{bmatrix}0\\2\\1\end{bmatrix},\begin{bmatrix}4\\1\\2\end{bmatrix}\right\},\qquad\dim W=2.$$

> [!note] Osservazione (non presente negli appunti)
> Verifica diretta: $C_2(A)-2C_1(A)=\begin{bmatrix}4\\1\\2\end{bmatrix}-2\begin{bmatrix}0\\2\\1\end{bmatrix}=\begin{bmatrix}4\\-3\\0\end{bmatrix}=C_3(A)$. Il numero di pivot è $r(A)=2=\dim W$ ([[73_MEG_e_Rango]]).

## Note collegate
- [[122_Estrazione_e_Completamento_Due_Problemi_Classici]]
- [[123_Base_per_Costruzione_Libera_con_il_MEG_sulle_Righe]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[69_Pivot_e_Matrice_a_Scala]]
- Successiva: [[125_Completamento_ad_una_Base]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/base/estrazione
