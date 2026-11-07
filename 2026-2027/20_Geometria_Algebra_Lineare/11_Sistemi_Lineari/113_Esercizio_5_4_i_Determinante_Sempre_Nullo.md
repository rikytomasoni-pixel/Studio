---
tags: [GAL, sistemi-lineari, esercizio, parametri, rouche-capelli, determinante]
data: 2026-10-27
lezione: esercizi
fonte: "Esercizio 5.4 (i); svolgimento redatto da Claude, non presente negli appunti"
---

# Esercizio 5.4 (i): determinante sempre nullo

> [!question] Sistema
> $$\begin{cases}y+az=1\\ ax-y=a-1\\ x+y+(1+a)z=1\end{cases}\qquad A=\begin{pmatrix}0&1&a\\ a&-1&0\\ 1&1&1+a\end{pmatrix}$$

## 1. Determinante
Sviluppo lungo la prima riga ([[65_Determinante_Sviluppo_di_Laplace]]):
$$\det A=-1\cdot\big(a(1+a)\big)+a\cdot\big(a+1\big)=0\qquad\forall a$$
Per [[88_Teorema_sull_Invertibilita_della_Matrice]] $r(A)<3$ sempre: non c'è mai soluzione unica. Se esistono soluzioni sono infinite, e bisogna controllare la compatibilità.

## 2. Dipendenza tra le righe
Cerco $\lambda_1R_1+\lambda_2R_2+\lambda_3R_3=\underline{0}$, colonna per colonna:
- colonna $x$: $a\lambda_2+\lambda_3=0\Rightarrow\lambda_3=-a\lambda_2$
- colonna $y$: $\lambda_1-\lambda_2+\lambda_3=0\Rightarrow\lambda_1=(1+a)\lambda_2$
- colonna $z$: $a\lambda_1+(1+a)\lambda_3=0$, verificata.

Con $\lambda_2=1$:
$$(1+a)R_1+R_2-aR_3=\underline{0}$$
Lo spazio delle relazioni ha dimensione 1, quindi $r(A)=2$ per ogni $a$ (anche per $a=0$, dove $R_1\parallel R_2$ ma $R_3$ è indipendente).

## 3. Compatibilità
Per [[82_Teorema_di_Rouche_Capelli]] serve $r(A|\underline{b})=2$: la stessa combinazione deve annullare i termini noti:
$$(1+a)\cdot1+1\cdot(a-1)-a\cdot1=a\overset{!}{=}0\ \Rightarrow\ a=0.$$

## 4. Verifica
- $a=0$: $y=1$, $-y=-1$, $x+y+z=1$ $\Rightarrow$ $y=1$, $x+z=0$: soluzioni $(x,y,z)=(-t,1,t)$, $\infty^1$ (parametri liberi $=3-2=1$).
- $a=1$: $x=y$, $z=1-y$, la terza equazione dà $2=1$: assurdo.

> [!success] Risultato
> Il sistema ha soluzioni $\iff a=0$.

## Note collegate
- [[112_Esercizio_5_4_Sistemi_con_Parametro]]
- [[116_Strategia_Determinante_per_Sistemi_con_Parametro]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[63_Rango_di_una_Matrice]]

#GAL/sistemi-lineari/esercizio-5-4
