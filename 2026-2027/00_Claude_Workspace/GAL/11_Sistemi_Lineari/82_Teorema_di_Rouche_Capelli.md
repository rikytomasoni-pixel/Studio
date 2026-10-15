---
tags: [GAL, sistemi-lineari, teorema, rouche-capelli, rango, MEG, lezione-9]
data: 2026-10-12
lezione: 9
fonte: "GAL_2026-2027_-_20261012_-_LEZIONE_9.pdf (slide 78-81)"
destinazione: "20_Geometria_Algebra_Lineare/11_Sistemi_Lineari"
---

# Teorema di Rouché-Capelli

> [!abstract] Teorema 9.1 (Teorema di Rouché-Capelli)
> **HP:** sia $A\underline{x}=\underline{b}$ un sistema lineare, $A\in M_{\mathbb{K}}(m,n)$.
>
> **TH1:** il sistema $A\underline{x}=\underline{b}$ è risolubile se, e solo se, $r(A)=r(A\mid\underline{b})$.
>
> **TH2:** se $r=r(A)=r(A\mid\underline{b})$, allora esistono $n-r+1$ vettori colonna $\underline{v}_0,\underline{v}_1,\dots,\underline{v}_{n-r}\in\mathbb{K}^n$ tali che tutte e sole le soluzioni del sistema sono descritte da
> $$\underline{x}=\underline{v}_0+t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$$
> dove $t_1,\dots,t_{n-r}\in\mathbb{K}$ (parametri liberi).

## Dimostrazione

**Struttura.** $A\underline{x}=\underline{b}$ risolubile $\iff r(A)=r(A\mid\underline{b})$ equivale a dimostrare due implicazioni:
- $A\underline{x}=\underline{b}$ risolubile $\Rightarrow r(A)=r(A\mid\underline{b})$ (equivalentemente: $r(A)\neq r(A\mid\underline{b})\Rightarrow$ non risolubile);
- $r(A)=r(A\mid\underline{b})\Rightarrow A\underline{x}=\underline{b}$ risolubile.

**Passo 1: MEG sulla rappresentazione del III tipo.**
$$[A\mid\underline{b}]\ \xrightarrow{\ \text{MEG}\ }\ [U\mid\underline{b}']$$
Per definizione di rango ([[63_Rango_di_una_Matrice]], [[73_MEG_e_Rango]]): $r=r(A)=r(U)=\#\text{pivot di }U$.

**Passo 2: guardo l'ultima colonna.** Ci sono due possibilità.

1. **Nessun pivot nell'ultima colonna:** le righe dalla $r+1$ in poi sono nulle (anche nei termini noti) e
$$r(A)=r(A\mid\underline{b})$$
2. **Un pivot nell'ultima colonna** (sulla riga $r+1$, con $b'_{r+1}\neq0$):
$$r(A\mid\underline{b})=r(A)+1\qquad(r(A)\neq r(A\mid\underline{b}))$$
L'equazione sulla riga $r+1$ dice $0=b'_{r+1}\neq0$, quindi $A\underline{x}=\underline{b}$ **non è risolubile**.

**Passo 3: il caso (1), ricerca delle soluzioni.** Divido le variabili in due gruppi:
- **variabili dipendenti**: corrispondono alle colonne contenenti i pivot ($r$ variabili);
- **variabili indipendenti**: corrispondono alle colonne non contenenti pivot ($n-r$ variabili).

Suppongo che le variabili dipendenti siano le prime $r$ (le righe nulle in fondo si possono eliminare).

Aggiungo $n-r$ equazioni (fittizie) per fissare le variabili indipendenti:
$$x_{r+1}=t_1,\ \dots,\ x_n=t_{n-r}\qquad t_i\in\mathbb{K}$$
Il sistema diventa un sistema con $n$ equazioni e $n$ incognite, che risolvo per **sostituzione all'indietro**:

$$\left[\begin{array}{ccc|ccc|c} p_1 & & * & * & \dots & * & b'_1\\ & \ddots & * & * & \dots & * & \vdots\\ 0 & & p_r & * & \dots & * & b'_r\\ \hline 0 & \dots & 0 & 1 & & 0 & t_1\\ \vdots & & \vdots & & \ddots & & \vdots\\ 0 & \dots & 0 & 0 & & 1 & t_{n-r}\end{array}\right]\qquad p_i\neq 0$$

- **Step 1:** sostituisco le $t_i$ nelle prime $r$ equazioni: i termini noti diventano $b'_i+\sum_j c_{ij}\,t_j$ (per opportuni coefficienti $c_{ij}$).
- **Step 2:** sostituisco a ritroso anche tra le prime $r$ equazioni (si continua il MEG fino ad avere pivot uguali a $1$ e zeri sopra di essi).

**Dove arrivo?**
$$\left[\begin{array}{c|c|c} \mathrm{Id}_r & 0 & v_{0i}+\sum_{j=1}^{n-r}v_{ji}\,t_j\\ \hline 0 & \mathrm{Id}_{n-r} & t_1,\dots,t_{n-r}\end{array}\right]$$
cioè
$$\underline{x}=\begin{bmatrix} x_1\\ \vdots\\ x_n\end{bmatrix}=\underbrace{\begin{bmatrix} v_{01}\\ \vdots\\ v_{0r}\\ 0\\ \vdots\\ 0\end{bmatrix}}_{\underline{v}_0\ \text{(parte costante)}}+t_1\underbrace{\begin{bmatrix} v_{11}\\ \vdots\\ v_{1r}\\ 1\\ 0\\ \vdots\\ 0\end{bmatrix}}_{\underline{v}_1}+t_2\underbrace{\begin{bmatrix} v_{21}\\ \vdots\\ v_{2r}\\ 0\\ 1\\ \vdots\\ 0\end{bmatrix}}_{\underline{v}_2}+\dots+t_{n-r}\underbrace{\begin{bmatrix} v_{n-r,1}\\ \vdots\\ v_{n-r,r}\\ 0\\ \vdots\\ 0\\ 1\end{bmatrix}}_{\underline{v}_{n-r}}$$
$\blacksquare$

## Applicazioni
- Esempio numerico con un parametro $k$: [[83_Esempio_Sistema_con_Parametro_k_e_Rouche_Capelli]]
- Il significato di $\underline{v}_0$ e dei $\underline{v}_i$: [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- Caso $r=n$ (nessun parametro libero): [[86_Teorema_di_Cramer]]

## Note collegate
- [[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]
- [[81_Risoluzione_di_un_Sistema_con_MEG_Esempio_Parametrico]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[69_Pivot_e_Matrice_a_Scala]]
- [[63_Rango_di_una_Matrice]]
- [[73_MEG_e_Rango]]
- Indice: [[10_Indice_Lezione_9]] · [[00_MOC_GAL]]

#GAL/sistemi-lineari/teorema-di-rouche-capelli
