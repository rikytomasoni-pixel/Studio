---
tags:
  - AM1
  - continuita
  - weierstrass
  - massimo-minimo
  - bisezione
  - teorema
data: 2026-11-04
lezione: "15-16"
fonte: "AM1 L15 26-27.pdf (pag. 26-28); AM1 L16 26-27.pdf (pag. 2-6)"
---

# Teorema di Weierstrass

> [!abstract] Teorema di Weierstrass
> Sia $f:[a,b]\to\mathbb{R}$ continua in $[a,b]$, $a,b\in\mathbb{R}$, $a<b$. Allora $f$ assume **massimo e minimo (assoluti)** in $[a,b]$, cioè $\exists x_m,x_M\in[a,b]$ tali che
> $$f(x_m)\le f(x)\le f(x_M)\qquad\forall x\in[a,b]$$
> cioè
> $$f(x_m)=\min_{x\in[a,b]}f(x)\in\mathbb{R}\qquad f(x_M)=\max_{x\in[a,b]}f(x)\in\mathbb{R}$$

> [!note] Osservazioni (L15)
> - $x_m$ si dice **punto di minimo assoluto** per $f$ e $f(x_m)$ si dice **minimo assoluto** per $f$; $x_M$ si dice **punto di massimo assoluto** per $f$ e $f(x_M)$ **massimo assoluto** per $f$; $x_m,x_M\in[a,b]$.
> - Se $f:[a,b]\to\mathbb{R}$ continua in $[a,b]$ allora per Weierstrass essa è **limitata** in $[a,b]$ perché
> $$\sup_{[a,b]}f=f(x_M)=\max_{[a,b]}f\in\mathbb{R}\qquad\inf_{[a,b]}f=f(x_m)=\min_{[a,b]}f\in\mathbb{R}$$
> - Se $f:J\subseteq\mathbb{R}\to\mathbb{R}$ con $J$ intervallo e $f$ non è continua, oppure $J$ non è limitato, oppure $J$ non è chiuso, allora la tesi può non valere.

## Dimostrazione (L16, metodo di bisezione)
Cominciamo osservando che se $f:I\to\mathbb{R}$ con $I=I_1\cup I_2$, allora
$$\sup_If=\max\Big\{\sup_{I_1}f,\ \sup_{I_2}f\Big\}$$

Procediamo col **metodo di bisezione**. Sia $a_0=a$, $b_0=b$, $c_0=\frac{b_0+a_0}2$. Per quanto visto sopra, se $\Lambda=\displaystyle\sup_{[a,b]}f\in\overline{\mathbb{R}}$ avremo
$$\Lambda=\sup_{[a_0,b_0]}f=\max\Big\{\sup_{[a_0,c_0]}f,\ \sup_{[c_0,b_0]}f\Big\}$$
Quindi $\displaystyle\sup_{[a_0,c_0]}f=\Lambda$ oppure $\displaystyle\sup_{[c_0,b_0]}f=\Lambda$.
- Se $\displaystyle\sup_{[a_0,c_0]}f=\Lambda$, definiamo $a_1=a_0$, $b_1=c_0$, $c_1=\frac{a_1+b_1}2$.
- Altrimenti deve essere $\displaystyle\sup_{[c_0,b_0]}f=\Lambda$ e definiamo $a_1=c_0$, $b_1=b_0$, $c_1=\frac{a_1+b_1}2$.

Ripetiamo iterativamente per ogni $n\in\mathbb{N}$. Otteniamo due successioni $a_n,b_n$ tali che

1. $a_n$ cresce, $b_n$ decresce
2. $a\le a_n\le b_n\le b\quad\forall n\in\mathbb{N}$
3. $0\le b_n-a_n=\dfrac{b-a}{2^n}\quad\forall n\in\mathbb{N}$
4. $\displaystyle\sup_{[a_n,b_n]}f=\Lambda=\sup_{[a,b]}f$

Poiché $a_n$ cresce e $b_n$ decresce ed entrambe sono limitate per (1) e (2), per il teorema di regolarità delle successioni monotone $\exists\ \bar a=\displaystyle\lim_{n\to\infty}a_n$, $\ \exists\ \bar b=\displaystyle\lim_{n\to\infty}b_n\in\mathbb{R}$. Per permanenza del segno da (2) segue $a\le\bar a\le\bar b\le b$, cioè $\bar a,\bar b\in[a,b]$. Infine da (3), per algebra dei limiti,
$$\bar b-\bar a=\lim_{n\to\infty}(b_n-a_n)=\lim_{n\to\infty}\frac{b-a}{2^n}=0\ \Rightarrow\ \bar b=\bar a\in[a,b]$$
Indichiamo con $x_M=\bar b=\bar a\in[a,b]$. Ci sono due possibilità: $\Lambda=+\infty$ oppure $\Lambda\in\mathbb{R}$.

### $\Lambda=+\infty$ non può essere
Per assurdo, se $\Lambda=+\infty$ allora $\displaystyle\sup_{[a_n,b_n]}f=\Lambda=+\infty$ $\forall n\in\mathbb{N}$, quindi $\forall n\in\mathbb{N}\ \exists x_n\in[a_n,b_n]$ tale che $f(x_n)>n$. Quindi per confronto
$$\lim_{n\to\infty}f(x_n)=+\infty\qquad(*)$$
e per il teorema dei due carabinieri, essendo $a_n\le x_n\le b_n$, $\displaystyle\lim_{n\to\infty}x_n=x_M=\bar a=\bar b$. Per continuità
$$\lim_{n\to\infty}f(x_n)=f\Big(\lim_{n\to\infty}x_n\Big)=f(x_M)\in\mathbb{R}$$
Assurdo perché contraddice $(*)$. Quindi $\displaystyle\sup_{[a,b]}f=\Lambda\in\mathbb{R}$.

### $\Lambda\in\mathbb{R}$: il sup è un massimo
Poiché $\forall n\in\mathbb{N}$ $\Lambda=\displaystyle\sup_{[a_n,b_n]}f$, $\forall\varepsilon>0$ $\exists x\in[a_n,b_n]$ (dipende da $n\in\mathbb{N}$ e da $\varepsilon>0$) tale che $\Lambda-\varepsilon<f(x)\le\Lambda$. Scegliamo $\varepsilon=\frac1n$: allora $\forall n\ge1$ $\exists x_n\in[a_n,b_n]$ tale che
$$\Lambda-\frac1n<f(x_n)\le\Lambda$$
Segue che $\displaystyle\lim_{n\to\infty}f(x_n)=\Lambda$ e, perché $a_n\le x_n\le b_n$, che $\displaystyle\lim_{n\to\infty}x_n=x_M=\bar a=\bar b$ per il teorema dei due carabinieri. Per continuità $\displaystyle\lim_{n\to\infty}f(x_n)=f\Big(\lim_{n\to\infty}x_n\Big)=f(x_M)$. Per unicità del limite
$$f(x_M)=\lim_{n\to\infty}f(x_n)=\Lambda=\sup_{[a,b]}f\ \Rightarrow\ f(x_M)=\max_{[a,b]}f$$
Similmente si dimostra che esiste $x_m\in[a,b]$ tale che $f(x_m)=\displaystyle\min_{[a,b]}f$. $\square$

## Note collegate
- [[111_Teorema_degli_Zeri]]
- [[114_Immagine_di_una_Funzione_Continua_su_un_Intervallo_Chiuso]]
- [[113_Teorema_dei_Valori_Intermedi]]
- [[08_Estremo_Superiore_Inferiore]]
- [[31_Successioni_Monotone]]
- [[100_Teorema_del_Confronto_per_Limiti_di_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/proprieta-globali/weierstrass
